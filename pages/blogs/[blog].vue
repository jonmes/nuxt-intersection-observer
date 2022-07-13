<script setup>
onMounted(() => {
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(
      (entry) => {
        entry.target.classList.toggle("show", entry.isIntersecting);
      },
      {
        threshold: 0.5,
      }
    );
  });

  document.querySelectorAll(".show").forEach((selection) => {
    observer.observe(selection);
  });
});
</script>
<template>
  <div>
    <NuxtLink to="/blogs"> Go to Home </NuxtLink>
    <div class="flex flex-col">
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card show
      </div>
    </div>
  </div>
</template>
