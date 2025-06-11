<template>
    <div class="app">
        <div class="content">
            <AppInfo/>
            <div class="search-panel style-01">
                <SearchPanel/>
                <AppFilter/>
            </div>
            <div class="move-list style-01">
                <MoveList/>
                <MoveAddForm/>
            </div>
        </div>
    </div>
</template>

<script>
import AppInfo from '@/components/app-info/AppInfo.vue'
import SearchPanel from '@/components/search-panel/SearchPanel.vue'
import AppFilter from '../app-filter/AppFilter.vue';
import MoveList from '../move-list/MoveList.vue';
import MoveAddForm from '../move-add-form/MoveAddForm.vue';

    export default{
        components:{
            AppInfo,
            SearchPanel,
            AppFilter,
            MoveList,
            MoveAddForm
        }
    }
</script>

<style>
    .app{
        height: 100vh;
        color: #000;
    }
    .content{
        width: 1000px;
        height: 700px;
        background-color: #fff;
        margin: 0 auto;
        padding: 5rem 0;
        /* border: 1px solid black; */
    }
    .style-01{
        margin-top: 2rem;
        padding: 1.5rem;
        background-color: #fcfaf5;
        border-radius: 4px;
        box-shadow: 15px 15px 15px rgba(0, 0, 0, .1);
    }
</style>