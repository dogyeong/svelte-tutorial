<script>
  function getRandomNumber() {
    return Promise.resolve((Math.random() * 100_100).toFixed(0));
  }

  let promise = getRandomNumber();

  function handleClick() {
    promise = getRandomNumber();
  }
</script>

<button on:click={handleClick}> generate random number </button>

{#await promise}
  <p>...waiting</p>
{:then number}
  <p>{number}</p>
{:catch error}
  <p>{error}</p>
{/await}
