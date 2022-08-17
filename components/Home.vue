<template>
    <div>   
        <div class="container-fluid py-5 bg-light">
            
            <h1 class="pt-5 text-center">{{textHomeTitle}}</h1>
            <p class="py-2 text-center" >{{parText}}</p>
            <Button class="p-3 pb-4 text-center" btnText="Download " />
            
            </div>
        </div> 
</template>

<script>
export default{
    name: 'Home',
    props: {
        textHomeTitle:String,
        parText:String,
    }
}
</script>
