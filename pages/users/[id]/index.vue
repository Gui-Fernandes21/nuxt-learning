<template>
  <h1>this is the user with id: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  validate(data) {
    console.log('sum2');
    return console.log(data);
  },
}
</script>