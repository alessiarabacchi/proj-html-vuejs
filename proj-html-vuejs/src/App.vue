<script>
import AppNavbar from "./components/AppNavbar.vue";
import HeroSection from "./components/HeroSection.vue";
import StatsSection from "./components/StatsSection.vue";
import ValuesSection from "./components/ValuesSection.vue";
import CausesSection from "./components/CausesSection.vue";
import ArticlesSection from "./components/ArticlesSection.vue";
import CallToAction from "./components/CallToAction.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppNavbar,
    HeroSection,
    StatsSection,
    ValuesSection,
    CausesSection,
    ArticlesSection,
    CallToAction,
    AppFooter,
  },
};
</script>

<template>
  <div id="app">
    <app-navbar />
    <hero-section />
    <stats-section />
    <values-section />
    <causes-section />
    <articles-section />
    <call-to-action />
    <app-footer />
  </div>
</template>
