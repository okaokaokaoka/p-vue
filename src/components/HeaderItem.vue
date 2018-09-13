<template>
  <div id="my-header">
    <v-navigation-drawer></v-navigation-drawer>
    <v-toolbar color="green" dark >
      <v-toolbar-title>徹子の部屋</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>search</v-icon>
      </v-btn>
    </v-toolbar>
  </div>
</template>

<script>
export default {
  name: 'HeaderItem'
}
</script>
