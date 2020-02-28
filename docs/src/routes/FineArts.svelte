<script>
  import marked from "marked";
  import ContactUS from "./ContactUs.svelte";
  let try_image = "/images/try.jpeg";
  let source = `
 ### ‘Art’ is with us, from the beginning of time. From caves to modern day media something that didn’t change is art. It has always spoken the same thing. Art expresses you, your point of view and at times its can be more effective than your elevator pitch. 
 # Our Services
 #### Fine Art
 Portraits

 Mandalas

 Sketching

 Wall Painting

 Sculpture 

 Custom Design 

 Illustrations
  
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

  </div>
  <div class="bottomright">
    <ContactUS />
    <!-- HI -->
  </div>
</div>
