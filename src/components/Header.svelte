<script>
  export let y;

  let tabs = [
    { name: "About Me", link: "/about" },
    { name: "Projects", link: "/projects" },
  ];
</script>

<header
  class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid " +
    (y > 0
      ? "py-4 bg-slate-950 border-violet-950"
      : "py-6 bg-transparent border-transparent")}
>
  <h1 class="font-medium">
    <a href='/'>Emma Richardson</a>
  </h1>
  <div class="flex flex-row ml-auto pr-4 gap-4">
    {#each tabs as tab, index}
      <a href={tab.link} class="duration-200 hover:text-violet-400">
        <p>
          {tab.name}
        </p>
      </a>
    {/each}
  </div>
</header>
