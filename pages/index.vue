<script setup>
import gsap from "gsap";

onMounted(() => {
  const observer = new IntersectionObserver(
    (entries) => {
      // console.log("entries value: ", entries[0].target.classList);
      let target = entries.map((entry) => {
        // entry.target.classList.toggle(
        //   "[&[show=true]]:opacity-100",
        //   entry.isIntersecting
        // );
        // entry.target.classList.toggle(
        //   "[&[show=true]]:translate-x-0",
        //   entry.isIntersecting
        // );
        if (entry.isIntersecting) {
          observer.unobserve(entry.target);
          return entry.target;
        }
      });
    },
    {
      threshold: 0.5,
    }
  );

  document.querySelectorAll(".card").forEach((selection) => {
    observer.observe(selection);
  });

  gsap.to(targets, {
    opacity: 1,
  });
});
</script>

<template>
  <div>
    <div class="card-container flex flex-col">
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        this is first card
      </div>
      <div
        show="true"
        class="card p-10 border-2 border-black self-start rounded-xl w-6/12 duration-1000 opacity-0 translate-x-40 bg-red-400"
      >
        Lorem ipsum dolor sit amet consectetur adipisicing elit. In rerum saepe
        minus quisquam obcaecati! Fuga architecto molestiae, dolorum nobis
        repellat reprehenderit libero doloribus unde autem inventore sapiente,
        incidunt eligendi eaque? At ullam hic doloribus. Consequuntur,
        perspiciatis enim provident veniam consequatur laborum quia dolor a,
        modi impedit praesentium vel dolores accusamus eum ex unde laboriosam ut
        sequi. Odio blanditiis repellat magnam. Libero commodi deleniti
        similique dolorum aliquam iure pariatur amet! Repellat, eius! Deleniti
        repellat natus maiores ipsa asperiores fugiat commodi assumenda,
      </div>
    </div>
  </div>
</template>
