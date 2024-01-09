<template>
    <SectionKnowUs />
    <SectionCyclingTrainings :CyclingTrainings="CyclingTrainings" />
    <SectionKnowUs />
</template>

<script>
import SectionKnowUs from './SectionKnowUs.vue';
import SectionCyclingTrainings from './SectionCyclingTrainings.vue';
import SectionOurEvents from './SectionOurEvents.vue';
export default {
    components: {
        SectionKnowUs,
        SectionCyclingTrainings,
        SectionOurEvents,

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
            ],
            EventsInfo: [
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event1.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event2.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event3.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event4.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event5.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event6.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event7.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event8.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event9.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHoures: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event10.jpg',
                    place: 'Toronto',
                }

            ]
        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped></style>