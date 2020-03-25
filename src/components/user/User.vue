<template>
    <div>
        <h1>The User Page</h1>
        <hr>
        <button @click.prevent="navigateToHome" class="btn btn-default">
            GO To Home
        </button>
        <hr>
        <router-view></router-view>
    </div>
</template>

<script>
export default {
    methods:{
        navigateToHome(){
            this.$router.push('/');
        }
    }
}
</script>