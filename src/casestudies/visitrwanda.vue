<script setup>
import casestudy_temp from '@/components/casestudy_temp.vue'
</script>

<template>
  <casestudy_temp>
    <!-- ************************************************************************** -->
    <template #casestudy_h1>experience<br />rwanda</template>
    <!-- -->
    <template #case-imgs>
      <img src="../assets/visit-rwanda/exp-rwanda-2.webp" alt="" class="case-imgs" />
      <img src="../assets/visit-rwanda/exp-rwanda-1.webp" alt="" class="case-imgs" />
    </template>

    <!--  -->
    <template #case-info-p> web & mobile design,&nbsp;typography&nbsp;copy writing </template>
    <!--  -->
    <template #case-imgs-row>
      <img src="../assets/visit-rwanda/exp-rwanda-4.webp" alt="" class="img-row-2" />
      <img src="../assets/visit-rwanda/exp-rwanda-3.webp" alt="" class="img-row-1" />
    </template>
  </casestudy_temp>
</template>

<style scoped>
.case-imgs {
  width: 100%;
  object-fit: cover;
}

@media (max-width: 1023px) {
  .img-row-1 {
    width: 100%;
    object-fit: cover;
  }
  .img-row-2 {
    height: fit-content;
    width: 100%;
    object-fit: cover;
  }
}

@media (min-width: 1024px) {
  .img-row-1 {
    width: 60vw;
    object-fit: cover;
  }
  .img-row-2 {
    height: fit-content;
    width: 20vw;
    object-fit: cover;
  }
}
</style>
