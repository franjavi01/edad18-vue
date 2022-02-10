<template>
  <div class="card" style="width: 18rem;">
    <h1 class="text-center">
      <slot name="title"></slot>
    </h1>
    <div class="card-body">
      <p class="card-text text-center">
        <slot></slot>
      </p>
    </div>
  </div>
</template>
