<template>
    <div class=" bg-info">
        

        <img class="img-fluid w-100" :src="image" alt="profile image">
        
        <h4 class="pt-2">{{name}}</h4>
        <p>{{role}}</p>
        <div class="pb-3 row d-flex justify-content-center">
            <i class="px-2 fa-brands fa-facebook"></i>
            <i class="px-2 fa-brands fa-twitter"></i>
            <i class="px-2 fa-brands fa-linkedin-in"></i>
        </div>

    </div>
</template>
<script>
export default {
    name:'TeamComp',
    props:{
        name:String,
        role:String,
        image:String,
    }
}
</script>