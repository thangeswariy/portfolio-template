<template>
    <div class="w-20 h-20 overflow-hidden m-2">
        <img :srcset="source"  class="w-full h-full object-cover bg-white rounded-full p-2"/>
    </div>
</template>
<script>
export default {
    props:{
        source: {
            type: String,
            default: '../img/user.png'
        }
    }
}
</script>