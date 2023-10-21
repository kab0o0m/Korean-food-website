<script>
  import { Router, Link, Route } from "svelte-routing";
  import Navbar from "./lib/Navbar.svelte";

  import Home from "./routes/Home.svelte";
  import Posts from "./routes/posts/Posts.svelte";
  import About from "./routes/about/About.svelte";
  export let url = "";
</script>

<Router {url}>
  <Navbar />
  <div>
    <Route path="/" component={Home} />
    <Route path="/posts" component={Posts} />
    <Route path="/about" component={About} />
  </div>
</Router>
