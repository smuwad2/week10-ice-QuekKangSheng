<script>
    //import component
    import SoundIcon from './subcomponents/SoundIcon.vue'
    export default { 
        data() {
            return {
                soundLevel: 0
            }
        },
        components: {
            SoundIcon
        }
    }
</script>

<template>

    Sound level
    <input type="number" min="0" max="3" v-model="soundLevel"> 
    <!-- TODO: Add Code Here to make use of the component -->
    <!-- If static variable you can just use soundlevel= x but since v-model is a dynamic variable, we need to use ":"
    in front of the soundlevel  -->
    <sound-icon :soundlevel="soundLevel"></sound-icon>
</template>

