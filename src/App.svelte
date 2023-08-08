<script lang="ts">
  import Cta from "./components/Cta.svelte";
  import Footer from "./components/Footer.svelte";
  import Hero from "./components/Hero.svelte";
  import Navbar from "./components/Navbar.svelte";
  import Tiles from "./components/Tiles.svelte";
</script>

<div class="App">
  <Navbar />
  <main>
    <Hero
      title="Aplikacja eksperymentu"
      description="Aplikacja ma przypominać stronę główną sklepu internetowego posiadającego wysokiej rozdzielczości grafikę, dwa rodzaje czcionek oraz kilka elementów interfejsu z ikonami."
    />
    <Tiles />
    <Cta title="Druga sekcja graficzna" />
  </main>
  <Footer />
</div>

