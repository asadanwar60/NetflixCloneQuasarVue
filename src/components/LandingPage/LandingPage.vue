<template>
  <q-layout view="lHh Lpr lFf">
    <!--Header Section-->
    <q-img src="src/assets/images/bg.jpg" class="dimmed">
      <HeaderNavbar />
      <HeaderCenter />
    </q-img>

    <MidSectionComponent
      v-for="(item, index) in midSection"
      :key="index"
      v-bind="item"
    />

    <!--Accordian Section-->
    <q-separator color="grey" size="6px" />
    <div class="row justify-center q-pb-xl q-pt-xl">
      <div class="col-md-7 col-sm-9 col-xs-12">
        <div class="gt-xs text-center text-white text-h3 q-pb-xl">
          Frequently Asked Questions
        </div>
        <div class="lt-sm text-center text-white text-bold text-h5 q-pb-md">
          Frequently Asked Questions
        </div>
        <AccordianComponent
          v-for="(item, index) in accordians"
          :key="index"
          v-bind="item"
        />
        <div class="q-pt-xl text-white">
          <GetStartedComponent />
        </div>
      </div>
    </div>
    <q-separator color="grey" size="6px" />
    <FooterComponent />
  </q-layout>
</template>

<script>
import sourceData from "app/data.json";
import AccordianComponent from "src/components/accordianComponent/AccordianComponent.vue";
import HeaderNavbar from "../headercomponent/HeaderNavbar.vue";
import HeaderCenter from "../headercomponent/HeaderCenter.vue";
import GetStartedComponent from "../headercomponent/GetStartedComponent.vue";
import MidSectionComponent from "../midSection/MidSectionComponent.vue";
import FooterComponent from "../footercomponent/FooterComponent.vue";

export default {
  name: "LandingPage",
  components: {
    AccordianComponent,
    HeaderNavbar,
    HeaderCenter,
    MidSectionComponent,
    GetStartedComponent,
    FooterComponent,
  },
  data() {
    return {
      accordians: sourceData.accordian,
      midSection: sourceData.midSection,
    };
  },
};
</script>

<style>
</style>
