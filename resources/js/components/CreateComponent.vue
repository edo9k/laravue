<template>
  <div>
    <h1>New Post</h1>
    <form @submit.prevent="addPost">
      <div class="row">
        <div class="cold-md-6">
          <div class="form-group">
            <label>Post Title:</label>
            <input type="text" class="form-control" v-model="post.title"> 
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-6">
          <div class="form-group">
            <label>Post Body:</label>
            <textarea class="form-control" v-model="post.body" row="5"></textarea>
          </div>
        </div>
      </div>
      <div class="form-group">
        <button class="btn btn-primary">Create</button>
      </div>
    </form>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        post: {}
      }
    },
    methods: {
      addPost() {
        console.log(this.post)
      }
    }

  }
</script>
