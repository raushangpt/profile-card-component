<script>
  let stats = [
    ['80K', 'Followers'],
    ['803K', 'Likes'],
    ['1.4K', 'Photos'],
  ];
</script>

<main class="bg-cyan grid h-screen w-screen place-items-center">
  <section
    class="font-kumbh-sans w-80 select-none overflow-hidden rounded-xl bg-white shadow-xl transition-all hover:shadow-2xl sm:w-96">
    <div class="relative grid place-items-center">
      <div
        class="h-32 w-full bg-[url('./images/bg-pattern-card.svg')] sm:h-40" />

      <div class="flex flex-col items-center pt-16 pb-4">
        <div class="space-x-2">
          <span class="text-blue text-xl font-bold">Victor Crest</span>
          <span class="text-xl text-gray-200">26</span>
        </div>

        <span class="text-gray-100">London</span>
      </div>

      <div class="absolute overflow-hidden rounded-full border-8 border-white">
        <img src="./images/image-victor.jpg" alt="" />
      </div>
    </div>

    <div class="flex justify-between border-t border-gray-100/50 p-8">
      {#each stats as [count, metric]}
        <div class="flex flex-col">
          <span class="text-blue text-center text-xl font-bold">{count}</span>
          <span class="text-center text-gray-100">{metric}</span>
        </div>
      {/each}
    </div>
  </section>
</main>
