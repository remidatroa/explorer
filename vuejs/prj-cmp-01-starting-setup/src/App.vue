<template>
    <ul>
        <Learning-resource v-for="res in storedResources" 
        :key="res.id" 
        :title="res.title" 
        :description="res.description" 
        :link="res.link">

        </Learning-resource>
    </ul>
</template>
<script>
    import LearningResource from './components/LearningResource.vue'

    export default{
        components:{
            LearningResource
        },

        data() {
            return {
                storedResources: [
                    { 
                        id:'official-guide', 
                        title: 'Official Guide',
                        description: 'The official Vuejs docummentation.',
                        link: 'https://vuejs.org'
                    },
                    {
                        id: 'google',
                        title: 'Google',
                        description: 'Learn to google...',
                        link: 'https://google.com'
                    },
                ]
            };
        }
    }
</script>