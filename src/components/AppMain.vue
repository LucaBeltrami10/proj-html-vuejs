<template>
    <SectionKnowUs />
    <SectionCyclingTrainings />
</template>

<script>
import SectionKnowUs from './SectionKnowUs.vue';
import SectionCyclingTrainings from './SectionCyclingTrainings.vue'
export default {
    components: {
        SectionKnowUs,
        SectionCyclingTrainings,

    },
    data() {
        return {
            CyclingTrainings: [
                {
                    name: 'Riding Lesson',
                    img: 'training-box-1.jpg'
                },
                {
                    name: 'Safeti Driving',
                    img: 'training-box-2.jpg'
                },
                {
                    name: 'Mountain Bike',
                    img: 'training-box-3.jpg'
                },
                {
                    name: 'Trail Drive',
                    img: 'training-box-4.jpg'
                },
                {
                    name: 'Riding Lesson',
                    img: 'training-box-5.jpg'
                }
            ]
        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped></style>