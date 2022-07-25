<script>
  import { onDestroy } from "svelte";

  let seconds = 0;
  const interval = setInterval(() => {
    seconds++;
  }, 1000);

  onDestroy(() => clearInterval(interval));
</script>

<div>
  <p>
    The Timer component has been open for
    {seconds}
    {seconds === 1 ? "second" : "seconds"}
  </p>
</div>
