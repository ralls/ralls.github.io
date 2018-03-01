<template>
  <div id="app" class="container">
    <div class="row align-items-center justify-content-center">
      <div class="col-auto">
        <div class="card">
          <div class="card-body text-center" itemscope itemtype="http://scema.org/Person">
            <h1 itemprop="name">Lee Ralls</h1>
            <h2>
              <span itemprop="jobTitle">Frontend Developer</span>
              <section itemprop="address" itemscope itemtype="http://scema.org/PostalAddress">
                <span itemprop="addressLocality">Eugene</span>, <span itemprop="addressregion">Oregon</span>
              </section>
            </h2>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
};
</script>

<style lang="scss">
@import "./styles/app.scss";
body, html {
  height: 100%;
}
body {
  background-color: $gray-100;
}
.container,
.row {
  height: 100%;
}

.card {
  border: none;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);

  &:hover {
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
  }
}
</style>
