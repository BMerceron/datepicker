<script lang="ts">
import { ref, defineComponent } from 'vue'

export default defineComponent({
    name: 'DatePicker',
    data() {
        return {
            days: [
                { day: 'lundi', id: 0 },
                { day: 'mardi', id: 1 },
                { day: 'mercredi', id: 2 },
                { day: 'jeudi', id: 3 },
                { day: 'vendredi', id: 4 },
                { day: 'samedi', id: 5 },
                { day: 'dimanche', id: 6 },
                { day: 'lundi', id: 7 },
                { day: 'mardi', id: 8 },
                { day: 'mercredi', id: 9 },
                { day: 'jeudi', id: 10 },
                { day: 'vendredi', id: 11 },
                { day: 'samedi', id: 12 },
                { day: 'dimanche', id: 13 },
                { day: 'lundi', id: 15 },
                { day: 'mardi', id: 16 },
                { day: 'mercredi', id: 17 },
                { day: 'jeudi', id: 18 },
                { day: 'vendredi', id: 19 },
                { day: 'samedi', id: 20 },
                { day: 'dimanche', id: 21 },
                { day: 'lundi', id: 22 },
                { day: 'mardi', id: 23 },
                { day: 'mercredi', id: 24 },
                { day: 'jeudi', id: 25 },
                { day: 'vendredi', id: 26 },
                { day: 'samedi', id: 27 },
                { day: 'dimanche', id: 28 },
                { day: 'samedi', id: 29 },
                { day: 'dimanche', id: 30 },
                { day: 'samedi', id: 31 },
            ],
            month: 'January'
        }
    },
})
</script>

<template>
    <div class="datePicker">
        <div class="date" v-for="d in days" v-bind:key="d.id">
            {{ d.id }}
        </div>
    </div>
</template>
<style scoped lang="css">
.datePicker {
    width: 200px;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
}
.date {
    max-width: 8px;
    max-height: 8px;
    padding: 10px;
}
</style>