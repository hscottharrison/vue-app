<template>
    <li>{{ item.text }}</li>
</template>

<script>
export default {
    name: 'listitem',    
    props: ['item']
}
</script>