<script>
  import Styling from "./d_Styling.svelte";
</script>

<div>
  <p>Nesting Component</p>
  <Styling />
</div>

<style>
  div {
    padding: 1rem;
    background-color: bisque;
  }

  p {
    color: dodgerblue;
  }
</style>
