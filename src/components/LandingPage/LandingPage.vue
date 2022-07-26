<template>
  <q-layout view="lHh Lpr lFf">
    <!--Header Section-->
    <q-img src="src/assets/images/bg.jpg" class="dimmed">
      <HeaderNavbar />
      <HeaderCenter />
    </q-img>

    <MidSectionLeft />

    <MidSectionRight />

    <MidSectionLeft />

    <MidSectionRight />

    <!--Accordian Section-->
    <q-separator color="grey" dark="true" size="6px" />
    <div class="row justify-center q-pb-xl q-pt-xl">
      <div class="col-md-7 col-sm-12 col-xs-12">
        <div class="text-center text-white text-h3 q-pb-xl">
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
    <q-separator color="grey" dark="true" size="6px" />
    <FooterComponent />
  </q-layout>
</template>

<script>
import AccordianComponent from "src/components/accordianComponent/AccordianComponent.vue";
import HeaderNavbar from "../headercomponent/HeaderNavbar.vue";
import HeaderCenter from "../headercomponent/HeaderCenter.vue";
import GetStartedComponent from "../headercomponent/GetStartedComponent.vue";
import MidSectionLeft from "../midSection/MidSectionLeft.vue";
import MidSectionRight from "../midSection/MidSectionRight.vue";
import FooterComponent from "../footercomponent/FooterComponent.vue";

export default {
  name: "LandingPage",
  components: {
    AccordianComponent,
    HeaderNavbar,
    HeaderCenter,
    MidSectionLeft,
    MidSectionRight,
    GetStartedComponent,
    FooterComponent,
  },
  data() {
    return {
      accordians: [
        { label: "What is Netflix ?", description: "Hello" },
        { label: "How much does Netflix cost ?", description: "Asad" },
        { label: "Where can I watch ?", description: "Anwar" },
        { label: "How do I cancel ?", description: "Ahmed" },
        { label: "What can I watch on Netflix ?", description: "Sania" },
        { label: "Is Netflix good for kids ?", description: "Sania" },
      ],
    };
  },
};
</script>

<style>
</style>
