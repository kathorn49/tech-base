<template>
  <body>
    <div>
      <div id="form-section" class="full-height p-0">
        <FormComponent />
      </div>

      <CardSection />

      <FeatureComponent />
    </div>
  </body>
</template>

<script>
import FormComponent from "./components/FormComponent.vue";
import CardSection from "./components/CardSection.vue";
import FeatureComponent from "./components/FeatureComponent.vue";

export default {
  name: "App",
  components: {
    FormComponent,
    CardSection,
    FeatureComponent,
  },
};
</script>

<style>
* {
  font-family: "Prompt", sans-serif;
}
.full-height {
  min-height: 100vh;
  align-content: center;
}
</style>
