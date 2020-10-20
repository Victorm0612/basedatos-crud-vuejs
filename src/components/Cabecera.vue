<template>
    <div id="nav-bar">
        <nav class="navbar fixed-top navbar-expand-md navbar-dark bg-dark">
        <router-link class="navbar-brand" active-class="active" to="/">
                <img class="mr-2" width="40" height="40" src="@/assets/bored-shrek-meme.png" alt="">
                A.B.M.O.D.E.L.
        </router-link>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarResponsive">
            <ul class="navbar-nav ml-auto">
            <li class="nav-item">
                <router-link class="nav-link" to="/">Create</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" to="/read">Read</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" to="/update">Update</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" to="/delete">Delete</router-link>
            </li>            
            </ul>
        </div>
        </nav>
    </div>
</template>

<script>
    export default {
        name: 'Cabecera'
    }
</script>

<style scoped>
    #nav-bar{
        padding: 30px;
        font-size: 1.2rem;
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
    }
    
</style>