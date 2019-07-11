<script>
  import Home from "./Home.svelte";
  import About from "./About.svelte";
  import Blog from "./Blog.svelte";
  import Router, { location } from "svelte-spa-router";

  const routes = {
    "/": Home,
    "/about/:name?": About,
    "/blog": Blog
  };
</script>

<div class="container">
  <Router {routes} />
  <div>current location: {$location}</div>
</div>
<nav class="navbar">
  <a href="#/">#</a>
  <a href="#/about">About</a>
  <a href="#/blog">Blog</a>
</nav>
