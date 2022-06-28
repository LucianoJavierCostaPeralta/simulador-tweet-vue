<template>
    <nav class="navbar navbar-dark bg-dark">
        <div class="container">
            <span class="navbar-brand">
            {{ titleMenu }}
            </span>

            <button class="btn btn-success px-4">
                {{ titleButton }}
            </button>
        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            titleMenu  : 'Simulador de tweets',
            titleButton: 'Nuevo Tweet'
        }
    }
}
</script>

<style>

</style>
