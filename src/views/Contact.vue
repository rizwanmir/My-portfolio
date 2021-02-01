<template>
    <div class="contact">
        <div class="contact-heading">
            <img src="@/assets/logo.jpg" />
            <h3>Rizwan <span>Mir</span> </h3>
        </div>
        <div class="contact-section">
            <div class="talk">
                <h3>Let's Talk</h3>
                <span>You can contact me by calling, email or via LinkedIn</span>
            </div>
            <div class="contact-details">
                <div>
                    <a href="tel:+46760906904">
                        <font-awesome-icon :icon="['fas', 'mobile']" />
                    +46760906904
                    </a>
                </div>
                <div>
                    <a href="mailto: rizwan_mir86@hotmail.com">
                        <font-awesome-icon :icon="['fas', 'envelope-square']" />
                        rizwan_mir86@hotmail.com
                    </a>
                </div>
                <div>
                    <a href="https://www.linkedin.com/in/rizwan-mir-344b5817/" target="_blank">
                        <font-awesome-icon :icon="['fab', 'linkedin']" />
                        rizwan-mir-344b5817
                    </a>
                </div>  
            </div> 
        </div>
       
    </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="less">
.contact {
    margin: 0 8% 0 8%;
    height: 100vh;
}
.contact-heading {
    padding: 10px 0 10px 0;
    display: flex;
    align-items: center;

    img {
        width: 80px;
        height: 80px;
        border-radius: 50%;
    }

    h3 {
        padding-left: 15px;
        font-family: Arial;
        font-size: 30px;
        font-weight: bold; 
        
        @media screen and (min-width: 600px) {
            font-size: 40px;
            padding-left: 20px;
        }
        span {
        color: rgb(179, 162, 162);
        }
    }
}
.contact-section {
    height: 60vh;
    background: rgb(223, 214, 214);
    position: relative;
    margin-top: 4vh;

     @media screen and (min-width: 600px) {
         height: 70vh;
     }
}
.talk {
    position: absolute;
    width: 100%;
    background: #17a2b8;
    top: 15%;
    height: 12vh;
    text-align: center;
    
    h3 {
        color: #da933f;
        font-family: Arial;
        font-size: 30px;
        font-weight: bold;

         @media screen and (min-width: 600px) {
             font-size: 50px;
         }
    }
    span {
        font-size: 10px;
        color: #ffff;

         @media screen and (min-width: 600px) {
             font-size: 16px;
         }
    }
}
.contact-details {
    position: absolute;
    top: 50%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 10px;

     @media screen and (min-width: 600px) {
         flex-direction: row;
         justify-content: space-around;
     }

     a {
         color: black;
     }
}
</style>