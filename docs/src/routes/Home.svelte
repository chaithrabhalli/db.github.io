<script>
  export let name;
  let logo = "/images/Designb.studio.svg";
  let digital = "/images/digital/digital_3.png";
  let home_image = "/images/home_img.svg";
  let and_image = "/images/and_media.svg";
  let blue = "/images/blue.png";
  let red = "/images/red.png";
  let forward = "/images/forward.png";
  import { push, pop, replace } from "svelte-spa-router";
  // let Icon = require("antd");
</script>

<div class="body-padding">
  <img class="logo" src={logo} />

  <div class="flex-container">

    <div class="left-div animated slideInLeft">
      <!-- <img class="digital-engineering" src={digital} /> -->
      <!-- <br /> -->
      <!-- <img height="150" width="200" class="and-media" src={and_image} /> -->
      <p class="digital-engineering">
        digital
        <br />
        engineering
      </p>
      <p class="and-media">and media</p>
    </div>

    <div class="right-div animated slideInRight">
      <img class="home-image" src={home_image} />
    </div>
  </div>

  <ul class="list-content">
    <li id="list1" on:click={() => push('/uidesign')} class="list-item">
      <div class="row">
        <span class="block">ui designs</span>
        <img class="block" src={blue} id="list-forward1" />
        <img src={forward} class="forward float-right" />
      </div>

    </li>

    <li id="list2" on:click={() => push('/wandm')} class="list-item">
      <div class="row">
        <span class="block">web and mobile products</span>
        <img class="block" src={blue} id="list-forward2" />
        <img src={forward} class="forward float-right" />
      </div>

    </li>
    <li id="list3" on:click={() => push('/pva')} class="list-item">
      <div class="row">
        <span class="block">photography , videography and animation</span>
        <img class="block" src={red} id="list-forward3" />
        <img src={forward} class="forward float-right" />
      </div>

    </li>
    <li id="list4" on:click={() => push('/finearts')} class="list-item">
      <div class="row">
        <span class="block">fine arts</span>
        <img class="block" src={red} id="list-forward4" />
        <img src={forward} class="forward float-right" />
      </div>

    </li>
    <li id="list5" on:click={() => push('/printmedia')} class="list-item">
      <div class="row">
        <span class="block">print media</span>
        <img class="block" src={red} id="list-forward5" />
        <img src={forward} class="forward float-right" />
      </div>

    </li>
  </ul>

</div>
