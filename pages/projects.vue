<template>
  <div>
    <div class="projects">
      <h1 class="projects-title">
        what i've done
      </h1>
      <div
        v-for="{ name, imgPath, description, url, gitUrl, tags } in projects"
        :key="name"
        class="projects-box"
      >
        <div class="projects-box-imgwrapper">
          <img v-if="imgPath" class="projects-box-img" :src="require('~/assets/projectImg/' + imgPath)" />
        </div>
        <div class="projects-box-info">
          <div class="projects-box-title">
            <a v-if="url" :href="url" target="_blank">
              <h3>{{ name }}</h3>
            </a>
            <h3 v-else>{{ name }}</h3>
          </div>
          <div class="projects-box-sub">
            <div>
              <div v-for="tag in tags" :key="tag" class="projects-box-tag">
                {{ tag }}
              </div>
            </div>
            <a :href="gitUrl" target="_blank">
              <img class="projects-box-git" src="~assets/icons/git.svg" />
            </a>
          </div>
          <p class="projects-box-description" v-html="description" />
        </div>
      </div>
    </div>
    <div class="index-bottom" />
  </div>
</template>

<style>
  .projects {
    margin: 100px 150px 0;
  }

  .projects-title {
    margin: 0 0 60px 0;
    font-family: var(--font-ovo);
    font-size: 52px;
  }

  .projects-box {
    display: flex;
    margin-bottom: 64px;
  }

  .projects-box-imgwrapper {
    max-width: 450px;
    margin-right: 64px;
    display: flex;
  }

  .projects-box-img {
    height: auto;
    width: 100%;
    margin: auto 0;
  }

  .projects-box:nth-of-type(3n+1) .projects-box-img {
    box-shadow: 16px 16px 0px 0px rgba(245,203,203,0.6);
  }

  .projects-box:nth-of-type(3n+2) .projects-box-img {
    box-shadow: 16px 16px 0px 0px rgba(40,50,70,0.6);
  }

  .projects-box:nth-of-type(3n) .projects-box-img {
    box-shadow: 16px 16px 0px 0px rgba(184,94,94,0.6);
  }

  .projects-box-info {
    width: 100%;
  }

  .projects-box-title {
    background: var(--main-pink);
    height: 40px;
    width: 0;
    transition: width 275ms ease;
    border-radius: 4px;
    position: relative;
  }

  .projects-box-title:hover {
    width: 100%;
  }

  .projects-box-title h3 {
    margin: 0 8px;
    position: absolute;
    top: 8px;
    width: max-content;
    cursor: default;
  }

  .projects-box-title a h3 {
    text-decoration: underline;
    cursor: pointer;
  }

  .projects-box-sub {
    display: flex;
    justify-content: space-between;
    margin: 8px 0 0 8px;
  }

  .projects-box-tag {
    display: inline-block;
    padding: 4px 8px;
    margin-right: 4px;
    background-color: var(--main-red);
    color: var(--main-neutral);
    border-radius: 8px;
  }

  .projects-box-git {
    width: 30px;
  }

  .projects-box-description {
    background-color: var(--main-neutral);
    margin: 8px 0 0 8px;
  }

  .index-bottom {
    height: 36px;
    width: 100%;
    background-color: var(--main-navy);
  }

  @media (max-width: 767px) {
    .projects {
      margin: 100px 16px 0;
    }

    .projects-title {
      margin-bottom: 36px;
      font-size: 36px;
    }

    .projects-box {
      display: block;
      margin-bottom: 24px;
    }

    .projects-box-imgwrapper {
      width: 100%;
    }

    .projects-box-img {
      margin: 0 20px 24px 0;
      max-width: calc(100% - 16px);
    }
  }
</style>

<script>
import projectData from '~/assets/projects.json'

export default {
  data: () => (
    {
      projects: projectData
    }
  )
}
</script>
