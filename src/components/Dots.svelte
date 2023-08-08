<script lang="ts">
  type $$Props = {
    direction?: "left" | "right";
  };

  export let direction = "right"
</script>

<div class="dots" class:dots--right="{direction === "left"}">
  <div class="dot__long"></div>
  <div class="dot__tight"></div>
</div>

<style >
.dots {
  display: flex;
  width: fit-content;
  gap: 8px;
  align-items: center;
}

.dots--right {
  flex-direction: row-reverse;
}

.dot__long {
  width: 32px;
  height: 16px;
  border-radius: 32px;
  background-color: var(--color-pink);
}

.dot__tight {
  width: 16px;
  height: 16px;
  border-radius: 32px;
  background-color: var(--color-pink);
}
</style>
