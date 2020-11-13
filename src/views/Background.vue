<template>
  <div class="container">
    <div class="profile">
      <b-row no-gutters>
        <b-col md="6">
          <b-card-body>
        <b-card-text>
          <span class="title">About Rizwan Mir</span>
          <h2 class="heading">
            Experience 
            <br>
            through
            <span class="text-highlight">
              Academics
            </span>
            <br>
              and
              <br>
              hobby projects
          </h2>
         
        </b-card-text>
          </b-card-body>
        </b-col>
        <b-col md="6">
       <p class="description">
            I have studied Web developemnt in E-commerce from Medieinstitutet Stockholm to pursue my interest in 
            digitalization. I have studied both frontend and backend development and I have gained good experience
            in working with HTML5, CSS3, JavaScript and PHP as backend development. I have also experience of working
            in VueJS and React to build single page applications. I am also interested to work with Restful API.
          </p>
        </b-col>
      
      </b-row>
      

      </div>
    </div>
 
</template>

<script>
export default {
  
}
</script>

<style scoped lang="less">
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
    height: 100vh;
  }
  .profile {
    display: flex;
    align-items: center;
    width: 80vw;
  }

.card {
  background: none;
  border: none;
  width: 100%;
  
}
.card-text {
  width: 80%;
}
.title {
  font-family: Questrial, sans-serif;
  text-transform: uppercase;
  letter-spacing: 2px;
  color: #444;
}
.card-img-right {
  width: 950px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  text-align: center;
}
.heading {
  font-size: 40px;
  line-height: 52px;
  border-left: 1px solid #da933f;
  padding-left: 20px;
  margin-top: 10px;
}
.text-highlight {
  color: #da933f;
}
.description {
  font-size: 18px;
  line-height: 26px;
  letter-spacing: .5px;
  color: #222;
  font-weight: 300;
}

</style>