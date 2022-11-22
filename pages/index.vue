<template>
  <section class="pt-4 pb-4">
    <div class="container">
      <h3 class="fw-bolder">Courses</h3>

      <div class="row">

        <h3 v-if="loading">Loading..</h3>

        <CourseCard v-else v-for="course in courses" :key="course.id" :course="course"/>

      </div>
    </div>
  </section>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      loading: true,
      courses: []
    }
  },
  mounted(){
    this.getCourses()
  },
  methods:{
    async getCourses(){
      const res = await this.$axios.get('/courses');

      if(!res.data.error){
        this.courses = res.data.courses;
        this.loading = false;
      }

    }
  }

}
</script>

<style scoped>

</style>
