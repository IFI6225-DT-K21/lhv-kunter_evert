<template>
  <div class="mainRow">
    <div id="dataRow">
      <div id="logoColumn">
        <img class="logo" src="https://www.lhv.ee/assets/images/lhv-logo.svg" />
      </div>
      <div id="portalsColumn">
        <a class="activeLink" href="/">PANK</a>
        <br />
        <a href="/">FINANTSPORTAAL</a>
        <br />
        <a href="/">INVESTOR</a>
        <br />
      </div>
      <div id="buttonsColumn">
        <a href="/">AVA KONTO</a>
        <a v-b-toggle.collapse-3 class="collapseButton">SISENE</a>

        <a href="/">EN</a>
        <a href="/">RU</a>
      </div>
    </div>
    <b-collapse class="formRow" visible id="collapse-3">
      <div class="formWrapper">
        <div class="formBlocks">
          <div class="formGroup">
            <b-button-group>
              <b-button id="radioBtnID" class="radioBtn">ID-kaart</b-button>
              <b-button id="radioBtnMobile" class="radioBtn"
                >Mobiil-ID</b-button
              >
              <b-button id="radioBtnSmart" class="radioBtn">Smart-ID</b-button>
              <b-button id="radioBtnPin" class="radioBtn"
                >PIN-kalkulaator</b-button
              >
              <b-button id="radioBtnPass" class="radioBtn">Salasõna</b-button>
            </b-button-group>
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
    return {};
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
  padding-bottom: 0.5px;
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
.form-group {
  margin-bottom: 0 !important;
}
.radioBtn {
  padding: 10px 13px;
  font-weight: 500;
  font-size: 14px;
  background: transparent;
  border-left: none;
  border-right: none;
  border-color: rgba(181, 181, 185, 1);
}
#radioBtnID {
  border-left: 1px solid;
  border-left-color: rgba(181, 181, 185, 1);
}
#radioBtnPass {
  border-right: 1px solid;
  border-right-color: rgba(181, 181, 185, 1);
}
.radioBtn:hover {
  border-color: rgba(181, 181, 185, 1);
}
.radiobtn:focus {
  // background: rgba(181, 181, 185, 1) !important;
  box-shadow: none;
  border-color: rgba(181, 181, 185, 1);
  background: transparent !important;
}
.radiobtn:active {
  // background: rgba(181, 181, 185, 1) !important;
  box-shadow: none;
  background: transparent !important;
}
.collapseButton {
  text-decoration: none;
  font-size: 14px !important;
  cursor: pointer;
  border-radius: 5px;
  border: 1px solid;
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 15px;
  padding-right: 15px;
  background-color: rgba(45, 44, 55);
  color: white !important;
}

.not-collapsed {
  font-size: 12px !important;
  font-weight: 500;
  border: none;
  background-color: transparent;
  color: black !important;
}
.not-collapsed:hover {
  color: black;
}
.not-collapsed:active {
  border: none;
}

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
.btn-secondary {
  color: black !important;
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
  height: 50px;
  justify-items: center;
  align-items: center;
  display: flex;
  float: left;
}
#portalsColumn {
  display: block;
  float: left;
  text-align: left;
  line-height: 18px;
  margin-left: 15px;
}
#portalsColumn a:hover {
  color: gray;
  text-decoration: none;
}
.activeLink {
  font-weight: bold;
}
.activeLink:hover {
  color: initial !important;
}
#buttonsColumn {
  float: right;
  line-height: 60px;
  margin-bottom: 20px;
  a {
    text-decoration: none;
    color: black;
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
label {
  background: white !important;
}
</style>