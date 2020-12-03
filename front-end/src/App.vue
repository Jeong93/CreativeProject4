<template>
<div id="app">
  <div class="header">
    <router-link to="/">
      <div class="logo">
        <a href="http://creative4.jeonghaeng.org">
        <img src="/logo.jpg">
        </a>
      </div>
    </router-link>
    <div class="title">
      <h1>Manage Customers</h1>
    </div>
  </div>
  <div class="menu">
    <router-link class="router-link" to="/admin">Admin</router-link>
  </div>
  <div class="content">
    <router-view />
  </div>
  <div class="footer">
    <a href="/">gitHub link</a>
  </div>
</div>
</template>

<style>
html {
  box-sizing: border-box;
}

body {
  font-family: 'Montserrat', sans-serif;
  font-size: 16px;
  background: #fff;
  padding: 0px;
  margin: 0px;
}

/* Header */
.header {
  display: flex;
  padding: 10px 100px 0px 100px;
  background-color: #19224b;
  color: #fff;
}

.title {
  margin-top: 5px;
}

.title h1 {
  font-size: 30px;
  padding-left: 10px;
}

.content {
  padding: 20px 100px;
  min-height: 500px;
}

/* menu */
.menu {
  height: 50px;
  padding: 20px 100px 0px 100px;
  background: #19224b;
  font-size: 20px;
  text-decoration:none;
  color: white;
  border-top: 1px solid white;
}
.menu li {
  display: inline;
}

.router-link:link,
.router-link:visited,
a:visited {
  text-decoration: none;
  color: white;
}


.menu a {
  color: #000;
}

/* footer */
.footer {
  height: 50px;
  padding: 20px 100px 0px 100px;
  font-size: 12px;
  background:#19224b;
  color: #b5b829;
  text-decoration: none;
}

.footer:visited {
  color: #b5b829;
}
.footer a {
  text-decoration: none;
}
h1 {
  font-size: 20px;
}

h2 {
  font-size: 14px;
}
</style>
