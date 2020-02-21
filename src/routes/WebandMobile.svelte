<script>
  import marked from "marked";
  let try_image = "/images/try.jpeg";
  import ContactUS from "./ContactUs.svelte";

  let source = `
 ### We use tools that puts your products in hands of your users fast, targeting maximum platforms in shorter amount of time. While you gather feedback and imagine changes we implement them for you.
 # Our Services
 #### Product Develpment
 Concept/MVP

 Web Development

 Analytics and App usage data

 Cloud deployment and Scalability

 Data Processing or Repoting at Big Data Scale

 #### Tech Skills

 NodeJS

 ReactJS

 HTML/CSS

 BigData

 Python
  
`;
  let markdown = marked(source);
</script>

<div class="content-container animated slideInRight">
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
