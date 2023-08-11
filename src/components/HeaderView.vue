<template>
  <div id="box">
    <div class="con">
      <p>
        <svg
          t="1691745490410"
          class="icon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="12435"
          width="16"
          height="16"
        >
          <path
            d="M729.6 931.2l-416-425.6 416-416c9.6-9.6 9.6-25.6 0-35.2-9.6-9.6-25.6-9.6-35.2 0l-432 435.2c-9.6 9.6-9.6 25.6 0 35.2l432 441.6c9.6 9.6 25.6 9.6 35.2 0C739.2 956.8 739.2 940.8 729.6 931.2z"
            p-id="12436"
            fill="#e6e6e6"
          ></path>
        </svg>
      </p>
      <ul>
        <li
          @click="lifun(index)"
          v-for="(item, index) in tab"
          :key="index"
          :class="item.flag ? 'li_true' : ''"
        >
          {{ item.title }}
        </li>
      </ul>
      <p>
        <svg
          t="1691745505953"
          class="icon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="12638"
          width="16"
          height="16"
        >
          <path
            d="M761.6 489.6l-432-435.2c-9.6-9.6-25.6-9.6-35.2 0-9.6 9.6-9.6 25.6 0 35.2l416 416-416 425.6c-9.6 9.6-9.6 25.6 0 35.2s25.6 9.6 35.2 0l432-441.6C771.2 515.2 771.2 499.2 761.6 489.6z"
            p-id="12639"
            fill="#e6e6e6"
          ></path>
        </svg>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tab: [
        {
          title: "我的订阅",
          flag: true,
        },
        {
          title: "全部",
          flag: false,
        },
        {
          title: "综合",
          flag: false,
        },
        {
          title: "科技",
          flag: false,
        },
        {
          title: "娱乐",
          flag: false,
        },
        {
          title: "社区",
          flag: false,
        },
        {
          title: "购物",
          flag: false,
        },
        {
          title: "财经",
          flag: false,
        },
        {
          title: "大学",
          flag: false,
        },
        {
          title: "日报",
          flag: false,
        },
        {
          title: "地方门户",
          flag: false,
        },
        {
          title: "影视",
          flag: false,
        },
        {
          title: "阅读",
          flag: false,
        },
      ],
    };
  },
  methods: {
    lifun(sindex) {
      this.tab.forEach((item, index) => {
        if (sindex == index) {
          item.flag = true;
          console.log(item);
        } else {
          item.flag = false;
        }
      });
    },
  },
};
</script>

<style lang="scss" scoped>
#box {
  width: 96%;
  height: 32px;
  margin: auto;
  padding-top: 50px;
  position: relative;
  z-index: -1;
  border-bottom: 3px solid #414243;
  color: white;
  .con {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-between;
    position: relative;
    ul {
      position: absolute;
      width: 94%;
      height: 35px;
      list-style: none;
      display: flex;
      justify-content: space-between;
      left: 3%;
      bottom: -3px;
      font-size: 14px;
      li {
        padding: 0 3px;
        letter-spacing: 1px;
        transition: all 0.1s linear;
      }
      li:hover {
        color: #1772de !important;
      }
      .li_true {
        // padding: 0 10px;
        border-bottom: 3px solid #1681ff !important;
        color: #1772de !important;
      }
      .li_false {
        border-bottom: 3px solid rgba(0, 0, 0, 0);
      }
    }
    p {
      display: block;
      display: flex;
      justify-content: center;
      width: 3%;
      height: 32px;
      background: #1c1c1e;
      svg {
        width: 14px;
        height: 14px;
        margin-top: 2px;
      }
    }
  }
}
</style>
