<template>
  <v-app>
    <v-app-bar 
      app dark 
      src="https://picsum.photos/1920/1080?random"
      color="#fcb69f"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top left, rgba(19,84,122,.5), rgba(128,208,199,.8)"
        ></v-img>
      </template>
      <div class="d-flex align-center mr-2">
        MINIPROJECT
      </div>
      <v-btn to="/tutorials" text>
        List
      </v-btn>
      <v-btn to="/add" text>
        Add New
      </v-btn>
    </v-app-bar>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>
<script>
export default {
  name: "app",
};
</script>