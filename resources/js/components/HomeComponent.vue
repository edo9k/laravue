<template>
  <div class="row justify-content-center">
    <div class="col-md-8">
      <div class="card card-default">
        <div class="card-header">Home Component</div>

        <div class="card-body">
          I'm a Home Component instance.
        </div>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    mounted() {
      console.log('Component mounted.')
    }
  }
</script>
