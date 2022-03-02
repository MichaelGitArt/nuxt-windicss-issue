<template>
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
</template>

<style lang="postcss" scoped>
.main {
  @apply p-4;
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