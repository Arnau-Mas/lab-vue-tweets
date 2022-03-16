<template>
    <span className="user">
        <span className="name">{{userName}}</span>
        <span className="handle">@{{userHandle}}</span>
    </span>
</template>

<script>
export default {
    props:{
        userName:{
            type:String
        },
        userHandle:{
            type:String
        }
    }
}
</script>

<style>

</style>