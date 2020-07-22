<template>
    <div class='flex flex-col py-8 justify-between px-4 md:px-32 lg:px-48'>
        <label class="text-gray-800 text-lg font-semibold">Experience</label>
        <div class='mt-1 border-red-500 h-1 w-24 border-dotted border-t border-b'></div>
        <slot name='career'></slot>
    </div>
</template>