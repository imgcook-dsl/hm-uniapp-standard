<template>
  <div class="box">
    <div @click="handleClick_1" v-for="(item, index) in loopData" :key="index">
      <div class="bd">
        <img class="layer" :src="constants.image1" />
        <img class="bg" :src="constants.image2" />
        <div class="wrap">
          <img class="riverdinwei" :src="constants.image3" />
          <span class="distance">距离500m</span>
        </div>
      </div>
      <div class="main">
        <span class="title">{{ item.title }}</span>
      </div>
      <div class="ft">
        <div class="block">
          <img class="xianjin" :src="item.user.userImage" />
          <span class="fashionHome">{{ item.user.userName }}</span>
        </div>
        <div class="group">
          <img class="favorite" :src="constants.image4" />
          <span class="num">{{ item.readCount }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { fetch } from 'whatwg-fetch';
export default {
  data() {
    return {
      stateData: 'test',
      loopData: [
        {
          title: '小户型卫浴怎样才能装得高大上？',
          coverImage:
            'https://img.alicdn.com/tfs/TB1Txq6o7T2gK0jSZFkXXcIQFXa-684-684.png',
          readCount: 200,
          user: {
            userImage:
              'https://img.alicdn.com/tfs/TB1DWe6oYj1gK0jSZFOXXc7GpXa-60-60.png',
            userName: '时尚家居'
          },
          url: 'https://www.imgcook.com'
        },
        {
          title: '拥有超多功能的40平米简约小公寓了解一下',
          coverImage:
            'https://img.alicdn.com/tfs/TB1XRQTo7P2gK0jSZPxXXacQpXa-684-648.png',
          readCount: 500,
          user: {
            userImage:
              'https://img.alicdn.com/tfs/TB1DWe6oYj1gK0jSZFOXXc7GpXa-60-60.png',
            userName: '花花设计工作'
          },
          url: 'https://www.imgcook.com/docs'
        }
      ],
      constants: {
        image1:
          'https://img.alicdn.com/tfs/TB1DDx_rQL0gK0jSZFxXXXWHVXa-684-684.png',
        image2:
          'https://img.alicdn.com/tfs/TB10TB_rQL0gK0jSZFxXXXWHVXa-684-684.png',
        image3:
          'https://img.alicdn.com/tfs/TB1UoB9rQL0gK0jSZFAXXcA9pXa-28-36.png',
        image4:
          'https://img.alicdn.com/tfs/TB1pxuarHj1gK0jSZFuXXcrHpXa-46-44.png'
      }
    };
  },
  methods: {
    isReadCountShow(readCount) {
      return readCount > 300;
    },
    fetch_example() {
      fetch('https://jsonplaceholder.typicode.com/todos/1', {
        method: 'GET',
        body: {}
      })
        .then(response => response.json())
        .then((data, error) => {
          console.log(dataHandler);
          return data;
        })
        .catch(e => {
          console.log('error', e);
        });
    },
    dataHandler(dataMap) {
      console.log('dataHandler 11');
      return dataMap;
    },
    handleClick_1(e) {
      window.open(this.item.url);
    }
  },
  created() {
    console.log('constructor');
    this.fetch_example();
    this.dataHandler();
  },
  beforeUpdate() {
    console.log('getDerivedStateFromProps');
  }
};
</script>

<style scoped>
.box {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: flex-start;
  height: 534px;
}

.bd {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: row;
  opacity: 1;
  width: 342px;
  height: 342px;
}

.layer {
  position: absolute;
  top: 0;
  left: 0;
  width: 342px;
  height: 342px;
  overflow: hidden;
}

.bg {
  position: absolute;
  top: 0;
  left: 0;
  opacity: 1;
  width: 342px;
  height: 342px;
}

.wrap {
  box-sizing: border-box;
  display: flex;
  position: absolute;
  top: 18px;
  left: 18px;
  align-items: center;
  flex-direction: row;
  border-radius: 15px;
  background-color: rgba(0, 0, 0, 0.4);
  padding-right: 9px;
  padding-left: 10px;
  height: 30px;
}

.riverdinwei {
  opacity: 1;
  width: 14px;
  height: 18px;
}

.distance {
  margin-left: 4px;
  width: 84px;
  height: 22px;
  line-height: 22px;
  white-space: nowrap;
  color: #ffffff;
  font-size: 18px;
  font-weight: 400;
}

.main {
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: center;
  background-color: #ffffff;
  width: 342px;
  height: 114px;
}

.title {
  margin-top: 22px;
  width: 300px;
  height: 88px;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 44px;
  color: #333333;
  font-size: 30px;
  font-weight: 400;
}

.ft {
  box-sizing: border-box;
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
  border-bottom-left-radius: 12px;
  border-bottom-right-radius: 12px;
  background-color: #ffffff;
  padding-right: 17px;
  padding-left: 18px;
  width: 342px;
  height: 78px;
  overflow: hidden;
}

.block {
  display: flex;
  align-items: center;
  flex-direction: row;
  height: 30px;
}

.xianjin {
  width: 30px;
  height: 30px;
}

.fashionHome {
  margin-left: 6px;
  line-height: 28px;
  white-space: nowrap;
  color: #666666;
  font-size: 24px;
  font-weight: 300;
}

.group {
  display: flex;
  align-items: center;
  flex-direction: row;
  height: 30px;
}

.favorite {
  width: 22px;
  height: 22px;
}

.num {
  margin-left: 5px;
  line-height: 26px;
  white-space: nowrap;
  color: #999999;
  font-size: 22px;
  font-weight: 400;
}
</style>
