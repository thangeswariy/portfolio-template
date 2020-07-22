<template>
    <div class=" py-8 bg-blue-900 justify-between items-center px-4 md:px-32 lg:px-48 grid grid-cols-1 md:grid-cols-3">
        <div class='flex items-center px-2 py-4 justify-center'>
            <img src='~/assets/img/Honeycomb.png' class='h-12 w-12 mx-2 transform rotate-180'/>
            <div class='flex flex-col text-indigo-300'>
                <label class='text-2xl'>{{project}}</label>
                <label class='text-md font-thin -mt-2'>Completed Projects</label>
            </div>
        </div>
        <div class='flex items-center px-2 py-4 justify-center'>
            <img src='~/assets/img/grinning.png' class='h-12 w-12 mx-2 -ml-8'/>
            <div class='flex flex-col text-indigo-300'>
                <label class='text-2xl'>{{client}}</label>
                <label class='text-md font-thin -mt-2'>Happy Clients</label>
            </div>
        </div>
        <div class='flex items-center px-2 py-4 justify-center'>
            <img src='~/assets/img/trophy.png' class='h-12 w-12 mx-2'/>
            <div class='flex flex-col text-indigo-300'>
                <label class='text-2xl'>{{award}}</label>
                <label class='text-md font-thin -mt-2'>Awards Received</label>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        project : {
            type : String,
            default : 'Number of Project'
        },
        client : {
            type : String,
            default : 'Number of Happy Clients'
        },
        award : {
            type: String,
            default: 'Number of Awards'
        }
    }
}
</script>