<template>
  <div class="con-left">
    <!-- <a style="color: white">{{ tabdata }}</a> -->
    <input type="text" placeholder="搜索" />
    <ul v-show="flag">
      <li
        id="dingyue"
        @click="tabFun(index)"
        :class="index == liIndex ? 'li_active' : ''"
        v-for="(item, index) in arr"
        :key="index"
      >
        <svg
          t="1691917457212"
          class="icon oneicon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="17232"
          width="16"
          height="16"
        >
          <path
            d="M284.416 236.373333C221.610667 236.373333 170.666667 183.466667 170.666667 118.101333S221.610667 0 284.416 0c62.890667 0 113.834667 52.906667 113.834667 118.186667 0 65.194667-50.944 118.101333-113.834667 118.101333z m0 393.813334C221.610667 630.186667 170.666667 577.28 170.666667 512s50.944-118.186667 113.749333-118.186667c62.890667 0 113.834667 52.906667 113.834667 118.186667S347.306667 630.186667 284.416 630.186667z m455.168-393.898667c-62.890667 0-113.834667-52.906667-113.834667-118.101333C625.749333 52.906667 676.693333 0 739.584 0 802.389333 0 853.333333 52.906667 853.333333 118.186667c0 65.194667-50.944 118.101333-113.749333 118.101333z m0 393.898667c-62.890667 0-113.834667-52.906667-113.834667-118.186667s50.944-118.186667 113.834667-118.186667C802.389333 393.813333 853.333333 446.72 853.333333 512s-50.944 118.186667-113.749333 118.186667zM284.416 1024C221.610667 1024 170.666667 971.093333 170.666667 905.813333c0-65.194667 50.944-118.101333 113.749333-118.101333 62.890667 0 113.834667 52.906667 113.834667 118.101333C398.250667 971.093333 347.306667 1024 284.416 1024z m455.168 0c-62.890667 0-113.834667-52.906667-113.834667-118.186667 0-65.194667 50.944-118.101333 113.834667-118.101333 62.805333 0 113.749333 52.906667 113.749333 118.101333C853.333333 971.093333 802.389333 1024 739.584 1024z"
            fill="#dbdbdb"
            p-id="17233"
          ></path>
        </svg>
        <img :src="item.img" alt="" />
        <b>{{ item.name }}</b>
        <svg
          t="1691917776385"
          class="icon iconlast"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="17435"
          width="16"
          height="16"
        >
          <path
            d="M150.528 431.104q37.888 0 58.368 24.064t20.48 51.712l0 11.264q0 34.816-17.92 58.88t-59.904 24.064l-7.168 0q-38.912 0-61.952-21.504t-23.04-59.392l0-14.336q0-13.312 5.632-26.624t15.872-24.064 25.6-17.408 33.792-6.656l10.24 0zM519.168 431.104q37.888 0 58.368 24.064t20.48 51.712l0 11.264q0 34.816-17.92 58.88t-59.904 24.064l-7.168 0q-38.912 0-61.952-21.504t-23.04-59.392l0-14.336q0-13.312 5.632-26.624t15.872-24.064 25.6-17.408 33.792-6.656l10.24 0zM887.808 431.104q37.888 0 58.368 24.064t20.48 51.712l0 11.264q0 34.816-17.92 58.88t-59.904 24.064l-7.168 0q-38.912 0-61.952-21.504t-23.04-59.392l0-14.336q0-13.312 5.632-26.624t15.872-24.064 25.6-17.408 33.792-6.656l10.24 0z"
            p-id="17436"
            fill="#dbdbdb"
          ></path>
        </svg>
        <button class="del" @click="delfun(index)">删除</button>
      </li>
    </ul>

    <ul v-show="!flag">
      <li
        @click="tabFun(index)"
        :class="index == liIndex ? 'li_active' : ''"
        v-for="(item, index) in arr"
        :key="index"
      >
        <img :src="item.img" alt="" />
        <b>{{ item.name }}</b>
        <svg
          @click="sc(0, index)"
          v-if="item.dingyue == 'true'"
          t="1691825376329"
          class="icon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="13996"
          width="16"
          height="16"
        >
          <path
            d="M335.008 916.629333c-35.914667 22.314667-82.88 10.773333-104.693333-25.557333a77.333333 77.333333 0 0 1-8.96-57.429333l46.485333-198.24a13.141333 13.141333 0 0 0-4.021333-12.864l-152.16-132.586667c-31.605333-27.52-35.253333-75.648-8.234667-107.733333a75.68 75.68 0 0 1 51.733333-26.752L354.848 339.2c4.352-0.362667 8.245333-3.232 10.026667-7.594667l76.938666-188.170666c16.032-39.2 60.618667-57.92 99.52-41.461334a76.309333 76.309333 0 0 1 40.832 41.461334l76.938667 188.16c1.781333 4.373333 5.674667 7.253333 10.026667 7.605333l199.712 16.277333c41.877333 3.413333 72.885333 40.458667 69.568 82.517334a76.938667 76.938667 0 0 1-26.08 51.978666l-152.16 132.586667c-3.541333 3.082667-5.141333 8.074667-4.021334 12.853333l46.485334 198.24c9.621333 41.013333-15.36 82.336-56.138667 92.224a75.285333 75.285333 0 0 1-57.525333-9.237333l-170.976-106.24a11.296 11.296 0 0 0-12.010667 0l-170.986667 106.24zM551.786667 756.032l170.976 106.24c2.624 1.621333 5.717333 2.122667 8.650666 1.408 6.410667-1.557333 10.56-8.426667 8.928-15.424l-46.485333-198.24a77.141333 77.141333 0 0 1 24.277333-75.733333L870.293333 441.706667c2.485333-2.165333 4.053333-5.312 4.330667-8.746667 0.565333-7.136-4.490667-13.173333-10.976-13.696l-199.712-16.288a75.989333 75.989333 0 0 1-64.064-47.168l-76.938667-188.16a12.309333 12.309333 0 0 0-6.538666-6.741333c-5.898667-2.496-12.725333 0.373333-15.328 6.741333l-76.949334 188.16a75.989333 75.989333 0 0 1-64.064 47.168l-199.701333 16.288a11.68 11.68 0 0 0-7.978667 4.181333 13.226667 13.226667 0 0 0 1.333334 18.261334l152.16 132.586666a77.141333 77.141333 0 0 1 24.277333 75.733334l-46.485333 198.229333a13.333333 13.333333 0 0 0 1.514666 9.877333c3.488 5.792 10.581333 7.530667 16.064 4.128l170.986667-106.229333a75.296 75.296 0 0 1 79.562667 0z"
            fill="#ffffff"
            p-id="13997"
          ></path>
        </svg>
        <svg
          @click="sc(1, index)"
          v-if="item.dingyue == 'false'"
          t="1691826326716"
          class="icon"
          viewBox="0 0 1024 1024"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          p-id="14295"
          width="16"
          height="16"
        >
          <path
            d="M335.008 916.629333c-35.914667 22.314667-82.88 10.773333-104.693333-25.557333a77.333333 77.333333 0 0 1-8.96-57.429333l46.485333-198.24a13.141333 13.141333 0 0 0-4.021333-12.864l-152.16-132.586667c-31.605333-27.52-35.253333-75.648-8.234667-107.733333a75.68 75.68 0 0 1 51.733333-26.752L354.848 339.2c4.352-0.362667 8.245333-3.232 10.026667-7.594667l76.938666-188.170666c16.032-39.2 60.618667-57.92 99.52-41.461334a76.309333 76.309333 0 0 1 40.832 41.461334l76.938667 188.16c1.781333 4.373333 5.674667 7.253333 10.026667 7.605333l199.712 16.277333c41.877333 3.413333 72.885333 40.458667 69.568 82.517334a76.938667 76.938667 0 0 1-26.08 51.978666l-152.16 132.586667c-3.541333 3.082667-5.141333 8.074667-4.021334 12.853333l46.485334 198.24c9.621333 41.013333-15.36 82.336-56.138667 92.224a75.285333 75.285333 0 0 1-57.525333-9.237333l-170.976-106.24a11.296 11.296 0 0 0-12.010667 0l-170.986667 106.24z"
            fill="#dbdbdb"
            p-id="14296"
          ></path>
        </svg>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: [],
      liIndex: 0,
    };
  },
  props: {
    tabdata: {
      type: [Object, Array],
      required: true,
    },
    flag: {
      type: Boolean,
      required: true,
    },
  },
  watch: {
    tabdata(newValue) {
      this.arr = newValue;
    },
  },
  mounted() {
    this.arr = this.tabdata;
  },
  methods: {
    tabFun(n) {
      this.liIndex = n;
      this.$emit("ss", n);
    },
    sc(num, index) {
      if (num == 0) {
        this.arr[index].dingyue = "false";
        this.$message.error("已取消收藏" + this.arr[index].name);
      } else if (num == 1) {
        this.arr[index].dingyue = "true";
        this.$message({
          message: "收藏成功！",
          type: "success",
        });
      }
    },
    delfun(index) {
      //   console.log(this.arr[index]);

      this.$confirm("确定要取消此订阅吗?", "提示", {
        confirmButtonText: "确定",
        cancelButtonText: "取消",
        type: "warning",
      })
        .then(() => {
          this.arr[index].dingyue = "false";
          this.arr = this.arr.filter((item) => item.dingyue == "true");
        })
        .catch(() => {
          this.arr[index].dingyue = "true";
        });
    },
  },
};
</script>

