<template>
    <div id="nav-bar">
        <nav class="navbar fixed-top navbar-expand-lg navbar-dark bg-dark">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse form-inline my-2 my-lg-0" id="navbarTogglerDemo01">
            <router-link class="navbar-brand" active-class="active" to="/">
                <img class="mr-2" width="40" height="40" src="@/assets/bored-shrek-meme.png" alt="">
                A.B.M.O.D.E.L.
            </router-link>
            <ul class="navbar-nav ml-auto">
            <li class="nav-item active">
                <router-link class="nav-link" active-class="active" to="/">Create</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" to="/read">Read</router-link>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Update</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Delete</a>
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
    }
    
</style>