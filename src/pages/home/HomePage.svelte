<script>
  import Header from "../../widgets/header/Header.svelte";
  import Footer from "../../widgets/footer/Footer.svelte";
  import Button from "../../shared/ui/Button.svelte";
</script>

<Header />

<main class="home">
  <section class="intro">
    <h1>Welcome to My Portfolio</h1>
    <p>
      Hi, I'm [Your Name], a passionate developer. Explore my projects and get
      in touch!
    </p>
    <Button
      text="View Projects"
      on:click={() => (window.location.href = "/projects")}
    />
  </section>
</main>

<Footer />

<style>
  .home {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
  }
  .intro {
    max-width: 600px;
    text-align: center;
  }
</style>
