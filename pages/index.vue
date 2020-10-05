<template>
  <div class="bg-dark">
    <div class="container-fluid bg-dark" style="height: 100vh">
      <div class="container py-5 bg-dark">
        <div class="mt-5">
          <h1 class="main-title mb-3">
            <span class="marker marker-teal px-md-4 py-md-3 py-2 px-2">
              #ManOfTheMatch
            </span>
          </h1>
          <p class="text-monospace">
            <span class="marker marker-teal marker-tag">
              <i> Developed by Team Blklight</i>
            </span>
          </p>

          <h2 class="exo-font mt-5">
            <span class="marker marker-teal marker-tag">
              <strong> Outubro em andamento...</strong>
            </span>
          </h2>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style lang="scss">
.main-title {
  font-weight: 900;
  font-style: italic;
  font-size: 88px;
  font-family: 'Exo', sans-serif;
}

@media screen and (max-width: 992px) {
  .main-title {
    font-size: 64px;
  }
}

@media screen and (max-width: 768px) {
  .main-title {
    font-size: 56px;
  }
}

@media screen and (max-width: 576px) {
  .main-title {
    font-size: 2.5rem;
  }
}

.exo-font {
  font-family: 'Exo', 'Roboto Mono', 'Fira Code', monospace !important;
}

.marker-teal {
  background-color: #00ff87;
}
</style>
