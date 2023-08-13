<template>
  <div :id="!bigflag ? 'xiao' : 'da'" class="box">
    <span class="icons">
      <b @click="bigflag = !bigflag">
        <svg
          v-show="!bigflag"
          t="1691743488525"
          class="icon"
          viewBox="0 0 1026 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="8451"
          width="16"
          height="16"
        >
          <path
            d="M163.2 94.08a48 48 0 0 0-67.84 0 48 48 0 0 0 0 67.84l67.84-67.84z m145.28 279.04a48 48 0 0 0 67.84 0 48 48 0 0 0 0-67.84L308.48 373.12z m-213.12-211.2l213.12 211.2 67.84-67.84-213.12-211.2-67.84 67.84zM95.36 859.52a48 48 0 0 0 67.84 68.48l-67.84-68.48z m280.96-142.72a48 48 0 0 0-67.84-68.48l67.84 68.48z m-213.12 211.2l213.12-211.2-67.84-68.48-213.12 211.2 67.84 68.48zM863.36 928a48 48 0 0 0 67.84-67.84l-67.84 67.84z m-143.36-279.04a47.36 47.36 0 0 0-67.84 0 48 48 0 0 0 0 67.84l67.84-67.84z m211.2 211.2l-211.2-211.2-67.84 67.84 211.2 211.2 67.84-67.84zM929.28 161.92a48 48 0 0 0 0-67.84 49.28 49.28 0 0 0-68.48 0l68.48 67.84z m-279.68 143.36a48 48 0 0 0 0 67.84 49.28 49.28 0 0 0 68.48 0l-68.48-67.84z m211.2-211.2l-211.2 211.2 68.48 67.84 211.2-211.2-68.48-67.84z"
            fill="#e6e6e6"
            p-id="8452"
          ></path>
          <path
            d="M704 80a48 48 0 0 0 0 96v-96zM896 128h48a48.64 48.64 0 0 0-48-48V128z m-48 192a48 48 0 0 0 96 0zM704 176h192v-96h-192v96zM849.28 128v192h96V128zM945.28 704a48 48 0 0 0-96 0zM896 896v48a48.64 48.64 0 0 0 48-48z m-192-48a48 48 0 0 0 0 96v-96zM849.28 704v192h96v-192z m46.72 144h-192v96h192v-96zM320 944a48 48 0 0 0 0-96v96zM128 896h-46.72a48 48 0 0 0 48 48V896z m48-192a48 48 0 0 0-96 0zM320 848H128v96h192v-96zM177.28 896v-192h-96v192zM81.28 320a48 48 0 0 0 96 0zM128 128v-48a48 48 0 0 0-46.72 48z m192 48a48 48 0 0 0 0-96v96zM177.28 320V128h-96v192zM128 176h192v-96H128v96z"
            fill="#e6e6e6"
            p-id="8453"
          ></path>
        </svg>
        <svg
          v-show="bigflag"
          t="1691744717898"
          class="icon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="10597"
          width="16"
          height="16"
        >
          <path
            d="M887.44 583.9H136.56c-39.71 0-71.9-32.19-71.9-71.9s32.19-71.9 71.9-71.9h750.87c39.71 0 71.9 32.19 71.9 71.9s-32.19 71.9-71.89 71.9z"
            fill="#dbdbdb"
            p-id="10598"
          ></path>
        </svg>
      </b>
      <b>
        <svg
          t="1691743735517"
          class="icon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="9558"
          width="16"
          height="16"
        >
          <path
            d="M567.168 512l189.184 188.352a40.064 40.064 0 0 1 0.768 55.68 37.76 37.76 0 0 1-54.4 0.832L512 566.912l-190.72 189.952a37.76 37.76 0 0 1-54.4-0.768 40.064 40.064 0 0 1 0.768-55.68L456.832 512 267.648 323.648a40.064 40.064 0 0 1-0.768-55.68 37.76 37.76 0 0 1 54.4-0.832L512 457.088l190.72-189.952a37.76 37.76 0 0 1 54.4 0.768 40.064 40.064 0 0 1-0.768 55.68L567.168 512z"
            fill="#dbdbdb"
            p-id="9559"
          ></path>
        </svg>
      </b>
    </span>
    <img class="title_img" src="../assets/热搜榜.png" alt="" />
    <div id="box">
      <div class="box_con">
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
            :tabdata="arr"
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
    <div class="con">
      <ConLeft :tabdata="arr" @ss="sssFun" :flag="flag" />
      <ConRight :tabcon="arr[a]" />
    </div>
  </div>
</template>

<script>
//数据
import conarr from "../components/arr.json";
//身体左侧导航
import ConLeft from "../components/ConLeft.vue";
//身体主体
import ConRight from "../components/ConRight.vue";
export default {
  data() {
    return {
      bigflag: false,
      arr: [],
      tab: [
        {
          title: "我的订阅",
          flag: false,
        },
        {
          title: "全部",
          flag: true,
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
      ],
      a: 0,
      //我的订阅状态
      flag: false,
    };
  },
  components: {
    ConLeft,
    ConRight,
  },
  methods: {
    sssFun(n) {
      console.log(n);
      this.a = n;
    },
    lifun(sindex) {
      this.a = 0;
      //传递数据
      this.arr = [];
      //我的订阅
      if (sindex == 0) {
        this.arr = conarr.filter((item) => item.dingyue == "true");
        this.flag = true;
      }
      //全部
      if (sindex == 1) {
        this.arr = conarr;
        this.flag = false;
      }
      if (sindex > 1) {
        this.flag = false;
        conarr.forEach((item) => {
          if (item.from == JSON.stringify(sindex - 1)) {
            this.arr.push(item);
          }
        });
      }
      // console.log(this.arr);

      // this.$refs.childComponent.updateData(this.dataFromParent);
      //li选中状态
      this.tab.forEach((item, index) => {
        if (sindex == index) {
          item.flag = true;
        } else {
          item.flag = false;
        }
      });
    },
  },
  mounted() {
    conarr.forEach((item) => {
      this.arr.push(item);
    });
  },
};
</script>

<style lang="scss" scoped>
//身体
.con {
  width: 100%;
  height: 84%;
  display: flex;
  flex-direction: row;
  margin-top: 1.5%;
  border-top: 1px solid rgba(245, 245, 245, 0.04);
}
//头部
#box {
  width: 96%;
  height: 32px;
  margin: auto;
  padding-top: 50px;
  position: relative;
  z-index: -1;
  border-bottom: 3px solid #414243;
  color: white;
  .box_con {
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
#xiao {
  width: 1000px !important;
  height: 650px !important;
  border-radius: 10px !important;
}
#da {
  width: 100vw !important;
  height: 100vh !important;
}
.box {
  background: #1c1c1e;
  position: relative;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);

  transition: all 0.2s;

  .icons {
    display: block;
    display: flex;
    flex-direction: row;
    width: 55px;
    justify-content: space-between;
    position: absolute;
    right: 5px;
    top: 5px;
    b {
      display: block;
      width: 25px;
      height: 25px;
      background: #49494b;
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: all 0.3s;
      svg {
        width: 14px;
        height: 14px;
      }
    }
    b:nth-child(1):hover {
      background: #a4a4a5 !important;
    }
    b:nth-child(2):hover {
      background: #e81123 !important;
    }
  }
}
.title_img {
  margin-top: 5px;
  position: absolute;
  left: 50%;
  transform: translate(-50%);
}
</style>
