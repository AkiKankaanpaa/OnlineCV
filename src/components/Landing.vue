<script setup>
</script>

<template>
  <div class="content">
    <div class="avatar-row">
      <img class="avatar" src="../assets/images/portrait.png">
      <div class="me">
        <h1>Aki Kankaanpää</h1>
        <h2>Junior Developer and Information Technology Student</h2>
      </div>
    </div>

    <div class="about-row">
      <h3>Hello!</h3>
      <p>This website contains my resume and contact details, as well as a small compendium of my past projects,
        done for university courses or for my own enjoyment.
        The icons below lead to my personal Github account as well as my LinkedIn. I hope we will be in touch!
      </p>
    </div>
    <div class="info-row">
      <ul class="info">
        <li>
          <span class="title">Current Residence: </span>
          <span class="value">Tampere, Finland</span>
        </li>
        <li>
          <span class="title">Email: </span>
          <span class="value">aki.k.kankaanpaa@gmail.com</span>
        </li>
        <li>
          <span class="title">Phone: </span>
          <span class="value">+358 44 0903200</span>
        </li>
      </ul>
      <div>
        <a href="https://www.linkedin.com/in/samuli-kappi/" target="_blank"><img class="icon" src="../assets/images/linkedin.png" alt="linkedin"></a>
        <a href="https://github.com/SamuliKappi?tab=repositories" target="_blank"><img class="icon" src="../assets/images/github.png" alt="github"></a>
    </div>
    </div>
  </div>
</template>

<style scoped>
  .content {
    position: fixed;
    right: 30%;
    left: 30%;
    top: 10%;
  }
  .avatar-row {
    display: flex;
    align-items: center;
  }
  .about-row {
    margin-top: 20px;
  }
  .info { 
    list-style: none;
  }

  .info-row {
    display: flex;
    align-items: center;
  }

  .icon {
    height: 75px;
    width: 75px;
    margin-top: 10px;
  }
  a:hover {
    background: none;
  }
  .title {
    width: 100px;
  }
  .avatar {
    height: 200px;
    width: 200px;
    vertical-align: middle;
    margin-right: 20px;
  }
</style>