<template>
  <q-layout view="hhh lpr fff" class="bg-black">
    <q-header>
      <q-img
        src="src/assets/images/bg.jpg"
        fit="fill"
        :ratio="16 / 9"
        class="gt-xs dimmed"
      >
        <HeaderNavbar />
        <HeaderCenter />
      </q-img>
      <q-img
        src="src/assets/images/bg.jpg"
        fit="fill"
        :ratio="1"
        class="lt-sm dimmed"
      >
        <HeaderNavbar />
        <HeaderCenter />
      </q-img>
    </q-header>

    <q-page-container>
      <q-page>
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
      </q-page>
    </q-page-container>

    <q-footer class="bg-black ftext">
      <div class="row justify-center">
        <div class="col-md-8 ftext q-ma-xl">
          <div>Questions? Call 000-800-040-1843</div>
          <div class="row">
            <FooterComponent
              v-for="(liItem, index) in footerLi"
              :key="index"
              v-bind="liItem"
            />
          </div>
        </div>
      </div>
    </q-footer>
  </q-layout>
</template>

<script>
import sourceData from "app/data.json";
import HeaderNavbar from "src/components/headercomponent/HeaderNavbar.vue";
import HeaderCenter from "src/components/headercomponent/HeaderCenter.vue";
import MidSectionComponent from "src/components/midSection/MidSectionComponent.vue";
import AccordianComponent from "src/components/accordianComponent/AccordianComponent.vue";
import FooterComponent from "src/components/footercomponent/FooterComponent.vue";
export default {
  components: {
    HeaderNavbar,
    HeaderCenter,
    MidSectionComponent,
    AccordianComponent,
    FooterComponent,
  },
  data() {
    return {
      accordians: sourceData.accordian,
      midSection: sourceData.midSection,
      footerLi: sourceData.footerList,
    };
  },
};
</script>

<style>
</style>
