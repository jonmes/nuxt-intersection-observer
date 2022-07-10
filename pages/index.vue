<script setup>
onMounted(() => {
  const observer = new IntersectionObserver((entries) => {
    console.log('entries value: ', entries);
  })

  document.querySelectorAll(".card").forEach((selection) => {
    observer.observe(selection)
  })
});
</script>

<template>
  <div>
    <div class="card-container">
      <div class="card">this is first card</div>
    </div>
  </div>
</template>
