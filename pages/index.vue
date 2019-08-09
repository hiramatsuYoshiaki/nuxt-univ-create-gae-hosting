<template>
  <div class="container">
    <div class="content con-wraper">
      <div class="con-hed-logo">
        <logo />
      </div>
      <div class="con-hed-title">
        <h2 class="title">
          h-works
        </h2>
        <div class="subtitle">
          <h5>Nuxt.js</h5>
          <h5>App Engine</h5>
          <h5>Google Cloud Platform</h5>
        </div>
        <div class="subscription">
          <p>Nuxt Project</p>
          <p>create-nuxt-app v2.8.0</p>
          <p>? Choose custom server framework None</p>
          <p>? Choose rendering mode Universal (SSR)</p>
        </div>
      </div>
    </div>
    <div class="link-content link-wraper">
      <div class="links">
        <a
          href="https://nuxt-univ-gae-app.appspot.com/"
          target="_blank"
          class="button--green"
        >
          Demo App (Google App Engine )
        </a>
      </div>
      <div class="links">
        <a
          href="https://github.com/hiramatsuYoshiaki/nuxt-univ-create-gae-hosting"
          target="_blank"
          class="button--grey"
        >
          nuxt-univ-create-gae-hosting (GitHub )
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  layout: 'topPage',
  components: {
    Logo
  }
}
</script>

<style scoped lang="scss">
%center {
  display: flex;
  justify-content: center;
  align-items: center;
}
%left {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
%right {
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
//content base-----------------------
.container {
  margin-top: $header-height;
  width: 100vw;
  min-height: 100vh;
  @extend %center;
  flex-direction: column;
  margin: 0;
  padding: 0;
  background: linear-gradient(#0452c7, #9dacf0);
}
.content {
  width: 100%;
  display: block;
  display: flex;
  flex-direction: column;
  @media (min-width: 992px) {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: flex-start;
  }
}
.link-content {
  width: 100%;
  display: block;
  display: flex;
  flex-direction: column;
  @extend %center;
  @media (min-width: 992px) {
    flex-direction: row;
    // justify-content: flex-start;
    // align-items: flex-start;
  }
}
// wraper-----------------------------
.con-wraper {
  padding: 8rem 2rem 0rem 2rem;
  @media (min-width: 992px) {
    padding: 10rem 5rem 0rem 5rem;
  }
}
.link-wraper {
  padding: 1rem 2rem 0rem 2rem;
  @media (min-width: 992px) {
    padding: 1rem 5rem 0rem 5rem;
  }
}

.con-hed-logo {
  @extend %center;
  width: 100%;
  @media (min-width: 992px) {
    width: 40%;
  }
}
.con-hed-title {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  @media (min-width: 992px) {
    justify-content: flex-start;
    align-items: flex-start;
  }
  h2 {
    font-size: 3rem;
    font-weight: 700;
    line-height: 3.5rem;
  }
  h5 {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7rem;
  }
  p {
    font-size: 1rem;
    font-weight: 500;
    line-height: 1.5rem;
  }

  @media (min-width: 992px) {
    width: 70%;
    h2 {
      font-size: 8rem;
      font-weight: 700;
      line-height: 8.5rem;
    }
    h5 {
      font-size: 3rem;
      font-weight: 400;
      line-height: 3.2rem;
    }
    p {
      font-size: 2rem;
      font-weight: 500;
      line-height: 2.2rem;
    }
  }
}

.links {
  @extend %center;
  margin: 2rem;
  width: 100%;
}
.links a {
  display: inline-block;
  margin: 0 2rem;
  cursor: pointer;
  // word-wrap: break-word;
  font-size: 1rem;
  font-weight: 500;
  line-height: 1.5rem;
  @media (min-width: 992px) {
    font-size: 2rem;
    font-weight: 500;
    line-height: 2.2rem;
  }
}

.title {
  margin: 2rem 0 1rem 0;
  color: #fff;
}
.subtitle {
  margin: 0rem 0 4rem 0;
  color: #fff;
  @extend %center;
  flex-direction: column;
}
.subscription {
  margin-bottom: 2rem;
  color: rgb(25, 25, 25);
}
// .content-footer {
//   width: 100vw;
//   display: flex;
//   justify-content: center;
//   align-items: center;
//   flex-direction: column;
//   margin-bottom: -5rem;
// }

// .done {
//   text-decoration: line-through;
// }
</style>
