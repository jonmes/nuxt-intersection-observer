<script setup>
const router = useRoute();

onMounted(() => {
  console.log("mounted");
  const card = ref(document.querySelectorAll(".card"));
  const observer = ref(new IntersectionObserver((entries) => {
    console.log("observing");
    entries.forEach(
      (entry) => {
        entry.target.classList.toggle("me", entry.isIntersecting);
      },
      {
        threshold: 0.5,
      }
    );
  }));

  watch(
    router,
    (newroute) => {
      observer.value = new IntersectionObserver((entries) => {
        console.log("observing");
        entries.forEach(
          (entry) => {
            entry.target.classList.toggle("me", entry.isIntersecting);
          },
          {
            threshold: 0.5,
          }
        );
      });
    },

  );
  document.querySelectorAll(".card").forEach((card) => {
    console.log("another observer", card);
    observer.value.observe(card);
  });
});

// onUnmounted(() => {
//   console.log("unmounted");
//   observer.value.disconnect();
// });
</script>

<template>
  <div>
    <NuxtLink to="/"> Go to blogs </NuxtLink>
    <div class="flex flex-col">
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
      <div
        me="true"
        class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
      >
        this is first card me
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  transition: 500ms;
  transform: translateX(100px);
}
.card.me {
  transform: translateX(0);
}
</style>
