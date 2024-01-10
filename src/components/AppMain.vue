<template>
    <SectionKnowUs />
    <SectionCyclingTrainings :CyclingTrainings="CyclingTrainings" />
    <SectionOurEvents :EventsInfo="EventsInfo" />
    <SectionOurTrainers :OurTrainers="OurTrainers" />
    <SectionMembershipPlans :subscriptionPlan="subscriptionPlan" />
    <SectionRecentArticles :newArticles="newArticles" />
</template>

<script>
import SectionKnowUs from './SectionKnowUs.vue'
import SectionCyclingTrainings from './SectionCyclingTrainings.vue'
import SectionOurEvents from './SectionOurEvents.vue'
import SectionOurTrainers from './SectionOurTrainers.vue'
import SectionMembershipPlans from './SectionMembershipPlans.vue'
import SectionRecentArticles from './SectionRecentArticles.vue'

export default {
    components: {
        SectionKnowUs,
        SectionCyclingTrainings,
        SectionOurEvents,
        SectionOurTrainers,
        SectionMembershipPlans,
        SectionRecentArticles,

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
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event1.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event2.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event3.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event4.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event5.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event6.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event7.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event8.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event9.jpg',
                    place: 'Toronto',
                },
                {
                    title: 'Toronto Cycling Event 2023',
                    startDate: '2022-06-22',
                    startHours: '01:30',
                    endDate: '2023-08-11',
                    endHours: '07:00',
                    tag: 'Bicycle Race',
                    img: 'event10.jpg',
                    place: 'Toronto',
                }

            ],
            OurTrainers: [
                {
                    img: 'biker1.jpg',
                    name: 'Michael',
                    surname: 'Lee',
                    profession: 'Biker',
                },
                {
                    img: 'biker4.jpg',
                    name: 'Robert',
                    surname: 'Lee',
                    profession: 'Biker',
                },
                {
                    img: 'biker3.jpg',
                    name: 'John',
                    surname: 'Doe',
                    profession: 'Biker',
                },
                {
                    img: 'biker2.jpg',
                    name: 'Emily',
                    surname: 'Brown',
                    profession: 'Biker',
                },
            ],
            subscriptionPlan: [
                {
                    plan: 'Basic',
                    description: 'Learn to ride a bike from the professionals.',
                    img: 'favicon-gobike.png',
                    price: '1000',
                    services: [
                        { included: true, service: 'Phone Mountaineer bike training' },
                        { included: true, service: 'Remote Excellent bike service' },
                        { included: true, service: 'Onsite Safe cycling training' },
                        { included: false, service: 'Saafety helmet on bike' },
                        { included: false, service: 'Free bikes for children' },
                    ]

                },
                {
                    plan: 'Standard',
                    description: 'Learn to ride a bike from the professionals.',
                    img: 'favicon-gobike.png',
                    price: '1000',
                    services: [
                        { included: true, service: 'Phone Mountaineer bike training' },
                        { included: true, service: 'Remote Excellent bike service' },
                        { included: true, service: 'Onsite Safe cycling training' },
                        { included: false, service: 'Saafety helmet on bike' },
                        { included: false, service: 'Free bikes for children' },
                    ]

                },
                {
                    plan: 'Premium',
                    description: 'Learn to ride a bike from the professionals.',
                    img: 'favicon-gobike.png',
                    price: '1000',
                    services: [
                        { included: true, service: 'Phone Mountaineer bike training' },
                        { included: true, service: 'Remote Excellent bike service' },
                        { included: true, service: 'Onsite Safe cycling training' },
                        { included: true, service: 'Saafety helmet on bike' },
                        { included: true, service: 'Free bikes for children' },
                    ]

                },
            ],
            newArticles: [
                {
                    data: '22.06.2022',
                    subject: 'Bike',
                    title: 'Road bike or mountain bike?',
                    preview: 'Compared to simila road bikes with a solid frame structure, [...] ',
                },
                {
                    data: '22.06.2022',
                    subject: 'Bike',
                    title: 'What is mountain biking called?',
                    preview: 'Mountain biking is one of the most popular outdoor sport, [...] ',
                },
                {
                    data: '22.06.2022',
                    subject: 'Bike',
                    title: 'How much should you cycle a day?',
                    preview: 'In order to get the right benefit from the exercise [...] ',
                },
                {
                    data: '22.06.2022',
                    subject: 'Bike',
                    title: 'Road bike or mountain bike?',
                    preview: 'It take 5 km and 10 minutes, sir. But at [...] ',
                },
            ],
        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped></style>