<template>
    <div class="app font-monospace">
        <div class="content">
            <AppInfo />
            <div class="search-panel">
                <SearchPanelVue />
                <AppFilterVue />
            </div>
            <MovieListVue />
            <MovieAddFormVue/>
        </div>
        
    </div>
</template>

<script>    
import AppFilterVue from '../app-filter/AppFilter.vue';
import AppInfo from '../app-info/AppInfo.vue';
import MovieAddFormVue from '../movie-add-form/MovieAddForm.vue';
import MovieListVue from '../movie-list/MovieList.vue';
import SearchPanelVue from '../search-panel/SearchPanel.vue';

export default{
    components:{
        AppInfo,
        SearchPanelVue,
        AppFilterVue,
        MovieAddFormVue,
        MovieListVue,
    }
}
</script>
<style>
    .app{
        height: 100vh;
        color:#000,
    }

    .content{
        width: 1000px;
        min-height: 700px;
        background-color: #fff;
        margin: 0 auto;
        padding: 5rem 0;
    }

    .search-panel{
        margin-top: 2rem;
        padding: 1.5rem;
        background-color: #fcfaf5;
        border-radius: 4px;
        box-shadow: 15px 15px 15px rgba(0, 0, 0,0.15);
    }
</style>