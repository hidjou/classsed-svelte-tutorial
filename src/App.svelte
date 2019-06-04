<script>
  import "../node_modules/materialize-css/dist/css/materialize.min.css";
  // import "../node_modules/materialize-css/dist/js/materialize.min.js";

  import { Router, Route } from "svelte-routing";

  import Navbar from "./layout/Navbar.svelte";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
</script>

<style>

</style>

<Router>
  <Navbar />
  <div class="container">
    <Route path="/" component={Home} />
    <Route path="/about" component={About} />
  </div>
</Router>
