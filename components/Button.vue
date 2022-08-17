<template>
    <div>
        
        <b-button pill variant="outline-secondary" class="btn-sm px-3">{{btnText}}</b-button>
    </div>  
</template>

<script>
export default{
    name: 'Button',
    props: {
        btnText:String,
    }
}
</script>


