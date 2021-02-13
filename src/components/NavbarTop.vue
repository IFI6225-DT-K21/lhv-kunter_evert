<template>
  <nav class="navWrap">
    <b-nav class="topNav">
      <div class="dropdown mr-1">
        <button
          type="button"
          class="btn btn-secondary"
          data-toggle="dropdown"
          aria-haspopup="true"
          aria-expanded="false"
        >
          IGAPÄEVAPANGANDUS
        </button>
        <div class="dropdown-menu">
          <div id="dropdownMenuOffset" class="container">
            <table class="table table-borderless">
              <thead>
                <tr>
                  <th scope="col">#</th>
                  <th scope="col">First</th>
                  <th scope="col">Last</th>
                  <th scope="col">Handle</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <th scope="row">1</th>
                  <td>Mark</td>
                  <td>Otto</td>
                  <td>@mdo</td>
                </tr>
                <tr>
                  <th scope="row">2</th>
                  <td>Jacob</td>
                  <td>Thornton</td>
                  <td>@fat</td>
                </tr>
                <tr>
                  <th scope="row">3</th>
                  <td colspan="2">Larry the Bird</td>
                  <td>@twitter</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
      <div class="dropdown mr-1">
        <button
          type="button"
          class="btn btn-secondary"
          id="dropdownMenuOffset"
          data-toggle="dropdown"
          aria-haspopup="true"
          aria-expanded="false"
          data-offset="10,20"
        >
          RAHA KASVATAMINE
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuOffset">
          <table class="table table-borderless">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">First</th>
                <th scope="col">Last</th>
                <th scope="col">Handle</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">1</th>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
              </tr>
              <tr>
                <th scope="row">2</th>
                <td>Jacob</td>
                <td>Thornton</td>
                <td>@fat</td>
              </tr>
              <tr>
                <th scope="row">3</th>
                <td colspan="2">Larry the Bird</td>
                <td>@twitter</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
      <div class="dropdown mr-1">
        <button
          type="button"
          class="btn btn-secondary"
          id="dropdownMenuOffset"
          data-toggle="dropdown"
          aria-haspopup="true"
          aria-expanded="false"
          data-offset="10,20"
        >
          LAEN JA LIISING
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuOffset">
          <table class="table table-borderless">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">First</th>
                <th scope="col">Last</th>
                <th scope="col">Handle</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">1</th>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
              </tr>
              <tr>
                <th scope="row">2</th>
                <td>Jacob</td>
                <td>Thornton</td>
                <td>@fat</td>
              </tr>
              <tr>
                <th scope="row">3</th>
                <td colspan="2">Larry the Bird</td>
                <td>@twitter</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
      <div class="dropdown mr-1">
        <button
          type="button"
          class="btn btn-secondary"
          id="dropdownMenuOffset"
          data-toggle="dropdown"
          aria-haspopup="true"
          aria-expanded="false"
          data-offset="10,20"
        >
          PENSION
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuOffset">
          <table class="table table-borderless">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">First</th>
                <th scope="col">Last</th>
                <th scope="col">Handle</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">1</th>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
              </tr>
              <tr>
                <th scope="row">2</th>
                <td>Jacob</td>
                <td>Thornton</td>
                <td>@fat</td>
              </tr>
              <tr>
                <th scope="row">3</th>
                <td colspan="2">Larry the Bird</td>
                <td>@twitter</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
      <b-nav-item id="my-nav-dropdown">VAJAD ABI? </b-nav-item>
    </b-nav>
  </nav>
</template>

<script>
import "bootstrap/dist/css/bootstrap.min.css";
import "jquery/src/jquery.js";
import "bootstrap/dist/js/bootstrap.min.js";
export default {
  name: "NavbarTop",
};
</script>

<style lang="scss" scoped>
.navWrap {
  box-shadow: 0 1px 2px rgb(0 0 0 / 10%);
  z-index: 101;
  display: flex;
  justify-content: center;
  width: 100%;
  background-color: rgba(243, 241, 241, 1);
}
.container {
  width: 970px;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
  display: block;
}
.dropdown-menu {
  margin-top: 15px;
  z-index: 1000;
  padding-bottom: 20px;
  left: 0;
  right: 0;
  background: none;
  border: 0;
  box-shadow: none;
  float: left;
}
nav {
  .btn,
  a {
    padding-top: 19px !important;
    padding-bottom: 17px !important;
    padding-left: 12px !important;
    padding-right: 12px !important;
    color: #00000f !important;
    background-color: transparent;
    font-size: 13px;
    border: none;
    line-height: 13px;
    font-weight: 600;
    text-transform: uppercase;
    text-decoration: none;
  }

  .btn:active:focus {
    background: transparent;
    border: none;
    box-shadow: none !important;
  }
  .btn-secondary:focus {
    box-shadow: none;
  }
}
</style>