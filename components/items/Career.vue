<template>
    <div class='flex flex-col py-4'>
        <div class='flex items-center'>
            <label class='uppercase text-gray-600 text-lg font-semibold mr-2'> {{companyName}} </label> | 
            <label class='capitalize text-gray-700 text-lg font-thin ml-2'> {{title}} </label>
        </div>
        <div class='text-sm text-gray-600 uppercase'>
            {{startDate}} - {{endDate}}
        </div>
        <slot name='experience'></slot>
    </div>
</template>
<script>
export default {
    props: {
        companyName: {
            type : String,
            default : 'Company Name'
        },
        title : {
            type : String,
            default : 'Job Title'
        },
        startDate : {
            type : String,
            default : 'Start Date'
        },
        endDate : {
            type : String,
            default : 'End Date'
        }
    }
}
</script>