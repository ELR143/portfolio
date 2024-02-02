<script>
    import portrait from '$lib/assets/IMG_9240.png'
  </script>
  
  <main class="scroll-smooth flex flex-col flex-1 p-4">
    <section
      id="introPage"
      class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
      <div
        class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
      >
        <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
          Hi! I'm <span class="font-bold bg-gradient-to-r from-violet-500 to-lime-400 text-transparent bg-clip-text">Emma</span> <br />
          Junior Software <span class="font-bold bg-gradient-to-r from-violet-500 to-lime-400 text-transparent bg-clip-text">Developer</span>
        </h2>
        <p class="text-base sm:text-lg md:text-xl">
          After recently graduating from the Northcoders Software Development bootcamp, I am excited to apply my new skills as a Junior Software Developer.
          
        </p>
      </div>

      <div class="relative grid place-items-center">
        <img
        src={portrait}
        alt="Portrait"
        class="rounded-lg max-h-[60vh]"
        />
      </div>

      
    </section>
  
    
  
    <!-- <section
      id="about"
      class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
      <div
        class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
      >
        <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
        <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
          A bit <span class="text-violet-400">about</span> me.
        </h3>
      </div>
      <p class="mx-auto font-semibold text-lg sm:text-xl md:text-2xl">
        I am . . .
      </p>
      <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
        {#each benefits as benefit, index}
          <div class="flex gap-6 sm:gap-8">
            <p
              class="text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
            >
              {index + 1}
            </p>
            <div class="flex flex-col gap-6 sm:gap-8">
              <h3 class="text-2xl sm:text-3xl md:text-5xl">
                {benefit.name}
              </h3>
              <p>{benefit.description}</p>
            </div>
          </div>
        {/each}
      </div>
    </section> -->
  </main>
  