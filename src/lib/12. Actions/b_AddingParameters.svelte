<script>
  import { longpress } from "./longpress";

  let pressed = false;
  let duration = 2000;
</script>

<label>
  <input type="range" bind:value={duration} max={2000} step={100} />
  {duration}ms
</label>

<button
  use:longpress={duration}
  on:longpress={() => (pressed = true)}
  on:mouseenter={() => (pressed = false)}>press and hold</button
>

{#if pressed}
  <p>congratulations, you pressed and held for {duration}ms</p>
{/if}
