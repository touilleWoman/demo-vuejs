<template>
    <div v-if="info !== null">
        <p>{{ info.user.email }}</p>
        <p>{{ info.user.username }}</p>
        <p>{{ info.user.last_login }}</p>
    </div>
</template>

<script>
export default {
    name: "user",
    props : ["info"]
}
</script>