<template>
      <img :src="urlImage" className="profile" alt="profile"/>
</template>

<script>
export default {
    props:{
        urlImage:{
            type:String
        }
    }
}
</script>

<style>

</style>