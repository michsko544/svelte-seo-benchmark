<script lang="ts">
  import Button from "./Button.svelte";
  import ctaImage from "@/assets/cta-neon.png";

  export let title=""
</script>

<section class="cta">
  <img src={ctaImage} alt="Neonowy kaktus" class="cta__image" />
  <div class="cta__content">
    <div class="cta__inner">
      <div class="content-wrapper">
        <div class="cta__wrapper">
          <h1 class="cta__title">{title}</h1>
          <Button>
            <span>AKCJA</span>
          </Button>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
.cta {
  position: relative;
}

.cta__image {
  width: 100%;
  height: 320px;
  object-fit: cover;
}

.cta__content {
  position: absolute;
  top: 50%;
  left: 0;
  translate: 0 -50%;
  width: 100%;
}

.cta__inner {
  padding: 0 64px;
}

.cta__wrapper {
  display: flex;
  gap: 128px;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}

.cta__title {
  font-size: 32px;
  color: var(--color-white);
  max-width: 280px;
  width: 100%;
}

</style>
