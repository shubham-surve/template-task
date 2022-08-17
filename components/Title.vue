<template>
    <div>
        <h1 class="pt-5">{{mainTitle}}</h1>
        <hr class="hr1">
        <p>{{subTitle1}} <br>{{subTitle2}} </p>
    </div>
</template>

<script>

export default{
    name: 'Title',
    props: {
        mainTitle:String,
        subTitle1:String,
        subTitle2:String,
    }
}
</script>