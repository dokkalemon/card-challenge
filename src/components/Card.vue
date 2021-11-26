<template>
  <div class="card-container">
      <div class="img-container">
          <img src="@/assets/image-equilibrium.jpg" alt="">
      </div>
      <div class="title">
          <h3>Equilibrium #3429</h3>
      </div>
      <div class="text">
          <h4>Our Equilibrium collection promotes balance and calm.</h4>
      </div>
      <div class="setting">
          <div class="value">
              <img src="@/assets/icon-ethereum.svg" alt="">
              <h4>0.041ETH</h4>
          </div>
          <div class="date">
              <img src="@/assets/icon-clock.svg" alt="">
              <h4>3 days left</h4>
          </div>
      </div>

      <div class="line"></div>

      <div class="author">
          <img src="@/assets/image-avatar.png" alt="">
          <h4>Creation of <span>Jules Wyvern</span></h4>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Card',
}
</script>

<style scoped lang="scss">
@import '@/styles/vars';

.card-container {
    height: 580px;
    width: 346px;
    background-color: $card-bg;
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.253);
    padding: 20px;
    border-radius: 15px;
    .img-container {
        width: 100%;
        img {
            width: 100%;
            border-radius: 10px;
        }
    }
    .title {
        padding: 15px 0;
        h3 {
            color: $white;
            font-weight: 400;
            font-size: 22px;
        }
    }
    .text {

        h4 {
            color: $white;
            font-weight: 300;
            font-size: 18px;
            color: $soft-blue;
            line-height: 25px;
        }
    }
    .setting {
        padding: 25px 0px;
        display: flex;
        .value {
            width: 100%;
            display: flex;
            justify-content: flex-start;
            align-self: start;
            img {
                margin-right: 5px;
                height: 90%;
            }
            h4 {
                color: $cyan;
                font-weight: 400;
            }
           
            

        }
        .date {
            width: 100%;
            display: flex;
            justify-content: flex-end;
            align-items: center;
            img {
                margin-right: 8px;
                height: 80%;
            }
            h4 {
                color: $soft-blue;
                font-weight: 300;
            }
           
           
        }
    }
    .line {
        height: 1px;
        width: 100%;
        background-color: $line;
    }
    .author {
        display: flex;
        align-items: center;
        padding: 15px 0;
        img {
            width: 35px;
            border: 1px solid white;
            border-radius: 100%;
            margin-right: 15px;
        }
        h4 {
            color: $soft-blue;
            font-weight: 300;
        }
        span {
            color: $white;
        }
    }
    
}

</style>