<script>
  import Router from "svelte-spa-router";
  import SelectUser from "./routes/selectUser.svelte";
    import Home from "./routes/home.svelte";
</script>

<Router
  routes={{
    "/": SelectUser,
    "/home": Home
  }}
/>
