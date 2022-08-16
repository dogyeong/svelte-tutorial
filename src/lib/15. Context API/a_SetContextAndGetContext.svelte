<script>
  import { setContext, getContext } from "svelte";

  const key = Symbol("contextKey");

  setContext(key, { foo: "bar" });

  const { foo } = getContext(key);
</script>
