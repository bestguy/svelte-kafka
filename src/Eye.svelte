<script>
	export let iris = "rgb(1,167,229)";
	export let pupil = 27;
	export let h = 0;
	export let v = 0;
	export let x = 0;
	export let y = 0;
	export let open = 1;
</script>

<g id="Eye1" transform={`translate(${x + 72},${y + 107.942})`}>
	<mask id="blink">
		<path
			d="M0,54.058C81.238,-18.163 153.19,-17.875 234,54.058C153.056,125.811 81.24,126.184 0,54.058Z"
			fill="white"
			transform={`translate(0,${54.058 * (1 - open)}) scale(1,${open})`}
		/>
	</mask>
	<g mask="url(#blink)">
		<path
			d="M0,54.058C81.238,-18.163 153.19,-17.875 234,54.058C153.056,125.811 81.24,126.184 0,54.058Z"
			style="fill:rgb(252,242,217);"
		/>
		<circle cx={117 + h} cy={54.058 + v} r="41.704" fill={iris} />
		<circle
			cx={117 + h}
			cy={54.058 + v}
			r={pupil}
			style="fill:rgb(33,31,32);"
		/>
	</g>
</g>
