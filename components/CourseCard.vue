<template>
  <div class="col-lg-4 col-md-6 col-12 mt-4">
    <div class="card">
      <img :src="course.thumbnail" class="card-img-top" :alt="course.name" />
      <i class="bi bi-bookmark card-bookmark"></i>
      <div class="card-body pb-0">
        <div class="tutor-course-ratings">
          <div class="tutor-ratings">
            <div class="tutor-ratings">
              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
            </div>
            <div class="tutor-ratings-average">5.0</div>
            <div class="tutor-ratings-count">(7)</div>
          </div>
        </div>
        <h5 class="card-title mt-3 mb-3">{{ course.name }}</h5>
        <div class="tutor-meta mb-3">
          <div class="d-inline">
            <span class="tutor-meta-icon tutor-icon-user-line" area-hidden="true"><i class="bi bi-person"></i></span>
            <span class="tutor-meta-value">815</span>
          </div>

          <div class="d-inline p-2">
            <span class="tutor-meta-icon tutor-icon-clock-line ml-3" area-hidden="true"><i
                class="bi bi-clock"></i></span>
            <span class="tutor-meta-value"> 2h 23m</span>
          </div>
        </div>

        <div class="tutor-meta">
          <div class="d-inline">
            <div class="tutor-avatar d-inline">
              <img src="https://ui-avatars.com/api/?background=0D8ABC&color=fff&name=Gazi+Moshiul" alt="" srcset="" />
            </div>
          </div>

          <div class="d-inline">
            By
            <a href="#">Polash Mahmud</a>

            In
            <a href="#">পলাশ মাহমুদ</a>
          </div>
        </div>
      </div>
      <hr class="border-1 mb-2" />
      <nuxt-link :to="'course/' + course.slug" class="btn-tutor">View Details</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props:{
    course: {}
  }
}
</script>

<style>

</style>
