<template>
  <div class="Panel">
    <h1 class="panel">Expansion Panels</h1>
    <v-row justify="center">
      <v-expansion-panels accordion>
        <v-expansion-panel v-for="panel in panels" :key="panel">
          <v-expansion-panel-header>{{ panel.title }}</v-expansion-panel-header>
          <v-expansion-panel-content>{{
            panel.desc
          }}</v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      panels: [
        {
          title: 'Button',
          desc: 'The v-btn component replaces the standard html button with a material design theme and a multitude of options. Any color helper class can be used to alter the background or text color. Try out an interactive screencast on how Vuetify buttons work.',
        },
        {
          title: 'Calenders',
          desc: 'The v-calendar component is used to display information in a daily, weekly, monthly, or category view. The daily view has slots for all day or timed elements, and the weekly and monthly view has a slot for each day. The category view has a slot for each category in the day and timed sections based on the categories given or the categories in the given events. Optionally you can pass in an array of events and they will be rendered over the appropriate days and times.',
        },
        {
          title: 'Cards',
          desc: 'The v-card component is a versatile component that can be used for anything from a panel to a static image. The card component has numerous helper components to make markup as easy as possible. Components that have no listed options use Vue’s functional component option for faster rendering and serve as markup sugar to make building easier. Try out an interactive screencast on how Vuetify cards work.',
        },
        {
          title: 'Chips',
          desc: 'The v-chip component is used to convey small pieces of information. Using the close property, the chip becomes interactive, allowing user interaction. This component is used by the v-chip-group for advanced selection options.',
        },
        {
          title: 'Dialog',
          desc: 'The v-dialog component inform users about a specific task and may contain critical information, require decisions, or involve multiple tasks. Use dialogs sparingly because they are interruptive.',
        },
      ],
    }
  },
}
</script>

<style scoped>
.panel {
  text-align: center;
}
.Panel {
  padding-top: 6%;
}
</style>