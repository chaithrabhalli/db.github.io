<script>
  import marked from "marked";
  let try_image = "/images/try.jpeg";
  import ContactUS from "./ContactUs.svelte";
  let source = `
 ### UI/UX are the visual and functional dimensions of your products. We help you achieve a very balanced and usable interface, fast by rapid experimentation and prorotyping.
 # Our Services
 #### UI Design
 Requirement Gathering & Information Architecture.

 Wireframe.

 Visual Hierarchies & Style Guide.

 Low Fidelity.

 High Fidelity (Interactive) Prototyping.

 Design Testing & Delievery.

 #### Product

 Concept/MVP

 Functional UI - HTML/CSS
  
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
