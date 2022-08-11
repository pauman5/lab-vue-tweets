<template>
  <p className="message" >
        {{message}}
      </p>
</template>

<script>
export default {
    name: "Message",
    components: {},
    props: {
        message: String,
    },
}
</script>

<style>

</style>