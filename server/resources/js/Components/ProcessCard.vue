<template>
    <v-container class="text-white d-flex flex-center">
        <v-card class="my-card">
            <v-card-text class="row">
                <div class="col-2 text-left title"><slot name="number"></slot></div>
                <div class="col">
                    <div class="list-title"><slot name="title"></slot></div>
                    <div class="q-py-sm"></div>
                    <div class="under-title"><slot name="description"></slot></div>
                </div>
            </v-card-text>
        </v-card>
    </v-container>
</template>

<style  scoped>
.my-card{
  width: 100%;
  min-width:300px;
  background-color: #1E1E1E;
  border: 1px solid white;
}

  .title{
    font-family: 'Kanit';
    font-style: normal;
    font-weight: 400;
    font-size: 45px;
    line-height: 55px;
    text-transform: uppercase;
  }

.under-title{
    font-family: 'Kanit';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
}

.list-title{
    font-family: 'Kanit';
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 24px;
}
</style>