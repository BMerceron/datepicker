<script lang="ts">
import { ref, defineComponent } from 'vue'
import Title from '../../types/Title'
import CardTitle from './CardTitle.vue'
import CardInputs from './CardInput.vue'
import DatePicker from '../datePicker/DatePicker.vue';

export default defineComponent({
  name: 'CardComponent',
  components: {
    DatePicker
  },
  data() {
    return {
      title: 'Title' as unknown as Title
    }
  },
  computed: {

  },
  methods: {

  }

})
</script>

<template>
  <div>
    <CardTitle :title="title" />
    <Cardinput/>
    <Cardinput/>
    <DatePicker/>
  </div>
</template>

<style scoped></style>
