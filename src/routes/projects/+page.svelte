<script>
  import Step from "../../components/Step.svelte";
  let steps = [
    {
      name: "Treasure Hunters",
      icon: "fa-regular fa-gem",
      link: "treasure-hunters",
      status: "complete",
    },
    {
      name: "ELR-news",
      icon: "fa-regular fa-newspaper",
      link: "elr-news",
      status: "complete",
    },
    {
      name: "ELR-news API",
      icon: "fa-solid fa-server",
      link: "elr-news-api",
      status: "complete",
    },
    {
      name: "Dimittis",
      icon: "fa-solid fa-music",
      link: "elr-news-api",
      status: "in progress",
    },
  ];
</script>

<section class="py-20 lg:py-32 flex flex-col gap-24">
  <div class="flex flex-col gap-2 text-center">
    <h6 class="text-lg sm:text-xl md:text-2xl">
      A few of my creative endeavours.
    </h6>
    <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
      Curious to <span class="text-violet-400">see</span> my work?
    </h3>
  </div>

  <div class="grid grid-cols-1 gap-6 sm:gap-10 lg:grid-cols-3 lg:gap-10">
    <Step step={steps[0]}>
      <p>
        Treasure Hunters is a GPS-based web application built using <strong
          class="text-violet-400"
          >Next.js, TailwindCSS, Django, Django REST</strong
        >
      </p>
    </Step>

    <Step step={steps[1]}>
      <p>
        ELR-news is a React CRUD application where users can view and comment on
        articles <strong class="text-violet-400">React</strong>
      </p>
    </Step>

    <Step step={steps[2]}>
      <p>
        ELR-news server is a RESTful API built using <strong
          class="text-violet-400">Node.js & Express.js</strong
        >
      </p>
    </Step>

    <Step step={steps[3]}>
      <p>
        ELR-news server is a RESTful API built using <strong
          class="text-violet-400">Node.js & Express.js</strong
        >
      </p>
    </Step>
  </div>
</section>
