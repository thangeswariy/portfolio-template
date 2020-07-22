<template>
    <div class="flex flex-col">
        <label class="text-indigo-300 text-2xl font-sans tracking-wide">{{ name }}</label>
        <label class="text-indigo-200 text-sm font-sans font-thin tracking-wide -mt-2"> {{ title }}</label>
    </div>
</template>
<script>
export default {
    props :{
        name : {
            type : String,
            default: 'Your Name'
        },
        title : {
            type: String,
            default: 'Job Title'
        }
    }
}
</script>