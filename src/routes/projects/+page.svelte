<script>
  import Step from "../../components/Step.svelte";
  import django from "$lib/assets/icons/django-icon.svg"
  import next from "$lib/assets/icons/nextjs-icon.svg"
  import psql from "$lib/assets/icons/postgresql.svg"
  import tailwind from "$lib/assets/icons/tailwindcss-icon.svg"
  import maps from "$lib/assets/icons/google-maps.svg"
  import react from "$lib/assets/icons/react.svg"
  import css from "$lib/assets/icons/css-3.svg"
  import node from "$lib/assets/icons/nodejs-icon.svg"
  import express from "$lib/assets/icons/express.svg"
  import supabase from "$lib/assets/icons/supabase-icon.svg"

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

<section class="py-20 px-5 lg:py-32 flex flex-col gap-24">
  <div class="flex flex-col gap-2 text-center">
    <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
      Have a look at my <span class="font-bold bg-gradient-to-r from-pink-500 to-orange-500 text-transparent bg-clip-text">projects:</span> 
    </h3>
  </div>

  <div class="grid grid-cols-1 gap-6 sm:gap-10 lg:grid-cols-3 lg:gap-10">
    <Step step={steps[0]}>
      <p>
        Treasure Hunters is a GPS-based web application built during our final project phase with Northcoders.
      </p>
      <div class='flex flex-row justify-center gap-3 xl:gap-6 mt-5'>
        <img class='w-12 h-12 'src={next} alt='next.js logo'/>
        <img class='w-12 h-12 'src={tailwind} alt='tailwindcss logo'/>
        <img class='w-12 h-12 'src={django} alt='django logo'/>
        <img class='w-12 h-12 'src={psql} alt='postgreSQL logo'/>
        <img class='w-11 h-11 'src={maps} alt='google maps logo'/>
      </div>
    </Step>

    <Step step={steps[1]}>
      <p>
        ELR-news is a React CRUD application where users can view and comment on
        articles.
      </p>
      <div class='flex flex-row justify-center gap-6 mt-5'>


        <img class='w-12 h-12 'src={react} alt='react logo'/>
        <img class='w-12 h-12 'src={css} alt='css logo'/>
      </div>
    </Step>

    <Step step={steps[2]}>
      <p>
        ELR-news server is a RESTful API that serves data to the ELR-news frontend, storing articles, users and comments in a PostgreSQL database.
      </p>
      <div class='flex flex-row justify-center gap-6 mt-5'>
        <img class='w-12 h-12'src={node} alt='node.js logo'/>
        <img class='w-12 h-12 bg-slate-100 rounded-lg p-1'src={express} alt='express logo'/>
        <img class='w-12 h-12 'src={psql} alt='postgreSQL logo'/>

      </div>
    </Step>

    <Step step={steps[3]}>
      <p>
        Dimittis will be a web application used by real users to track the attendance of a choir.
      </p>
      <div class='flex flex-row justify-center gap-6 mt-5'>


        <img class='w-12 h-12 'src={react} alt='svelte logo'/>
        <img class='w-12 h-12 'src={tailwind} alt='tailwindcss logo'/>
        <img class='w-12 h-12 'src={supabase} alt='supabase logo'/>
      </div>
    </Step>
  </div>
</section>
