<template>
    <div>
        <h3>{{ title }}</h3>
        <MyInput @addItem='addItem' />
        <ol>
            <listItem 
                v-for='item in items'
                :item='item'
                :key='item.id'
            />
        </ol>
    </div>
</template>

<script>
import listItem from './listItem';
import MyInput from './input';
export default {
    name: 'list',
    props: ['title'],
    data: () => ({
        items: [],
    }),
    methods: {
        addItem (value) {
            this.items.push({ id: this.items.length+1, text: value });
        },
    },
    components: {
        listItem,
        MyInput,
    }
}
</script>