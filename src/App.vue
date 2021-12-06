<template>
  <img landingimg src="./assets/kid.png" />
  <div container>
    <p title v-text="name" />
    <div socials>
      <a ml-auto href="http://google.com">TIKTOK</a>
      <a href="http://google.com">INSTAGRAM</a>
      <a ml-auto href="http://google.com">SPOTIFY</a>
    </div>
    <p v-text="description" />
  </div>
</template>
<script>
  export default {
    name: 'App',
    data: () => ({
      url: "https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxjb2xsZWN0aW9uLXBhZ2V8MXw3NjA4Mjc3NHx8ZW58MHx8fHw%3D&w=1000&q=80",
      name: 'SWIXZY PIXXI',
      description: "LOREM IPSUM IS PRIMARY DUMMY TEXT OF THE PRINTING AND TYPESETTINGS INDUSTRY.",
  })
  }
</script>

<style>
  body {
    background: #a0c8d8;
    color: #000;
    font-family: 'Courier';
    font-weight: bolder;
    font-size: 20px;
    margin: 0;
  }
  [landingimg] {
    position: absolute;
    width: 80%;
    margin: 25vh 10% 0;
    border-radius: 50%;
  }
  [container] {
    box-sizing: border-box;
    position: relative;
    padding: 30px 20px 0;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
  [title] {
    font-size: 100px;
    color: #d350d8;
    margin: 0;
  }
  [socials] {
    margin-top: auto;
    display: flex;
    flex-direction: column;
  }
  a {
    font-size: 40px;
    width: fit-content;
    color: #000;
    border: 5px solid #000;
    border-radius: 10px;
    text-decoration: none;
    padding: 10px 30px;
    margin-bottom: 10px;
  }
  [ml-auto] {
    margin-left: auto;
  }
</style>
