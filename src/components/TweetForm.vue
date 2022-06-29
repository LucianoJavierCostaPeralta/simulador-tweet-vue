<template>
<div class="container tweet-form mt-4"
    :class="{open : showForm}">
    <form class="mb-5">
        <input class="form-control mb-2"
        :placeholder="placeholder.input" />

        <textarea class="form-control mb-2" rows="3"
        :placeholder="placeholder.textArea"></textarea>

        <button class="btn btn-primary w-100" type="button">
            {{ buttonText.enviar }}
        </button>
    </form>
</div>
</template>

<script>
export default {
    props: {
        showForm : Boolean
    },

    data() {
        return {
            buttonText : {
                enviar   : 'Enviar Tweet'
            },

            placeholder: {
                input    : 'Tu nombre',
                textArea : 'Escribe un tweet'
            }
        }
    }
}
</script>

<style lang="scss" scoped>
    .tweet-form {
        height: 0;
        overflow: hidden;

        &.open {
            height: auto;
        }
    }


</style>
