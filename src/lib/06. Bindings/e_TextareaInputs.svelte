<script>
  let value = `Some words are *italic*, some are **bold**`;
</script>

{@html value}

<textarea bind:value />

<style>
  textarea {
    width: 100%;
    height: 200px;
  }
</style>
