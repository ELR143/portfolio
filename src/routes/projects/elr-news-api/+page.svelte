<script>
  import github from "$lib/assets/icons/github-icon.svg";
  import endpoints from "$lib/assets/elr-news-api/elr-news-endpoints.png";
  import model from "$lib/assets/elr-news-api/elr-news-model.png";
</script>

<section class="p-10 lg:p-32 flex flex-col gap-24">
  <h1 class="pt-4 text-5xl font-semibold text-center">
    <span
      class="font-bold bg-gradient-to-r from-red-700 to-green-700 via-blue-700 text-transparent bg-clip-text"
      >ELR-news API</span
    >
  </h1>

  <div class="flex flex-row gap-16">
    <p class="text-base sm:text-lg md:text-xl w-3/4">
      The ELR-news API is a RESTful API built with Node.js that imitates the back-end of a real
      world application, such as Reddit. It uses a PostgreSQL database to store
      articles, users and user comments. Its current functionality includes
      users can view and add comments to articles, upvote and downvote an
      article and delete their own comments.
    </p>
    <div class="flex flex-col gap-4 justify-center">
      <div class="flex justify-start items-center gap-4">
        <a href="https://github.com/ELR143/elr143-news-server" target="_blank">
          <img
            src={github}
            class="w-8 bg-gradient-to-r from-red-700 to-green-700 via-blue-700 hover:transform hover:scale-125 hover:transition-colors hover:bg-gradient-to-r hover:from-green-700 hover:to-red-700 hover:via-blue-700 rounded-lg p-1"
            alt="link to frontend"
          />
        </a>
        <p>GitHub</p>
      </div>
    </div>
  </div>
  
  <div class="flex flex-row">
    <img
      class="w-full mx-3"
      src={endpoints}
      alt="screenshot of endpoints.json"
    />
    <img
      class="w-full mx-3"
      src={model}
      alt="screenshot of model"
    />
    
  </div>
  <p class="text-base sm:text-lg md:text-xl">
    The home page helps the user navigate to different pages. You can navigate
    back to this page from anywhere by pressing the top left icon, or to the
    profile page by pressing the top right. The file-based routing in Next.js
    made this very easy to implement.
  </p>
</section>
