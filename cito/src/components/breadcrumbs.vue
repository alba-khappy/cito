<template>
    <div class="header-breadcrumbs-wrapper">
        <ul class="header__breadcrumbs container">
            <breadcrumbsItem 
            v-for="breadcrumb of breadcrumbs"
            :breadcrumb="breadcrumb"
            :key="breadcrumb.id"/>
        </ul>
    </div>
</template>

<script>
import breadcrumbsItem from '@/components/breadcrumbs-item'

export default {
    props: ['breadcrumbs'],
    components: {
        breadcrumbsItem
    }
}
</script>


<style scoped>

.header-breadcrumbs-wrapper {
    background-color: #F7F7F7;
}

.header__breadcrumbs {
    list-style: none;
    display: flex;
    padding: 16px 0;
}

.container {
    margin: 0 auto;
    max-width: 1440px;
}

</style>