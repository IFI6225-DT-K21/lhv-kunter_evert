<template>
  <div class="mainRow">
    <div id="dataRow">
      <div id="logoColumn">
        <img
          class="logo"
          src="https://upload.wikimedia.org/wikipedia/commons/b/be/Lhv-logo_2.svg"
        />
      </div>
      <div id="portalsColumn">
        <a style="font-weight: bold" href="/">PANK</a>
        <br />
        <a href="/">FINANTSPORTAAL</a>
        <br />
        <a href="/">INVESTOR</a>
        <br />
      </div>
      <div id="buttonsColumn">
        <a href="/">AVA KONTO</a>
        <a style="font-weight: bold" href="/">SISENE</a>
        <a href="/">EN</a>
        <a href="/">RU</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
.mainRow {
  height: 100px;
  position: relative;
  z-index: 1;
  padding-top: 20px;
  padding-bottom: 20px;
  background: #fff;
  height: 100px;
  width: 100%;
  text-transform: uppercase;
  font-size: 11px;
  line-height: 20px;
}
#dataRow {
  width: 970px;
  margin-left: auto;
  margin-right: auto;
}
#logoColumn {
  display: block;
  float: left;
}
#portalsColumn {
  display: block;
  float: left;
  text-align: left;
  line-height: 18px;
  margin-left: 15px;
}
#buttonsColumn {
  float: right;
  line-height: 60px;
  a {
    margin-left: 20px;
  }
}
a {
  text-decoration: none;
  color: black;
}
.logo {
  width: 84px;
  height: 100%;
}
</style>