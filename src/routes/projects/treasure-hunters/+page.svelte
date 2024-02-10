<script>
  import django from "$lib/assets/icons/django-icon.svg"
  import next from "$lib/assets/icons/nextjs-icon.svg"
  import psql from "$lib/assets/icons/postgresql.svg"
  import tailwind from "$lib/assets/icons/tailwindcss-icon.svg"
  import maps from "$lib/assets/icons/google-maps.svg"
  import login from "$lib/assets/treasure-hunters/treasure-hunters-login.png";
  import home from "$lib/assets/treasure-hunters/treasure-hunters-home.png";
  import leaderboard from "$lib/assets/treasure-hunters/treasure-hunters-leaderboard.png";
  import map from "$lib/assets/treasure-hunters/treasure-hunters-map.png";
  import mapZoomed from "$lib/assets/treasure-hunters/treasure-hunters-map-zoomed.png";
  import github from "$lib/assets/icons/github-icon.svg";
  import treasure from "$lib/assets/treasure-hunters/treasure-map-svgrepo-com.svg";
</script>

<section class="p-10 lg:p-32 flex flex-col gap-12">
  <h1 class="text-5xl md:text-7xl font-semibold text-center">
    <span
      class="font-bold bg-gradient-to-r from-cyan-400 to-orange-500 text-transparent bg-clip-text"
      >Treasure Hunters</span
    >
  </h1>
  <div class='flex flex-row justify-center gap-6 xl:gap-6'>
    <img class='w-12 h-12 'src={next} alt='next.js logo'/>
    <img class='w-12 h-12 'src={tailwind} alt='tailwindcss logo'/>
    <img class='w-12 h-12 'src={django} alt='django logo'/>
    <img class='w-12 h-12 'src={psql} alt='postgreSQL logo'/>
    <img class='w-12 h-12 'src={maps} alt='google maps logo'/>
  </div>

  <div class="flex flex-row gap-16">
    <p class="text-base sm:text-lg md:text-xl w-3/4">
      Treasure Hunters is a full stack web application developed by our team of
      6 developers for the final project at Northcoders. We chose to build the
      backend with Django which required most of our team to teach ourselves
      Python over the Christmas holidays. The frontend was built with Next.js as
      we were familiar with React from the Bootcamp and wanted to try it out.
    </p>
    <div class="flex flex-col gap-4 justify-center">
      <div class="flex justify-start items-center gap-4">
        <a
          href="https://github.com/ELR143/treasure-hunt-frontend"
          target="_blank"
        >
          <img
            src={github}
            class="w-8 bg-gradient-to-r from-cyan-400 to-orange-500 hover:transform hover:scale-125 hover:transition-colors hover:bg-gradient-to-r hover:from-orange-500 hover:to-cyan-400 rounded-lg p-1"
            alt="link to frontend"
          />
        </a>
        <p>Frontend</p>
      </div>

      <div class="flex justify-start items-center gap-4">
        <a
          href="https://github.com/LW95x/treasure-hunt-backend-host"
          target="_blank"
        >
          <img
            src={github}
            class="w-8 bg-gradient-to-r from-cyan-400 to-orange-500 hover:transform hover:scale-125 hover:transition-colors hover:bg-gradient-to-r hover:from-orange-500 hover:to-cyan-400 rounded-lg p-1"
            alt="link to frontend"
          />
        </a>
        <p>Backend</p>
      </div>

      <div class="flex justify-start items-center gap-4">
        <a href="https://treasure-hunters.netlify.app/" target="_blank">
          <img
            src={treasure}
            class="w-8 bg-gradient-to-r from-cyan-400 to-orange-500 hover:transform hover:scale-125 hover:transition-colors hover:bg-gradient-to-r hover:from-orange-500 hover:to-cyan-400 rounded-lg p-1"
            alt="link to frontend"
          />
        </a>
        <p>Try it yourself</p>
      </div>
    </div>
  </div>

  <div class="flex flex-wrap justify-center m-4">
    <img
      class="w-3/4 self-center mb-8"
      src={login}
      alt="treasure hunters home login"
    />
    <p class="text-base sm:text-lg md:text-xl mb-8">
      Users can sign up for an account to create their profile. Authentication
      is handled efficiently by Django, which automatically hashes the user's
      password.
    </p>

    <img class="w-3/4 mb-8" src={home} alt="treasure hunters home page" />
    <p class="text-base sm:text-lg md:text-xl pb-8">
      The home page helps the user navigate to different pages. You can navigate
      back to this page from anywhere by pressing the top left icon, or to the
      profile page by pressing the top right. The file-based routing in Next.js
      made this very easy to implement.
    </p>

    <div class="flex flex-wrap justify-center">
      <img class="w-5/12 mb-8 mr-4" src={map} alt="treasure hunters home map" />
      <img
        class="w-5/12 mb-8 ml-4"
        src={mapZoomed}
        alt="treasure hunters zoomed map"
      />
      <p class="text-base sm:text-lg md:text-xl mb-8">
        GPS tracks the user's location (with permission) in real time, which can
        be toggled on and off. The map shows the location of treasures as
        clusters initially; when the user zooms in to a certain level, the
        treasure radius appears. The user must walk around inside the radius,
        pressing the 'Scan for Treasures!' button periodically. Once the user is
        close enough, the radius will disappear and the treasure will pop up,
        allowing the user to click it and add it to their collection.
      </p>
    </div>

    <img
      class="w-3/4 self-center mb-8"
      src={leaderboard}
      alt="treasure hunters leaderboard"
    />
    <p class="text-base sm:text-lg md:text-xl mb-8">
      The leaderboard compares the database of users based on different
      criteria, such as number of treasures. Users can also add other users as
      friends.
    </p>
  </div>
</section>
