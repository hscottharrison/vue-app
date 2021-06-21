<template>
    <div>
        <input v-model='text' />
        <button v-on:click='submit'>Submit</button>
    </div>
</template>

<script>
export default {
    name: 'myinput',
    data: () => ({
        text: '',
    }),
    methods: {
        submit() {
            console.log(this.text)
            this.$emit('addItem', this.text);
            this.text = '';
        }
    }
}
</script>