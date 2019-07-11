<script>
  import { push } from "svelte-spa-router";
  function gotoBlog() {
    push("/blog");
  }
</script>

<h1>Home</h1>
<button class="btn btn-primary" on:click={gotoBlog}>Go To Blog Page</button>
