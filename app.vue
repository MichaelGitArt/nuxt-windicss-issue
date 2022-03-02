<template>
  <div class="m-4">
    <h2 class="text-xl mt-4">postcss and `@apply`:</h2>
    
    <main class="main">
      <div class="list">
        <a href="#" class="item">
          Good
        </a>
        <a href="#" class="item">
          Jobs
        </a>
        <a href="#" class="item">
          About
        </a>
      </div>
    </main>

    <hr>

    <h2 class="text-xl mt-4">plain windicss classes:</h2>
    <main class="p-4 border border-gray-500">
      <div class="py-2 flex justify-center">
        <a href="#" class="text-xs text-gray-500 px-2">
          Good
        </a>
        <a href="#" class="text-xs text-gray-500 px-2">
          Jobs
        </a>
        <a href="#" class="text-xs text-gray-500 px-2">
          About
        </a>
      </div>
    </main>

    <hr>

    issue report
  </div>
</template>

<style lang="scss" scoped>
.main {
  @apply p-4 border border-gray-500;
}

.list {
  @apply
    py-2
    flex justify-center
  ;
}

.item {
  @apply
    text-xs text-gray-500
    px-2

    hover:(text-gray-700)
  ;

  &:not(:last-child) {
    @apply
     border-gray-500 border-r-1
    ;
  }
}
</style>