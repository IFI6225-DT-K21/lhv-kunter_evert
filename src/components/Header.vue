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
        <b-button v-b-toggle.collapse-3 class="m-1">Sisene</b-button>

        <a href="/">EN</a>
        <a href="/">RU</a>
      </div>
    </div>
    <b-collapse class="formRow" visible id="collapse-3">
      <div class="formWrapper">
        <div class="formBlocks">
          <div class="formGroup">
            <b-form-radio-group
              id="btn-radios-1"
              v-model="selected"
              :options="options"
              :aria-describedby="ariaDescribedby"
              name="formButton"
              buttons
            ></b-form-radio-group>
          </div>
          <label for="inputPassword2" class="sr-only">Kasutajanimi</label>
          <input
            type="email"
            class="emailInput"
            id="inputPassword2"
            placeholder="Kasutajanimi"
          />
        </div>
        <button type="submit" class="loginButton">Sisene</button>
      </div>
    </b-collapse>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      selected: "radio1",
      options: [
        { text: "ID-kaart", value: "radio1" },
        { text: "Mobiil-ID", value: "radio2" },
        { text: "Smart-ID", value: "radio3" },
        { text: "PIN-kalkulaator", value: "radio4" },
        { text: "Salasõna", value: "radio5" },
      ],
    };
  },
};
</script>



<style lang="scss" scoped>
body {
  font-family: "Neue Helvetica W06", "Helvetica Neue", sans-serif;
  font-size: 16px;
  line-height: 26px;
  font-weight: 400;
  letter-spacing: 0;
}
.mainRow {
  position: relative;
  z-index: 1;
  padding-top: 20px;
  padding-bottom: 20px;
  background: #fff;
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
.formRow {
  display: flex;
  justify-content: center;

  width: 100%;
  border-bottom: 1px solid rgba(255, 255, 255, 0.9);
  background-color: rgba(243, 241, 241, 1);
}
.formWrapper {
  padding-top: 20px;
  padding-bottom: 20px;
}
.formBlocks {
  display: inline-block;
}
// .collapseWrapper {
//   position: relative;
//   width: 100%;
//   margin-top: 50px;
//   text-align: center;
// }
.emailInput {
  margin-right: 8px;
  margin-left: 12px;
  padding-left: 12px;
  width: 180px;
  height: 36px;
  font-size: 12px;
  font-weight: 500;
  line-height: 1.2;
  background-repeat: no-repeat;
  background-position: 7px center;
  border: 1px solid #c2c2c5;
  box-shadow: none;
  color: #00000f;
}
.loginButton {
  background-color: #3b3b47;
  color: white;
  border-radius: 5px;
  font-size: 14px;
  font-weight: 500;
  padding: 5px 16px !important;
}
.formGroup {
  display: inline-block;
  vertical-align: middle;
}

.formButton {
  padding: 0 12px;
  font-size: 12px;
  line-height: 30px;
  text-decoration: none;
  font-weight: 500;
  background-color: transparent;
  border-radius: 0;
  border-left: none;
  border-right: none;
  border-color: rgba(181, 181, 185, 1);
  color: black;
}
.formButtonFirst {
  border-top-left-radius: 5px !important;
  border-bottom-left-radius: 5px !important;
  padding: 0 12px;
  font-size: 12px;
  line-height: 30px;
  text-decoration: none;
  font-weight: 500;
  background-color: transparent;
  border-radius: 0;
  border-right: none;
  border-color: rgba(181, 181, 185, 1);
  color: black;
}
.formButtonLast {
  border-top-right-radius: 5px !important;
  border-bottom-right-radius: 5px !important;
  padding: 0 12px;
  font-size: 12px;
  line-height: 30px;
  text-decoration: none;
  font-weight: 500;
  background-color: transparent;
  border-radius: 0;
  border-left: none;
  border-color: rgba(181, 181, 185, 1);
  color: black;
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