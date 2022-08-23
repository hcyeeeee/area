<template>
    <div class="layout_footer">
        <div class="layout_grid">
            <p>{{ title }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            title: `Copyright © 2022 民視新聞網路部 社群中心`,
        }
    },
}
</script>

<style scoped>
.layout_footer {
    background-color: #efefef;
    box-shadow: rgba(0, 0, 0, ) 2.4px 2.4px 3.2rem 3rem;

}

p {
    font-size: 1.2rem;
    color: #333;
    font-weight: 500;
}

.layout_grid {
    grid-template-columns: 1fr;
    padding: 1.5rem;

}
</style>
