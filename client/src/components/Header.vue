<template>
    <div className="header">
        <h1>{{ name }}</h1>
        <h2>{{ title }}</h2>
    </div>
</template>

<script>
export default {
    data() {
        return {
            name: "Tyler Miller",
            title: "software engineer"
        }
    },
    name: 'Header',
}
</script>

<style>
.header {
    background-color: #007cc7;
    color: #fff;
    padding: 3%;
}

.header h1 {
    font-size: 2rem;
    margin-bottom: 1%;
}
</style>