<template>
<div class="column flex-center text-white">
    <div class="col-5 flex flex-center title" style="width: 75%;">
        <slot name="upTitle"></slot>
    </div>
    <div class="q-py-md"></div>
    <div class="col flex flex-center text-center under-title" style="width: 75%;">
        <slot name="underTitle"></slot>
    </div>
</div>
</template>

<style scoped>
.title{
    font-family: 'Kanit';
    font-style: normal;
    font-weight: 400;
    font-size: 60px;
    line-height: 70px;
    text-align: center;
    text-transform: uppercase;

}

.under-title{
    font-family: 'Kanit';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    text-align: center; 
}
</style>