<style lang="scss" scoped>
.del {
  position: absolute;
  right: 30px;
  transition: all 0.2s;
  border: none;
  padding: 5px 10px;
  font-size: 13px;
  border-radius: 5px;
  display: none;
}
#dingyue {
  padding: 14px 14px 14px 35px;
  font-size: 13px;
  display: flex;
  align-items: center;
  position: relative;
  color: white;
  transition: all 0.1s linear;
  img {
    margin-left: 10px;
    width: 20px;
    height: 20px;
    border-radius: 3px;
  }
  .oneicon {
    width: 16px;
    height: 16px;
    position: absolute;
    left: 20px;
  }
  .iconlast {
    width: 16px;
    height: 16px;
    position: absolute;
    right: 14px;
  }
  .iconlast:hover {
    .del {
      display: block;
    }
  }
  b {
    // color: white;
    margin-left: 7px;
  }
}
#dingyue:hover {
  color: white;
  .del {
    display: block;
  }
  svg path {
    fill: white;
  }
}
.li_active {
  background: #1681ff !important;
  color: white !important;
  svg path {
    fill: #ffffff;
  }
}
.con-left {
  width: 20%;
  padding-right: 3%;
  padding-top: 0.6%;
  height: 99.4%;
  //   background: yellowgreen;
  border-right: 1px solid rgba(245, 245, 245, 0.04);
  input {
    width: 100%;
    margin-left: 4%;
    background: #25252c;
    outline-style: none;
    border: none;
    height: 26px;
    border-radius: 8px;
    text-indent: 10px;
    margin-bottom: 4%;
  }
  ul {
    width: 100%;
    list-style: none;

    li {
      padding: 10px 14px 10px 20px;
      font-size: 13px;
      display: flex;
      align-items: center;
      position: relative;
      color: white;
      transition: all 0.1s linear;
      img {
        margin-left: 10px;
        width: 20px;
        height: 20px;
        border-radius: 3px;
      }
      svg {
        width: 20px;
        height: 20px;
        position: absolute;
        right: 14px;
      }
      b {
        // color: white;
        margin-left: 7px;
      }
    }
    li:hover {
      color: #1681ff;
      svg path {
        fill: rgb(87, 111, 187);
      }
    }
  }
}
</style>
