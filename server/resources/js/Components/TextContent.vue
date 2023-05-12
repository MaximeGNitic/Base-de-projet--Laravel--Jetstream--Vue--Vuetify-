<template>
    <div class="column flex-center text-white">
        <div class="col title" style="width: 75%;">
            <slot name="upTitle"></slot>
        </div>
        <div class="q-py-md"></div>
        <div class="col under-title" style="width: 75%;">
            <slot name="underTitle"></slot>
        </div>
        <div class="col list-title" style="width: 75%">
            <slot name="listTitle"></slot>
        </div>
        <div class="col under-title" style="width: 75%">
            <slot name="listContent"></slot>
        </div>
        <div class="col under-title" style="width: 75%;">
            <slot name="underTitle2"></slot>
        </div>
    </div>
    </template>
    
    <style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Kanit&display=swap');
    .title{
        font-style: normal;
        font-weight: 400;
        font-size: 45px;
        line-height: 55px;
        text-transform: uppercase;
    }
    
    .under-title{
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 24px;
    }

    .list-title{
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 24px;
    }
    </style>