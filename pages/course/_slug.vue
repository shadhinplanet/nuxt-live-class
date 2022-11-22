<template>
  <section class="pt-5 pb-4">
   <div v-if="course" class="">
    <div class="container">
      <div class="row">

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
        <div class="single-page-tutor-meta mb-3">
          <div class="d-inline">
            <span class="tutor-meta-icon tutor-icon-user-line" area-hidden="true">Cagetories:</span>
            <span class="tutor-meta-value">Programming</span>
          </div>

          <div class="d-inline p-2 wishlist">
            <span class="tutor-meta-icon tutor-icon-clock-line ml-3" area-hidden="true"><i
                class="bi bi-bookmark single-card-bookmark"></i></span>
            <span class="tutor-meta-value"> Wishlist</span>
          </div>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row">

        <!-- single page left side content start -->
        <div class="col-lg-8 left-tutor-col">
          <div class="row">
            <img :src="course.thumbnail" class="card-img-top" :alt="course.name" />
          </div>
          <div class="row single-tutor-info">
            <ul class="nav nav-pills mb-3" id="pills-tab" role="tablist">
              <li class="nav-item" role="presentation">

                <button class="nav-link active" id="pills-home-tab" data-bs-toggle="pill" data-bs-target="#pills-home"
                  type="button" role="tab" aria-controls="pills-home" aria-selected="true">
                  Course Info
                </button>
              </li>
              <li class="nav-item" role="presentation">
                <button class="nav-link" id="pills-profile-tab" data-bs-toggle="pill" data-bs-target="#pills-profile"
                  type="button" role="tab" aria-controls="pills-profile" aria-selected="false">
                  Reviews
                </button>
              </li>
            </ul>
            <div class="tab-content" id="pills-tabContent">
              <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">
                <h4 class="about-course-heading">About Course</h4>
                <div class="course-info" v-html="course.description">

                </div>
                <div class="tutor-course-detail">
                  <h4>What Will You Learn?</h4>
                  <ul class="tutor-course-detail-ul">

                    <li>
                      <span class="tutor-course-detail-bullet"></span>
                      <span>এই কোর্সটি করে সুপার স্পিডের একটি ইকমার্স ওয়েবসাইট তৈরি করতে পারবেন।</span>
                    </li>
                    <li>
                      <span class="tutor-course-detail-bullet"></span>
                      <span>এই কোর্সটি করে সুপার স্পিডের একটি ইকমার্স ওয়েবসাইট তৈরি করতে পারবেন।</span>
                    </li>
                    <li>
                      <span class="tutor-course-detail-bullet"></span>
                      <span>এই কোর্সটি করে সুপার স্পিডের একটি ইকমার্স ওয়েবসাইট তৈরি করতে পারবেন।</span>
                    </li>
                    <li>
                      <span class="tutor-course-detail-bullet"></span>
                      <span>এই কোর্সটি করে সুপার স্পিডের একটি ইকমার্স ওয়েবসাইট তৈরি করতে পারবেন।</span>
                    </li>
                  </ul>
                </div>
                <div class="couse-content">
                  <h4>Course Content</h4>
                  <div class="accordion" id="accordionExample">
                    <div class="accordion-item">
                      <h2 class="accordion-header" id="headingOne">
                        <button class="accordion-button" type="button" data-bs-toggle="collapse"
                          data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                          <h5>Accordion Item #1</h5>
                        </button>
                      </h2>
                      <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne"
                        data-bs-parent="#accordionExample">
                        <div class="accordion-body">
                          <ul class="tutor-class-content-list">
                            <li class="tutor-course-content-list-item">
                              <div class="tutor-d-flex tutor-align-center">
                                <span
                                  class="tutor-course-content-list-item-icon tutor-icon-brand-youtube-bold tutor-mr-12"><i
                                    class="bi bi-youtube"></i></span>
                                <p class="tutor-course-content-list-item-title">
                                  1. How to use Vue (using the CDN)
                                </p>
                              </div>

                              <div>
                                <span class="tutor-course-content-list-item-duration tutor-fs-7 tutor-color-muted">
                                  09:18</span>
                                <span
                                  class="tutor-course-content-list-item-status tutor-icon-lock-line tutor-color-muted tutor-ml-20"
                                  area-hidden="true"><i class="bi bi-lock"></i></span>
                              </div>
                            </li>
                            <li class="tutor-course-content-list-item">
                              <div class="tutor-d-flex tutor-align-center">
                                <span
                                  class="tutor-course-content-list-item-icon tutor-icon-brand-youtube-bold tutor-mr-12"><i
                                    class="bi bi-youtube"></i></span>
                                <p class="tutor-course-content-list-item-title">
                                  1. How to use Vue (using the CDN)
                                </p>
                              </div>

                              <div>
                                <span class="tutor-course-content-list-item-duration tutor-fs-7 tutor-color-muted">
                                  09:18</span>
                                <span
                                  class="tutor-course-content-list-item-status tutor-icon-lock-line tutor-color-muted tutor-ml-20"
                                  area-hidden="true"><i class="bi bi-lock"></i></span>
                              </div>
                            </li>
                            <li class="tutor-course-content-list-item">
                              <div class="tutor-d-flex tutor-align-center">
                                <span
                                  class="tutor-course-content-list-item-icon tutor-icon-brand-youtube-bold tutor-mr-12"><i
                                    class="bi bi-youtube"></i></span>
                                <p class="tutor-course-content-list-item-title">
                                  1. How to use Vue (using the CDN)
                                </p>
                              </div>

                              <div>
                                <span class="tutor-course-content-list-item-duration tutor-fs-7 tutor-color-muted">
                                  09:18</span>
                                <span
                                  class="tutor-course-content-list-item-status tutor-icon-lock-line tutor-color-muted tutor-ml-20"
                                  area-hidden="true"><i class="bi bi-lock"></i></span>
                              </div>
                            </li>
                          </ul>
                        </div>
                      </div>
                    </div>


                  </div>
                </div>
              </div>
              <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">
                <h5>Student Ratings & Reviews</h5>

                <div class="students-review-on-tutor card">
                  <div class="tutor-review card-body">
                    <div class="tutor-review-left">
                      <div class="tutor-review-summary-average-rating">5.0</div>
                      <div>
                        <div class="tutor-d-inline-block">
                          <div class="tutor-ratings tutor-ratings-lg">
                            <div class="tutor-ratings-stars">
                              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                              <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="tutor-fs-6 tutor-color-secondary tutor-mt-12 tutor-total-rating-count">Total: 23
                        Ratings</div>
                    </div>
                    <div class="tutor-review-right">

                      <div class="tutor-review-summary-ratings">
                        <div class="row tutor-align-center tutor-review-summary-rating">
                          <div class="col-2 text-end">
                            <div class="tutor-ratings">
                              <div class="tutor-ratings-stars">
                                <span class="tutor-icon-star-line" area-hidden="true">
                                  <i class="bi bi-star"></i>
                                </span>
                              </div>
                              <div class="tutor-ratings-average">
                                5
                              </div>
                            </div>
                          </div>

                          <div class="col-7">
                            <div class="progress">
                              <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar"
                                aria-valuenow="75" aria-valuemin="0" aria-valuemax="100" style="width: 70%"></div>
                            </div>
                          </div>

                          <div class="col-3">
                            <span class="tutor-fs-6 tutor-color-secondary tutor-individual-star-rating">1 Rating</span>
                          </div>
                        </div>
                      </div>


                    </div>
                  </div>

                  <hr class="border-1 mb-2" />
                  <!-- </div>

                <div class="card"> -->
                  <div class="row card-body single-tutor-meta-info">
                    <div class="col-lg-4 tutor-meta-info">
                      <div class="tutor-avatar">
                        <img src="https://ui-avatars.com/api/?background=0D8ABC&color=fff&name=Gazi+Moshiul" alt=""
                          srcset="" />
                      </div>
                      <a href="#">Polash Mahmud</a>
                      <div class="tutor-comments-date">5th Sep, 2022</div>
                    </div>
                    <div class="col-lg-8 tutor-meta-user-comments">
                      <div class="tutor-meta-ratings-star">
                        <div class="tutor-ratings tutor-ratings-lg">
                          <div class="tutor-ratings-stars">
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                          </div>
                        </div>
                      </div>
                      <div class="tutor-meta-comments">Lorem ipsum dolor sit amet.</div>
                    </div>
                  </div>


                  <div class="row card-body single-tutor-meta-info">
                    <div class="col-lg-4 tutor-meta-info">
                      <div class="tutor-avatar">
                        <img src="https://ui-avatars.com/api/?background=0D8ABC&color=fff&name=Gazi+Moshiul" alt=""
                          srcset="" />
                      </div>
                      <a href="#">Polash Mahmud</a>
                      <div class="tutor-comments-date">5th Sep, 2022</div>
                    </div>
                    <div class="col-lg-8 tutor-meta-user-comments">
                      <div class="tutor-meta-ratings-star">
                        <div class="tutor-ratings tutor-ratings-lg">
                          <div class="tutor-ratings-stars">
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                            <span class="tutor-icon-star-bold"><i class="bi bi-star"></i></span>
                          </div>
                        </div>
                      </div>
                      <div class="tutor-meta-comments">Lorem ipsum dolor sit amet.</div>
                    </div>
                  </div>


                </div>

              </div>
            </div>
          </div>
        </div>


        <!-- single page right sidebar start -->
        <div class="col-lg-4 right-tutor-col">
          <div class="card">
            <div class="card-body single-page-card-body pb-0">
              <h3 class="card-title mt-3 mb-3">Free</h3>
            </div>
            <a href="single-page.html" class="btn-tutor">Enroll Course</a>
            <div class="tutor-meta">
              <div class="tutor-avatar text-center">
                Free access this course
              </div>
            </div>
            <hr class="border-1 mb-2" />

            <div class="single-tutor-meta mb-3">
              <ul class="single-tutor-ul">
                <li>
                  <span><i class="bi bi-water"></i></span>Intermediate
                </li>
                <li>
                  <span><i class="bi bi-mortarboard"></i></span>1719 Total
                  Enrolled
                </li>
                <li>
                  <span><i class="bi bi-arrow-repeat"></i></span>August 24,
                  2022 Last Updated
                </li>
              </ul>
            </div>
          </div>

          <div class="card mt-4">
            <div class="card-body single-page-card-body pb-0">
              <span>A course by</span>
              <div class="single-tutor-user-meta">
                <div class="d-inline">
                  <div class="tutor-avatar d-inline">
                    <img src="https://ui-avatars.com/api/?background=0D8ABC&color=fff&name=Shadhin+Ahmed" alt=""
                      srcset="" />
                    By
                    <a href="#">Polash Mahmud</a>
                  </div>
                </div>
              </div>
            </div>
            <hr class="border-1 mb-2" />
            <div class="single-tutor-meta-side-info card-body">
              <h4>Material Includes</h4>
              <ul class="single-tutor-meta-side-info-ul">
                <li>
                  Github Code
                </li>
                <li>
                  Design File
                </li>
                <li>
                  Discord help
                </li>
              </ul>
            </div>

            <div class="single-tutor-requirements card-body">
              <h4 class="">Requirements</h4>
              <div class="single-tutor-req-desc">
                <span class="single-tutor-require-bullet-icon"></span>
                <span class="single-tutor-require-desc">এই কোর্সটি করার জন্য আপনাকে অবশ্যই বেসিক এইচটিএমএল, সিএসএস,
                  জেকুয়েরি, পিএইচপি জানা থাকতে হবে। এগুলা না জানা থাকলে শিখুন.নেট থেকে কোর্সগুলা করে নিতে পারেন।</span>
              </div>

            </div>

            <div class="single-tutor-requirements card-body">
              <h4 class="">Audience</h4>
              <div class="single-tutor-req-desc">
                <span class="single-tutor-require-bullet-icon"></span>
                <span class="single-tutor-require-desc">যারা বেসিক এইচটিএমএল, সিএসএস, জাভাস্ক্রীপ্ট এবং পিএইচপি শিখেছেন,
                  ইকমার্স ওয়েবসাইট তৈরি করতে চান তাদের জন্যই এই কোর্স।</span>
              </div>

            </div>

          </div>

        </div>
      </div>
    </div>
   </div>
   <div v-else class="">
    <h3>Loading..</h3>
   </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      course: {},
      loading:true
    }
  },
  created(){
    this.getCourseData()
  },
  methods:{
    async getCourseData(){
      const res = await this.$axios.get(this.$route.path).then((res)=>{
      this.course = res.data.course[0];
      this.loading = false;
    });
    }
  }
}
</script>

<style>

</style>
