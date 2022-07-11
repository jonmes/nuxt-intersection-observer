<script setup>
onMounted(() => {
  const observer = new IntersectionObserver(
    (entries) => {
      // console.log("entries value: ", entries[0].target.classList);
      entries.forEach((entry) => {
        entry.target.classList.toggle(
          "[&[show=true]]:visible",
          entry.isIntersecting
        );
        entry.target.classList.toggle(
          "[&[show=true]]:translate-x-0",
          entry.isIntersecting
        );
      });
    },
    {
      threshold: 0.5,
    }
  );

  document.querySelectorAll(".card").forEach((selection) => {
    observer.observe(selection);
  });
});
</script>

<template>
  <div>
    <div class="card-container flex flex-col">
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 invisible translate-x-40 bg-red-400"
      >
        this is first card
      </div>
    </div>
  </div>
</template>
