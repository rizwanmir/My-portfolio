<template>
  <div class="portfolio">
    <div>
      <h2>
        Published Websites and applications
      </h2>
    </div>
  <div>
  <b-card no-body class="overflow-hidden">
    <b-row 
      no-gutters
      v-for="project in projects" 
      :key="project.id"
    >
    <b-col md="6">
      <b-card-img 
        :src="project.image"  
        alt="Image" 
        class="rounded-0"
      >
      </b-card-img>
    </b-col>
    <b-col md="6">
      <b-card-body>
          <b-card-sub-title>
          {{project.category}}
        </b-card-sub-title>
        <b-card-title>
          {{project.title}}
        </b-card-title>
        <b-list-group horizontal>
          <b-list-group-item v-for="(list, index) in project.tech" :key="index">
            {{list}}
          </b-list-group-item>
        </b-list-group>
        <b-card-text>
          {{project.description}}
        </b-card-text>
        <div class="portfolio_btn_container">
          <a :href="project.websiteLink" target="blank" class="portfolio_btn">Show Website <span><font-awesome-icon :icon="['fas', 'angle-double-right']" /></span></a>
          <a :href="project.githubLink" target="blank" class="portfolio_btn">Show Github <span><font-awesome-icon :icon="['fas', 'angle-double-right']" /></span></a>
        </div>
      </b-card-body>
      </b-col>
    </b-row>
  </b-card>
</div>
</div>
</template>

<script>
export default {
  name: 'Portfolio',
  data () {
    return {
      projects: [
        {
          id: 1,
          image: require('@/assets/project.png'),
          category: 'Project',
          title: 'Website',
          tech: [
            "HTML5",
            "CSS3",
            "JavScript",
            "PHP"

          ],
          websiteLink: 'https://github.com/rizwanmir/My-portfolio',
          githubLink: 'https://github.com/rizwanmir/My-portfolio',
          description: 'I have developed this personal website to showcase my projects and will use a portfollio. I have used HTML, CSS/LESS and VueJS in this project.'
      
        },
        {
          id: 2,
          image: require('@/assets/php-project.png'),
          category: 'Project',
          title: 'Website',
           tech: [
            "HTML5",
            "CSS3",
            "JavScript",

          ],
          websiteLink: 'https://github.com/rizwanmir/My-portfolio',
          githubLink: 'https://github.com/rizwanmir/My-portfolio',
          description: 'I have developed this personal website to showcase my projects and will use a portfollio. I have used HTML, CSS/LESS and VueJS in this project.'

        },
        {
          id: 3,
          image: require('@/assets/project3.png'),
          category: 'Project',
          title: 'Website',
           tech: [
            "HTML5",
            "CSS3",
            "JavScript",
            "VueJS"

          ],
          websiteLink: 'https://github.com/rizwanmir/My-portfolio',
          githubLink: 'https://github.com/rizwanmir/My-portfolio',
          description: 'I have developed this personal website to showcase my projects and will use a portfollio. I have used HTML, CSS/LESS and VueJS in this project.'

        },
        {
          id: 3,
          image: require('@/assets/project4.png'),
          category: 'Project',
          title: 'Website',
           tech: [
            "HTML5",
            "CSS3",
            "JavScript",
            "VueJS"

          ],
          websiteLink: 'https://github.com/rizwanmir/My-portfolio',
          githubLink: 'https://github.com/rizwanmir/My-portfolio',
          description: 'I have developed this personal website to showcase my projects and will use a portfollio. I have used HTML, CSS/LESS and VueJS in this project.'

        }
      ]
    }
  }
}
</script>

<style scoped lang="less">
  .portfolio {
    margin: 4%;
  }

  @media screen and (min-width: 600px) {
  .portfolio {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin: 3vh 4vw 6vh 4vw;
  }
}
@media screen and (min-width: 992px) {
  .portfolio {
    margin: 3vh 9vw 6vh 9vw
  }
  
}
  .list-group-item {
    margin: 4px;
    background: #17a2b8;
    border: none;
    padding: 0.20rem 0.8rem;
    border-radius: inherit;
    color: #fff;
    font-size: 14px;
  }
  .card-img {
    padding: 40px;
  }

  .portfolio_btn_container {
    margin-top: 1.5rem;
    .portfolio_btn {
        color: #da933f;
        background-color: transparent;
        border-bottom: 1px solid #da933f;
        font-size: 13px;
        padding: 0.375rem 0;
        letter-spacing: 2px;
        margin-right: 2rem;
        transition: all 0.15s;

        span {
            margin-left: 0;
            transition: all 0.15s;
        }

        &:hover {
            margin-right: 1.5rem;
            border-color: #da933f;
            color: #da933f;
            text-decoration: none;
            span {
                margin-left: 0.5rem;
                path {
                    stroke: #da933f;
                }
            }
        }
    }
}

</style>