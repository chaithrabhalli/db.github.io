<script>
  import Router from "svelte-spa-router";
  import Home from "./routes/Home.svelte";
  import UID from "./routes/UIDesigns.svelte";
  import WandM from "./routes/WebandMobile.svelte";
  import PVA from "./routes/PVA.svelte";
  import FineArts from "./routes/FineArts.svelte";
  import PrintMedia from "./routes/PrintMedia.svelte";

  const routes = {
    // Exact path
    "/": Home,
    "/uidesign": UID,
    "/wandm": WandM,
    "/pva": PVA,
    "/finearts": FineArts,
    "/printmedia": PrintMedia
  };
</script>

<!-- <body> -->
<Router {routes} />
<!-- </body> -->
