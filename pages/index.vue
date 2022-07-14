<script setup>
const root = ref(null);
const target = ref(null);

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

  target.value.forEach((card) => {
    observer.observe(card);
  });
});
</script>

<template ref="root">
  <div>
    <NuxtLink to="/blogs" class="mb-60">Got blog</NuxtLink>

    <div v-for="i in 1" class="flex flex-col">
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
      <div>
        <div>hello</div>
        <div>
          <p
            ref="target"
            class="card p-10 border-2 border-black self-start rounded-xl bg-red-400"
          >
            this is first card show
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  transition: 500ms;
  transform: translateX(100px);
  opacity: 0;
}
.card.show {
  transform: translateX(0);
  opacity: 1;
}
</style>
