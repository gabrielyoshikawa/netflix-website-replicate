<script>
  import Router from "svelte-spa-router";
  import SelectUser from "./routes/selectUser.svelte";
</script>

<Router
  routes={{
    "/": SelectUser,
  }}
/>
