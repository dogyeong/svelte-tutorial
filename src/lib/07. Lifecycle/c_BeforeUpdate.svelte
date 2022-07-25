<script>
  import { onDestroy, beforeUpdate, afterUpdate } from "svelte";

  let blocks = [];
  let div, autoscroll;

  const interval = setInterval(() => {
    blocks = [...blocks, blocks.length];
  }, 1000);

  beforeUpdate(() => {
    autoscroll =
      div && div.offsetHeight + div.scrollTop > div.scrollHeight - 20;
  });

  afterUpdate(() => {
    if (autoscroll) div.scrollTo(0, div.scrollHeight);
  });

  onDestroy(() => {
    clearInterval(interval);
  });
</script>

<div bind:this={div}>
  {#each blocks as block}
    <p>{block}</p>
  {/each}
</div>

<style>
  div {
    max-height: 160px;
    overflow: scroll;
    border: 1px solid grey;
  }
</style>
