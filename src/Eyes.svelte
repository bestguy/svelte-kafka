<script>
	import Eye from "./Eye.svelte";
	import { onMount } from "svelte";
	import { tweened } from "svelte/motion";
	import { cubicOut, quintInOut } from "svelte/easing";

	export let x = 0;
	export let y = 0;
	export let spacing = 306;
	export let delay = (Math.random() * 2 + 1) * 1000;
	export let blinkDelay = (Math.random() * 2 + 3) * 1000;
	export let left = true;
	export let right = true;
	export let iris = undefined;

	const h = tweened(0, {
		duration: 650,
		easing: quintInOut,
	});
	const v = tweened(0, {
		duration: 650,
		easing: quintInOut,
	});
	const pupil = tweened(27, {
		duration: blinkDelay * 1.123,
		easing: quintInOut,
	});
	const open = tweened(1, {
		duration: 100,
		easing: cubicOut,
	});

	onMount(() => {
		let interval = setInterval(() => {
			h.set(Math.random() * 40 - 20);
			v.set(Math.random() * 20 - 10);
		}, delay);

		let blink = setInterval(() => {
			open.set(0);
			setTimeout(() => open.set(1), 100);
		}, blinkDelay);

		let pupils = setInterval(() => {
			pupil.set(Math.random() * 15 + 10);
		}, blinkDelay * 1.123);

		return () => {
			clearInterval(interval);
			clearInterval(blink);
			clearInterval(pupils);
		};
	});
</script>

{#if left}
	<Eye pupil={$pupil} h={$h} v={$v} {x} {y} {iris} open={$open} />
{/if}
{#if right}
	<Eye pupil={$pupil} h={$h} v={$v} x={x + spacing} {y} {iris} open={$open} />
{/if}
