<template>
  <div class="home">
    <div class="text-item">
      <div class="item-title">
        <h1> What Is Smail</h1>
      </div>
      <p>S’Mail is sort of an email client application that enable configuring one or more email addresses to receive, read, compose and send emails from one user to another.</p>
      <div class="btnlist">
        <button class="btn btn-outline-light" v-b-modal.showus>About Us</button>
        <router-link to="/user/register" class="btn btn-dark">Join Us</router-link>
      </div>
    </div>
    <div class="image-item">
      <img src="@/assets/Speedwagon_sepia.jpg" alt="" class="image">
    </div>

    <!-- sizenya bisa 3 macem xl, lg, sm-->
    <b-modal size="xl" id="showus">
      <div class="Frameouter">
          <div class="Frameinner">
          <div class="Background"></div>
          <div class="header">
              <div class="title">
                  <h1>Speedwagon Fo'un</h1>
              </div>
          </div>
          <div class="Text">
              <div class="one">
                  <p>At the beginning of the century, a lone Englishman by the name of Robert E. O. Speedwagon, arrived in the USA and started his own oil business. </p>
              </div>
              <div class="two">
                  <p>Because of this he became one of the world's richest men. Speedwagon decided that after his demise, the large sum of his fortune would be used for medical research and wild animal and plant protection.</p>
              </div>
              <div class="three">
                  <p>In this organization exists a department called the Supernatural Research Department, which is responsible for supplying the Joestar Family with everything they need. This was the will of Speedwagon, who died in 1952.</p>
              </div>
          </div>
          <div class="Founder">
              <div class="Robert">
                  <p>Founder :</p>
                  <p>Robert E. O. Speedwagon</p>
              </div>
          </div>
      </div>
    </div>
  </b-modal>
  



  </div>
</template>


<script>
export default {
  name: "Home",
  components: {}
  
}

</script>

<style scoped lang=scss>
.text-item{
  .item-title{
    h1:before{
      content: "What Is Smail";
      left: -180px;
    }
  }
}
.image-item{
  margin-right: 0;
  .image{
    width: 50vw;
  }
}
.btnlist{
  display: flex;
  justify-content: space-between;
  .btn{
    font-family: Roboto;
    padding: .8rem 50px;
  }
}


.Frameouter{
    position: relative;
    width: 802px;
    height: 618px;
    
    background: #938D8D;
    max-width: 1000px;
    margin: auto;
}
.Frameinner{
    position: absolute;
    width: 756px;
    height: 570px;
    left: 22px;
    top: 23px;

    background: #DBEFF0;
    .Background{
        position: absolute;
        width: 755px;
        height: 571px;
        left: -1px;
        top: -1px;
    
        background: url('/assets/Speed.png'); 
        background-repeat: no-repeat;
        background-size: 100% 100%;
        opacity: 0.1;
    }
}

.header{
    display: flex;
    flex-direction: column;
    align-content: flex-start;
    .title{
        h1{
            text-decoration: underline;
        }
    }
}
.Text{
    display: flex;
    flex-direction: column;
    width: 718px;
    height: 335px;
    top: 123px;
    left: 19px;
    
    font-family: Roboto;
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 28px;

    color: #7A6868;
}

.Founder{
    position: absolute;
    width: 328px;
    height: 44px;
    left: 409px;
    top: 440px;

    font-family: Roboto;
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 28px;
    text-align: right;

    color: #000000;
}


</style>