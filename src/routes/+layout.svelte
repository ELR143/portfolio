<script>
  import "../app.css";
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import BallAnimation from "../components/BallAnimation.svelte";

  let y;
  let innerHeight = 0;
  let innerWidth = 0;

  function goToTop() {
    document.body.scrollIntoView();
  }
</script>

<div
  class="relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen"
>
  <Header {y} />

  <slot />
  <Footer />
</div>
<div
  class={"fixed bottom-0 w-full duration-200 flex p-10 " +
    (y > 0
      ? "opacity-full pointer-events-auto"
      : "opacity-0 pointer-events-none")}
>
  <button
    on:click={goToTop}
    class="ml-auto rounded-full aspect-square bg-violet-700 text-slate-950 px-3 sm:px-4 hovering:bg-slate-800 cursor-pointer"
  >
    <i class="fa-solid fa-arrow-up grid place-items-center aspect-square"></i>
  </button>
</div>
<div>
  <BallAnimation />
</div>

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
