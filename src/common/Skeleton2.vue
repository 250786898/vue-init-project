<template>
  <div class="skeleton page">
    <!-- <div class="skeleton-nav"></div> -->
    <div class="skeleton-swiper"></div>
    <ul class="skeleton-tabs">
      <li v-for="i in 8" :key="i" class="skeleton-tabs-item"><span></span></li>
    </ul>
    <div class="skeleton-banner"></div>
    <div v-for="j in 6" :key="j" class="skeleton-productions"></div>
  </div>
</template>

<style>
.skeleton {
  position: relative;
  height: 100%;
  overflow: hidden;
  padding: 0.15rem;
  box-sizing: border-box;
  background: #fff;
}
.skeleton-nav {
  height: 0.5rem;
  background: #eee;
  margin-bottom: 0.15rem;
}
.skeleton-swiper {
  height:1.6rem;
  background: #eee;
  margin-bottom: 0.15rem;
}
.skeleton-tabs {
  list-style: none;
  padding: 0;
  margin: 0 -0.15rem;
  display: flex;
  flex-wrap: wrap;
}
.skeleton-tabs-item {
  width: 25%;
  height: 0.55rem;
  box-sizing: border-box;
  text-align: center;
  margin-bottom: 0.15rem;
}
.skeleton-tabs-item span {
  display: inline-block;
  width: 0.45rem;
  height: 0.45rem;
  border-radius: 0.45rem;
  background: #eee;
}
.skeleton-banner {
  height: 60px;
  background: #eee;
  margin-bottom: 0.15rem;
}
.skeleton-productions {
  height: 0.2rem;
  margin-bottom: 0.15rem;
  background: #eee;
}

.skeleton {
  padding: 0.1rem;
}

.skeleton .skeleton-head,
.skeleton .skeleton-title,
.skeleton .skeleton-content {
  background: rgb(194, 207, 214);
}

.skeleton-head {
  width: 100px;
  height: 1rem;
  float: left;
}

.skeleton-body {
  margin-left: 110px;
}

.skeleton-title {
  width: 5rem;
  height: 0.6rem;
  transform-origin: left;
  animation: skeleton-stretch .5s linear infinite alternate;
}

.skeleton-content {
  width: 2.6rem;
  height: 0.3rem;
  margin-top: 0.1rem;
  transform-origin: left;
  animation: skeleton-stretch .5s -.3s linear infinite alternate;
}

@keyframes skeleton-stretch {
  from {
    transform: scalex(1);
  }
  to {
    transform: scalex(.3);
  }
}
</style>
