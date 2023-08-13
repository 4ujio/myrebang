<template>
  <div class="con-right" style="color: white">
    <div class="right_hea">
      <img :src="tabcon.img" alt="" />
      <span>{{ tabcon.title }}</span>
      <svg
        data-v-d7b5176e=""
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1024 1024"
      >
        <path
          fill="currentColor"
          d="M512 64a448 448 0 1 1 0 896.064A448 448 0 0 1 512 64zm67.2 275.072c33.28 0 60.288-23.104 60.288-57.344s-27.072-57.344-60.288-57.344c-33.28 0-60.16 23.104-60.16 57.344s26.88 57.344 60.16 57.344zM590.912 699.2c0-6.848 2.368-24.64 1.024-34.752l-52.608 60.544c-10.88 11.456-24.512 19.392-30.912 17.28a12.992 12.992 0 0 1-8.256-14.72l87.68-276.992c7.168-35.136-12.544-67.2-54.336-71.296-44.096 0-108.992 44.736-148.48 101.504 0 6.784-1.28 23.68.064 33.792l52.544-60.608c10.88-11.328 23.552-19.328 29.952-17.152a12.8 12.8 0 0 1 7.808 16.128L388.48 728.576c-10.048 32.256 8.96 63.872 55.04 71.04 67.84 0 107.904-43.648 147.456-100.416z"
        ></path>
      </svg>
    </div>
    <ul>
      <li v-for="(item, index) in tabcon.data" :key="index">
        <b v-color="index">{{ ++index }}</b>
        <span>{{ item.title }}</span>
        <i style="font-style: normal">{{ item.hotValue }}</i>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  directives: {
    color(i, n) {
      if (n.value == 0) {
        i.style.background = "#fe2d46";
      }
      if (n.value == 1) {
        i.style.background = "#ff6600";
      }
      if (n.value == 2) {
        i.style.background = "#faa90e";
      }
    },
  },
  props: {
    tabcon: {
      type: [Object, Array],
      required: true,
    },
  },
  data() {
    return {
      dataobj: {},
      num: 0,
    };
  },
  //   watch: {
  //     tabcon(newValue) {
  //       this.arr = newValue;
  //     },
  //   },
  mounted() {
    this.dataobj = this.tabcon;
  },
};
</script>

<style lang="scss" scoped>
.con-right {
  width: 73%;
  height: 100%;
  padding: 0 2%;
  //   background: red;
  .right_hea {
    width: 100%;
    height: 10%;
    border-bottom: 1px solid rgba(245, 245, 245, 0.04);
    display: flex;
    align-items: center;
    position: relative;
    img {
      width: 20px;
      height: 20px;
      margin-right: 10px;
      display: block;
      border-radius: 50%;
    }
    span {
      color: #dfdddd;
      font-size: 20px;
    }
    svg {
      position: absolute;
      right: 0;
      width: 17px;
      height: 17px;
    }
  }
  ul {
    overflow: auto;
    scrollbar-width: thin; /* Firefox */
    scrollbar-color: transparent transparent; /* Firefox */
  }

  /* 定制滚动条样式 */
  ul::-webkit-scrollbar {
    width: 4px;
    height: 30px;
  }

  ul::-webkit-scrollbar-thumb {
    background-color: gray; /* 滚动条颜色 */
  }

  ul::-webkit-scrollbar-track {
    background-color: transparent; /* 轨道背景颜色 */
  }
  ul {
    width: 100%;
    height: 90%;
    // overflow: auto;
    position: relative;

    li {
      width: 100%;
      display: flex;
      align-items: center;
      padding: 8px 0;
      color: #dfdddd;
      b {
        display: block;
        width: 20px;
        height: 20px;
        background: #25252c;
        font-weight: normal;
        line-height: 18px;
        text-align: center;
        border-radius: 4px;
        margin-right: 15px;
        font-size: 12px;
      }
      i {
        position: absolute;
        right: 0;
        color: gray;
        font-size: 14px;
      }
    }
    li:hover {
      color: #1981ff;
    }
  }
}
</style>
