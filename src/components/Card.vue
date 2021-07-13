<template>
  <div>
    <h1>heloo hthre i ma</h1>
    <b-card :title="title" tag="article" style="max-width: 20rem;" class="mb-2">
      <b-card-text>
        {{ para }}
      </b-card-text>

      <b-button href="#" variant="primary">Go somewhere</b-button>
    </b-card>
  </div>
</template>

<script>
export default {
  props: ["title", "para"],
};
</script>

<style></style>
