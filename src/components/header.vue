<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="col-md-12 col-sm-12 col-lg-12 col-xl-3">
          <div class="logo">
            <a
              href="/"
              title="logo"
              style="font-family: 'Mrs Saint Delafield', cursive"
            >
              Smart Learning
            </a>
          </div>
          <div class="mob-menu">
            <span>
              <i class="fa fa-bars"></i>
            </span>
          </div>
        </div>
        <div class="col-md-12 col-sm-12 col-lg-12 col-xl-9">
          <div class="main-menu">
            <ul class="nav">
              <li>
                <a href="/"> Home </a>
              </li>
              <li>
                <div
                  class="dropdown"
                  style="background-color: #ffeed5 !important"
                >
                  <button
                    style="background-color: #ffeed5 !important"
                    class="dropbtn"
                  >
                    Menu
                  </button>
                  <div class="dropdown-content">
                    <a><router-link to="/alphabets">Alphabets</router-link></a>
                    <a><router-link to="/vehicles">Vehicles</router-link></a>
                    <a><router-link to="/flowers">Flowers</router-link></a>
                    <a><router-link to="/animals">Animals</router-link></a>
                  </div>
                </div>
              </li>
              <li><a href="#"> About </a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  name: "headerComponent",
};
</script>
<style>
.dropbtn {
  /* background-color: #4caf50; */
  color: rgb(0, 0, 0);
  padding: 16px;
  font-size: 20px;
  border: none;
  cursor: pointer;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #ffeed5;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 10px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {
  background-color: #f1f1f1;
}

.dropdown:hover .dropdown-content {
  display: block;
}

/* Header start*/
header {
  transition: all 0.3s ease-in-out;
  box-shadow: 0 1px 6px 0 rgba(214, 220, 239, 1);
  top: 0px !important;
  background-color: #ffeed5;
  position: sticky;
  z-index: 2;
  height: auto;
}
.logo {
  padding: 26px 0px;
}
.logo a {
  color: #111317;
  text-transform: capitalize;
  color: #000000;
  font-size: 35px;
  font-weight: 500;
  text-decoration: none;
}
.mob-menu {
  display: none;
}
.main-menu {
  margin: 20px 0px;
  float: right;
}
.main-menu ul.nav {
  float: left;
  margin-right: 20px;
  list-style: none;
  padding-left: 0px;
  margin-bottom: 0px;
  padding-top: 10px;
}
.nav li:first-child {
  margin-left: 0px;
}
.main-menu ul {
  display: inline-block;
}
.main-menu ul li {
  position: relative;
  display: inline-block;
  margin: 12px 20px;
}
.main-menu ul li a {
  font-size: 20px;
  font-weight: 500;
  line-height: 1.3;
  color: #111317;
  display: block;
  text-decoration: none;
}
.main-menu ul.right-nav {
  padding-left: 0px;
}
.main-menu ul.right-nav li a {
  width: 150px;
  height: 40px;
  border-radius: 4px;
  background-color: #fff;
  text-align: center;
  color: #111317;
  border: solid 1px #111317;
  vertical-align: middle;
  display: table-cell;
}
.main-menu ul.right-nav li:last-child {
  margin-right: 0px;
}
.main-menu ul.right-nav li.active a {
  background-color: #111317;
  color: #fff;
}
@media (max-width: 1000px) {
  .logo {
    display: inline-block;
    width: 78%;
    padding: 10px 10px 10px 0px;
  }
  .mob-menu {
    display: inline-block;
    width: 20%;
  }
  .mob-menu span {
    border: solid 2px #111317;
    display: block;
    text-align: center;
    border-radius: 4px;
    padding: 2px 6px;
    width: 50px;
    color: #111317;
    font-size: 25px;
    cursor: pointer;
  }
  .main-menu {
    margin: 0px 0px 20px 0px;
    float: left;
    background-color: #f1f1f1;
    width: 100%;
    display: none;
  }
  .main-menu ul {
    list-style: none;
    padding-left: 0px;
    margin-bottom: 0px;
    width: 100%;
  }
  .main-menu ul.right-nav {
    text-align: center;
    margin-top: 6px;
  }
  ul.right-nav {
    margin-bottom: 10px;
  }
  .main-menu {
    margin: 0px 0px 20px 0px;
    float: left;
    background-color: #f1f1f1;
    width: 100%;
    display: none;
  }
  .main-menu ul li {
    display: block;
    width: 100%;
    margin: 0px;
  }
  .nav li:first-child {
    margin-left: 0px;
  }
  .main-menu ul li a {
    padding: 10px 15px;
    display: block;
    border-bottom: solid 1px #e2e4e6;
    text-align: center;
  }
  .main-menu ul.right-nav li {
    margin-left: 0px;
    margin-right: 30px;
    display: inline-block;
    width: 150px;
  }
  .main-menu ul.right-nav li a {
    font-size: 18px !important;
  }
}
/* header end */
</style>