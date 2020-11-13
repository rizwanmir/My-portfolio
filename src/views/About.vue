<template>
  <div class="container">
    <div class="profile">
      <b-row no-gutters>
        <b-col md="6">
          <b-card-body>
        <b-card-text>
          <span class="title">About Rizwan Mir</span>
          <h2 class="heading">
            Intrested in 
            <br>
            <span class="text-highlight">
              Modern solutions
            </span>
            <br>
              to develop interesting
              <br>
              web applications.
          </h2>
          <p class="description">
            I have great commitment and willingness to work and succeed in the feild of web development. I have growth
            mindset attitude where I want to learn and grow everyday by working with diversity of people. I have interest
            in frontend development by working with modern technologies and I am also interested to devleop my skills in
            backend develoopment.
          </p>
        </b-card-text>
          </b-card-body>
        </b-col>
        <b-col md="6">
      <b-card-img :src='profileImg' img-alt="profile" img-right ></b-card-img>
        </b-col>
      
      </b-row>
      

      </div>
    </div>
 
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      profileImg:require('@/assets/profile.jpg')
    }
  }
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
  font-size: 13px;
  line-height: 26px;
  letter-spacing: .5px;
  color: #222;
  font-weight: 300;
}

</style>