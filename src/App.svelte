<script>
  import Eye from "./Eye.svelte";
  import Eyes from "./Eyes.svelte";
</script>

<svg
  width="100%"
  height="100%"
  viewBox="0 0 693 1062"
  version="1.1"
  xmlns="http://www.w3.org/2000/svg"
  xmlns:xlink="http://www.w3.org/1999/xlink"
  xml:space="preserve"
  style="fill-rule:evenodd;clip-rule:evenodd;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:1.5;"
>
  <!-- Background -->
  <g id="Layer1" transform="matrix(1.08451,0,0,1.05357,-29.2817,-37.9286)">
    <rect x="27" y="36" width="639" height="1008" fill="rgb(252,242,217)" />
    <rect x="47" y="56" width="599" height="968" fill="rgb(255,53,31)" />
  </g>

  <!-- Eyes -->
  <Eyes right={false} iris="rgb(208,158,87)" y={738.058} />

  <Eyes y={-9} />
  <Eyes y={140} />
  <Eyes y={290} />
  <Eyes y={439} />
  <Eyes y={589} />

  <!-- Text -->
  <g transform="matrix(1,0,0,1,3.65356,-11.8635)">
    <g transform="matrix(1.02,0,0,1,-8.5617,0)">
      <text
        x="428.085px"
        y="974.145px"
        style="font-family:'BodoniSvtyTwoOSITCTT-Book', 'Bodoni 72 Oldstyle', serif;font-size:35.243px;fill:rgb(252,234,210);"
      >
        F.
      </text>
    </g>
    <g transform="matrix(1.16,0,0,1,-73.1065,0)">
      <text
        x="463.471px"
        y="974.145px"
        style="font-family:'BodoniSvtyTwoOSITCTT-Book', 'Bodoni 72 Oldstyle', serif;font-size:35.243px;fill:rgb(252,234,210);"
      >
        Kafka
      </text>
    </g>
  </g>
  <g id="The-Trial">
    <path
      d="M350.568,919.53C350.568,919.53 339.912,887.821 341.082,869.092"
      style="fill:none;stroke:black;stroke-width:4px;"
    />
    <path
      d="M425.047,913.51C411.216,919.599 403.549,898.331 414.087,895.828C420.037,894.415 417.617,910.431 398.043,914.893C392.75,916.1 389.593,898.871 384.744,899.139C380.433,899.377 378.249,914.374 372.169,913.664C357.856,911.993 363.337,864.329 369.505,865.515C372.757,866.14 377.606,877.44 364.931,895.158"
      style="fill:none;stroke:black;stroke-width:3.5px;"
    />
    <path
      d="M478.936,873.164C476.461,883.978 479.334,903.751 485.202,917.727"
      style="fill:none;stroke:black;stroke-width:3.5px;"
    />
    <path
      d="M497.229,916.2C508.17,911.636 509.584,893.854 506.771,896.884C497.426,906.95 517.537,897.935 517.481,901.872C517.05,932.191 538.221,901.777 538.375,902.024C558.637,934.693 566.337,892.778 573.264,894.279C585.036,896.83 576.459,913.996 572.067,913.05C559.168,910.274 572.662,877.458 582.607,905.575C595.631,942.394 627.092,866.031 616.919,864.499C606.578,862.942 599.863,921.548 627.32,913.327"
      style="fill:none;stroke:black;stroke-width:3.5px;"
    />
    <path
      d="M317.487,858.21C316.419,865.491 365.668,857.477 365.668,857.477C365.668,857.477 328.535,859.725 317.487,858.21Z"
      style="stroke:black;stroke-width:3.5px;"
    />
    <g
      transform="matrix(0.949665,0.0829189,-0.0889564,1.01881,227.326,-40.0013)"
    >
      <path
        d="M317.487,858.21C316.419,865.491 365.668,857.477 365.668,857.477C365.668,857.477 328.535,859.725 317.487,858.21Z"
        style="stroke:black;stroke-width:3.54px;"
      />
    </g>
    <path
      d="M541.307,885.122C541.716,885.494 542.124,885.867 542.533,886.239"
      style="fill:none;stroke:black;stroke-width:3.5px;"
    />
  </g>
</svg>

<style>
  :global(body) {
    background-color: black;
  }
</style>
