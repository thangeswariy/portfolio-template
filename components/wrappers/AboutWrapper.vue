<template>
    <div class='flex py-8 justify-between items-center px-4 md:px-32 lg:px-48'>
        <div class='w-1/2 md:w-2/3 px-2'>
            <div class='flex flex-col'>
                <label class="text-gray-800 text-lg font-semibold">
                    About Me !
                </label>
                <div class='mt-1 border-red-500 h-1 w-24 border-dotted border-t border-b'></div>
            </div>
            <div class='mt-4 text-gray-600 text-justify'>
                {{aboutMe}}
            </div>
        </div>
        <div class='flex flex-col w-1/2 md:1/3 pl-8 font-semibold'>
            <div class='flex items-center my-1'>
                <img src='~/assets/img/linkedin.png' class='h-4 w-4 mr-1'/>
                <label class="text-gray-800 font-sans tracking-wide text-sm mx-2">LinkedIn:</label>
                <label class="text-gray-600 font-sans tracking-wide text-sm mx-2 font-thin">
                    <a :href="linkedInURL" target="blank"> LinkedIn Profile </a>
                </label>
            </div>
            <div class='flex items-center my-1'>
                <img src='~/assets/img/language.png' class='h-5 w-5 mr-1 -ml-1'/>
                <label class="text-gray-800 font-sans tracking-wide text-sm mx-2">Spoken Languages:</label>
                <label class="text-gray-600 font-sans tracking-wide text-sm mx-2 font-thin">{{ languages }}</label>
            </div>
            <div class='flex items-center my-1'>
                <img src='~/assets/img/location.png' class='h-5 w-5 mr-1 -ml-1'/>
                <label class="text-gray-800 font-sans tracking-wide text-sm mx-2">Nationality:</label>
                <label class="text-gray-600 font-sans tracking-wide text-sm mx-2 font-thin">{{ nationality }}</label>
            </div>
            <div class='flex items-center my-1'>
                <img src='~/assets/img/star.png' class='h-4 w-4 mr-1'/>
                <label class="text-gray-800 font-sans tracking-wide text-sm mx-2">Interest:</label>
                <label class="text-gray-600 font-sans tracking-wide text-sm mx-2 font-thin">{{ interest }}</label>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props : {
        aboutMe: {
            type : String,
            default : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.'
        },
        linkedInURL : {
            type : String,
            default : '#'
        },
        languages : {
            type : String,
            default : 'Languages'
        },
        nationality : {
            type : String,
            default : 'Your Nationaltiy'
        },
        interest : {
            type : String,
            default : 'Your Interest'
        }
    }
}
</script>