<template>
    <cfooter class="footer">
        <ul>
            <li v-for="item in lis" :key="item.li">{{item.li}}</li>
        </ul>
        <p>
            Copyright&nbsp;&copy;&nbsp;{{author}} - 2016 All rights reserved
        </p>
    </cfooter>
</template>

<script>
export default {
  name: "cfooter",
  data() {
    return {
      lis: [
        { li: "琉璃之金" },
        { li: "朦胧之森" },
        { li: "缥缈之滔" },
        { li: "逍遥之火" },
        { li: "璀璨之沙" }
      ]
    };
  },
  computed: {
    author() {
      return this.$store.state.author;
    }
  }
};
</script>
