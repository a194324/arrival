<template>
  <div class="wrap d-flex flex-column zx">
    <header>
      <slot name="header"></slot>
    </header>
    <main class="flex-fill container-fluid p-0 ">
      <div class="row">
      <slot></slot>
      </div>
    </main>
    <footer>
      <slot name="footer"></slot>
    </footer>
  </div>
</template>

<style lang="scss">
.zx{
  max-width: 1480px;
}

</style>



