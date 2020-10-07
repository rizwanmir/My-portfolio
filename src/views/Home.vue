<template>

    <div id="fullScreenDiv">
        
        <div id="videoDiv">           
            <!-- <video id="video" preload autoplay muted playsinline loop>
            <source src="@/assets/video.mp4" type="video/mp4" />
            </video>  -->
        </div>
        <div class="messageBox"> 
            <div class="name-heading">
                <h1>Rizwan <span> Mir </span></h1>
            </div>
            <div class="desc-heading">
                <h2>Web Developer - rizwan_mir86@hotmail.com - +46760906904 </h2>
            </div>
            <div class="icons">
                <h3>
                    <a href="#main" class="scrolly"><font-awesome-icon :icon="['fab', 'github']" /></a>
                    <a href="#main" class="scrolly"><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
                </h3>
            </div>
        </div>   
    </div>

  
</template>

<script>

export default {

}
</script>

<style scoped lang="less">
 /* Default to hide the video on all devices */
#video{display:none}

/* Default to display the image on all devices */
#videosubstitute{display:block;width:auto;height:100%;}

#fullScreenDiv{
    width:100%;
    min-height: 100%; 
   /* Set the height to match that of the viewport. */
    height: 100vh;
    width: auto;
    padding:0!important;
    margin: 0!important;
    background-color: gray;
    position: relative;
}
#video{    
    width: 300vw; 
    height: 100vh;
    object-fit: cover;
    left: 0px;
    top: 0px;
    z-index: -1;
    //position: absolute;
}

@media (min-aspect-ratio: 16/9) {
  #video{
    height: 150%;
    top: -100%;
  }
  #videosubstitute{
    display:block;
    width: 100%;
    height: auto;}
}

@media (max-aspect-ratio: 16/9) {
  #video {
    width: 150%;
    left: -100%;
  }
  #videosubstitute{display:block;width:auto;height:100%;}
}
/*if there is 992  pixels or more, then display the video but hide the image*/
@media only screen and (min-width : 992px) {
#video{display:block;}
#videosubstitute{display:none}
}   

/* The container for our text and stuff */
.messageBox{
    position: absolute;  top: 0;  left: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    height:100%;
}
.name-heading h1 {
    font-family: Arial;
    font-size: 60px;
    font-weight: bold;
    span {
        color: #ffff;
    }
}
.desc-heading {
    background: rgb(150, 147, 17);
    
    height: 5vh;
    padding: 10px;
    font-family: Arial;
    
    h2 {
        font-size: 18px;
        color: #ffff;
    }
}
.icons {
    padding: 20px;
    a {
        padding: 60px;
    }
}

</style>