<template>
  <div class="navbar">
    <div class="nav_container flex">
      <div class="logo">
        <a href="/">
          <img src="../assets/images/logo.png" alt="logo" />
        </a>
      </div>

      <nav>
        <ul class="flex">
          <li>
            <div class="dropdown">
              <a href="#">Semester</a>
              <ul class="dropdown-content">
                <li class="litag"><a href="#/firstsemester">First Sem</a></li>
                <li class="litag"><a href="#/firstsemester">Second Sem</a></li>
                <li class="litag"><a href="#/firstsemester">Third Sem</a></li>
                <li class="litag"><a href="#/firstsemester">Forth Sem</a></li>
                <li class="litag"><a href="#/firstsemester">Fifth Sem</a></li>
                <li class="litag"><a href="#/firstsemester">Sixth Sem</a></li>
              </ul>
            </div>
          </li>

          <li><a href="#/about">About </a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<style>
@import url("../Style/global.css");


.navbar {
  background-color: var(--primary-color);
  color: #fff;
  height: 70px;
}
.navbar ul {
  margin: 19px 25px;
}
.navbar a {
  color: #fff;
  padding: 0px 10px;
  margin: 0 5px;
  font-weight: 600;
}

.navbar a:hover {
  border-bottom: 2px solid white;
}

.navbar .flex {
  justify-content: space-around;
}

.nav_container img {
  width: 77px;
  height: 71px;
}
.dropdown-content {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  visibility: hidden;
  align-items: center;
  justify-content: center;
  position: absolute;
  top: 23px;
  right:  309px;
  color: whitesmoke;
  background-color: var(--primary-color);
  min-width: 182px;

  box-shadow: inset 0px 0px 15px 1px;
  border-radius: 12px;
  overflow: scroll;
  list-style-type: none;
}
.litag {
  background: none;
}
.dropdown-content li a {
  padding: 10px 17px;
  text-decoration: none;
  display: block;
  z-index: -65;
  text-decoration: none;
}

.dropdown-content a:hover  {
  opacity: 0.9;
}

.dropdown:hover .dropdown-content {
  visibility: visible;
}

.dropdown:hover .dropbutton {
  background-color: rgb(255, 255, 255);
}
.dropdown-content::-webkit-scrollbar {
  display: none;
}

@media(max-width:900px){
.dropdown-content{
    top: 22px;
    right:75px;
  }
}
</style>>