<script>
  let close = "/images/close.svg";
  let mail = "/images/mail.svg";
  let whatsapp = "/images/whatsapp.svg";
  import { push, pop, replace } from "svelte-spa-router";
</script>

<div class="flex-verticle">
  <!-- <a href="whatsapp://send?text=Hello World!&phone=+919535136548">
    <img class="contact-class" height="70" width="70" src={whatsapp} />
  </a> -->
  <a
    href="mailto:hello.designb@gmail.com?subject=Hi%20Team&amp;body=Hey%20Designb%2C%0A%0ACan%20you%20please%20provide%20me%20an%20estimate%20for%20%3Cmy%2Bidea%3E%20%0A">
    <img class="contact-class" src={mail} />
  </a>
  <img on:click={() => push('/')} class="contact-class" src={close} />
</div>
