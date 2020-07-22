<template>
    <div class="flex py-8 bg-blue-900 justify-between items-center px-4 md:px-32 lg:px-48">
        <div class="flex items-center">
            <UserImage :source='userImgURL'/>
            <UserNameTitle :name='name' :title='title'/>
        </div>
        <div class='flex flex-col'>
            <div class='flex items-center my-1'>
                <img src="~/assets/img/phone.png" class='h-4 w-4 mx-2'/>
                <label class="text-indigo-300 font-sans tracking-wide text-sm mx-2">Phone :</label>
                <label class="text-indigo-200 font-sans tracking-wide text-sm mx-2 font-thin">{{ phone }}</label>
            </div>
            <div class='flex items-center my-1'>
                <img src="~/assets/img/email.png" class='h-4 w-4 mx-2'/>
                <label class="text-indigo-300 font-sans tracking-wide text-sm mx-2">Email :</label>
                <label class="text-indigo-200 font-sans tracking-wide text-sm mx-2 font-thin"> {{ email }}</label>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        name : {
            type : String,
            default : 'Your Name'
        },
        title : {
            type : String,
            default : 'Your Title'
        },
        userImgURL : {
            type : String,
            default : '../img/user.png'
        },
        phone: {
            type : String,
            default : 'Phone Number'
        },
        email: {
            type : String,
            default : 'Email'
        }
    }
}
</script>