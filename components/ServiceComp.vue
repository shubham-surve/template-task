<template>
    <div>
        
        <div class="p-5" v-html="img"></div>
        <h4>{{title}}</h4>
        <p>{{para}}</p>
    </div>
</template>

<script>
export default{
    name: 'ServiceComp',
    props: {
        title:String,
        para:String,
        img:String,
    }
}
</script>
