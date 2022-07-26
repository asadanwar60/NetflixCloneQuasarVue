<template>
  <div class="row justify-center">
    <div class="col-md-8 text-white q-ma-xl">
      <div class="row">Questions? Call 000-800-040-1843</div>
      <ul class="row">
        <div class="col-3">
          <li>{{ footerLi.fTitle }}</li>
        </div>
        <!-- <div class="col-3">
          <li>Investor Relations</li>
          <li>Investor Relations</li>
          <li>Investor Relations</li>
          <li>Investor Relations</li>
        </div>
        <div class="col-3">
          <li>Investor Relations</li>
          <li>Investor Relations</li>
          <li>Investor Relations</li>
          <li>Investor Relations</li>
        </div>
        <div class="col-3">
          <li>Investor Relations</li>
          <li>Investor Relations</li>
          <li>Investor Relations</li>
          <li>Investor Relations</li>
        </div> -->
      </ul>
      <div class="row"></div>
    </div>
  </div>
</template>

<script>
import sourceData from "app/data.json";
export default {
  data() {
    return {
      footerLi: sourceData.footerLi,
    };
  },
};
</script>

<style>
</style>
