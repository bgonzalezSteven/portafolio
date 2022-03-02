<template>
  <q-layout view="lHh Lpr lFf">
    <vs-navbar style="margin: 2em 0em 0em 0em;padding: 1em;" center-collapsed v-model="active">
      <template #left>
        <img style="width:3em" src="../assets/web.png" alt="" />
      </template>
      <template #right>
        <vs-button style="font-size: 11pt;" flat success animation-type="vertical">
          Mentorship
          <template #animate> <q-icon name="developer_mode"/>Go </template>
        </vs-button>
        <vs-button style="font-size: 11pt;" gradient warn>Say hello</vs-button>
      </template>
    </vs-navbar>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: "MainLayout",
  data() {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksData,
    };
  },
};
</script>
<style>
.q-layout {
  font-family: 'Open Sans Condensed', sans-serif;
}
.q-page {
  font-family: 'Open Sans Condensed', sans-serif;
  margin-top: 10em;
}
.q-menu {
  font-family: 'Open Sans Condensed', sans-serif;
}
.fixed, .fixed-full, .fullscreen, .fixed-center, .fixed-bottom, .fixed-left, .fixed-right, .fixed-top, .fixed-top-left, .fixed-top-right, .fixed-bottom-left, .fixed-bottom-right {
  position: absolute;
}
</style>