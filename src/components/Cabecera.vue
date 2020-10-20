<template>
    <div id="nav-bar">
        <nav class="navbar fixed-top navbar-expand-lg navbar-dark bg-dark">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse form-inline my-2 my-lg-0" id="navbarTogglerDemo01">
            <a class="navbar-brand" href="#">A.B.M.O.D.E.L.</a>
            <ul class="navbar-nav ml-auto">
            <li class="nav-item active">
                <a class="nav-link" href="#">Create</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Read</a>
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

<style lang="sass" scoped>

</style>