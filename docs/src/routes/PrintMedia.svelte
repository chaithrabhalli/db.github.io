<script>
  import marked from "marked";
  import ContactUS from "./ContactUs.svelte";
  let try_image = "/images/try.jpeg";
  let source = `
 ### Media is a way of getting attention. We help you to come up with media that sends a message across to your coustomers and investors, grabbing their attention and making them to perform the action you want. 

 # Our Services
 #### Print Media
 Flex

 Hoarding

 Signage

 Promotion (digital and print)

 Canvas Print 

 Customized Prints

 Advertisement (Facebook, Insta etc..)
  
`;
  let markdown = marked(source);
</script>

<div class="content-container animated slideInRight">
  <!-- <header class="header">
    <h1 class="header-title">Svelte markdown editor</h1>
  </header> -->

  <div class="output">
    {@html markdown}
    <a href={try_image} download>
      <button class="download-button">
        <span class="button-text">Download Pricing</span>
      </button>
    </a>

    <p class="close-icon" />
  </div>
  <div class="bottomright">
    <ContactUS />
    <!-- HI -->
  </div>
</div>
