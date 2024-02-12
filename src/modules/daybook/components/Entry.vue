<template>
  <div class="entry-container mb-3 pointer p-2"
    @click="$router.push({ name:'entry', params:{ id: 10 } })"
  >

    <!-- Titulo -->
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold">15</span>
        <span class="mx-1 fs-5">Febrero</span>
        <span class="mx-2 fs-5 fw-light">2024, lunes</span>
    </div>

    <div class="entry-description">
        Duis cillum do ex aute culpa exercitation sunt sint velit laborum aute incididunt. Mollit non esse mollit eu veniam ad. Ipsum aliqua eiusmod dolore adipisicing commodo culpa nulla ut.
    </div>

  </div>
</template>

<script>
export default {
    name:'EntryItem'
}
</script>

<style lang="scss" scoped>
.entry-container{
    border-bottom: 1px solid #3c3e50;
    transition: 0.2s all ease-in;

    &:hover{
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2s all ease-in;
    }
    .entry-description{
        font-size: 12px;
    }
}
</style>