<template>
    <li>
        {{ breadcrumb.title}} / 
    </li>
</template>

<script>

export default {
    props: {
        breadcrumb: {
            type: Object,
            required: true
        }
    }
}
</script>
