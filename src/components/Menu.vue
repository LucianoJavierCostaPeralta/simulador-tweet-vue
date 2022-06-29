<template>
    <nav class="navbar navbar-dark bg-dark">
        <div class="container">
            <span class="navbar-brand">
            {{ titleMenu }}
            </span>

            <button class="btn px-4"
                    :class="{'btn-success' : !showForm , 'btn-danger' : showForm}"
                    @click="openCloseForm" >
                    {{
                        !showForm ? this.titleButton.new : this.titleButton.close
                    }}
            </button>
        </div>
    </nav>
</template>

<script>
export default {
    props: {
        openCloseForm : Function,
        showForm      : Boolean
    },

    data() {
        return {
            titleMenu  : 'Simulador de tweets',
            titleButton: {
                new    : 'Nuevo Tweet',
                close  : 'Cerrar Tweet'
            }
        }
    }
}
</script>

<style>

</style>
