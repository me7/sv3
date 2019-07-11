<script>
  import { pop } from "svelte-spa-router";
  function goBack() {
    pop();
  }
  export let params;
</script>

<h1>About</h1>
<p>name: {params.name} </p>
<button on:click={goBack}>Go Back</button>
