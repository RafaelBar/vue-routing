<template>
    <div class="d">
        <h3>Some User Details</h3>
        <p class="">User Loaded has ID: {{$route.params.id}}</p>
        <router-link 
            tag="button" 
            :to="{ name: 'userEdit', params: {id: $route.params.id}, query:{locale:'en', q:'100'} }"
            class="btn btn-primary">Edit The User</router-link>
    </div>
</template>