<template>
  <div class="card-container">
      <div class="img-container">
          <img :src="require(`../assets/${thumb}`)" alt="">
          <div class="hover-effect">
              <img src="@/assets/icon-view.svg" alt="">
          </div>
      </div>
      <div class="title">
          <h3>{{ title }}</h3>
      </div>
      <div class="text">
          <h4>{{ text }}</h4>
      </div>
      <div class="setting">
          <div class="value">
              <img src="@/assets/icon-ethereum.svg" alt="">
              <h4>{{ value }}</h4>
          </div>
          <div class="date">
              <img src="@/assets/icon-clock.svg" alt="">
              <h4>{{ date}}</h4>
          </div>
      </div>

      <div class="line"></div>

      <div class="author">
          <img :src="require(`../assets/${avatar}`)" alt="">
          <h4>Creation of <span>{{ name }}</span></h4>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Card',

    props: {
        thumb: String,
        title: String,
        text: String,
        value: String,
        date: String,
        avatar: String,
        name: String,
    }
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
        height: 57%;
        width: 100%;
        position: relative;
        overflow: hidden;
        border-radius: 10px;
        cursor: pointer;
        img {
            height: 100%;
            width: 100%;
        }
        .hover-effect {
            height: 100%;
            width: 100%;
            background-color: hsla(178, 100%, 50%, 0.473);
            position: absolute;
            top: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            opacity: 0;
            transition: all 0.5s ease;
            img {
                height: 50px;
                width: 50px;
            }
        }
        &:hover .hover-effect {
            opacity: 1;
        }
    }
    .title {
        padding: 15px 0;
        h3 {
            color: $white;
            font-weight: 400;
            font-size: 22px;
            cursor: pointer;
            transition: all .5s ease;

            &:hover {
                color: $cyan;
            }
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
            cursor: pointer;
            transition: all .5s ease;
            &:hover {
                color: $cyan;
            }
        }
    }
    
}

</style>