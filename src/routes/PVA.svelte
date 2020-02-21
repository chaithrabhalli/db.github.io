<script>
  import marked from "marked";
  import ContactUS from "./ContactUs.svelte";

  let try_image = "/images/try.jpeg";
  let source = `
 ### People do not buy goods and services. They buy relationships, stories and magic - Seth Godin. Videos  are a very powerful instrument to narrate your brand’s story, to showcase your service, and to engage with your audience. 
 # Our Services
 #### 2D & 3D animation
 Scripting

 Storyboard / Character Design / Voiceover

 Voiceover

 Animation

 Sound Design

 Motion Graphics

 #### Photograpghy & Videography

 Photo Editing

 Pre-Production

 Filming, Equipment & Acquisition

 Post-Production, Editing, Graphics, Narration

 Music Licensing
  
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
