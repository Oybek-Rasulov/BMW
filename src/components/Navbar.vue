<template>
  <div class="container">
    <nav class="navbar opacity-40">
      <!-- Links -->
      <div class="navbar-menu">
        <a href="#" class="logo-link">
          <img src="../assets/logo.png" alt="Company Logo">
        </a>
        <ul>
          <li><a href="#" class="current">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Product</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </div>

      <!-- Register -->
      <div class="navbar-auth">
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 -960 960 960" width="48px" fill="#F3F3F3"><path d="M222-255q63-44 125-67.5T480-346q71 0 133.5 23.5T739-255q44-54 62.5-109T820-480q0-145-97.5-242.5T480-820q-145 0-242.5 97.5T140-480q0 61 19 116t63 109Zm257.81-195q-57.81 0-97.31-39.69-39.5-39.68-39.5-97.5 0-57.81 39.69-97.31 39.68-39.5 97.5-39.5 57.81 0 97.31 39.69 39.5 39.68 39.5 97.5 0 57.81-39.69 97.31-39.68 39.5-97.5 39.5Zm.66 370Q398-80 325-111.5t-127.5-86q-54.5-54.5-86-127.27Q80-397.53 80-480.27 80-563 111.5-635.5q31.5-72.5 86-127t127.27-86q72.76-31.5 155.5-31.5 82.73 0 155.23 31.5 72.5 31.5 127 86t86 127.03q31.5 72.53 31.5 155T848.5-325q-31.5 73-86 127.5t-127.03 86Q562.94-80 480.47-80Zm-.47-60q55 0 107.5-16T691-212q-51-36-104-55t-107-19q-54 0-107 19t-104 55q51 40 103.5 56T480-140Zm0-370q34 0 55.5-21.5T557-587q0-34-21.5-55.5T480-664q-34 0-55.5 21.5T403-587q0 34 21.5 55.5T480-510Zm0-77Zm0 374Z"/></svg></a>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  setup() {
        
 },
}
</script>

<style scoped>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    /* animation */
    animation-name: menu;
    animation-duration: 1.5s;
    
  }

  @keyframes menu {
    0% {
      transform: translateY(-50px);
      opacity: 0;
    } 100% {
      transform: translateY(0);
      opacity: 1;
    }
  }

  .navbar-menu {
    display: flex;
    align-items: center;
  }

  .navbar-menu ul li:first-child {
    margin-left: 3rem;
  }

  .navbar-menu ul li {
    display: inline-block;
    margin-left: 1rem;
  }

  .navbar-menu ul li a {
    padding: 1rem 2rem;
    border: 2px solid #fff;
    border-radius: 50px;
  }

  .navbar-menu ul li a:hover {
    background-color: #fff;
    color: #333;
    transition: background 0.2s ease-in;
  }

  .navbar-menu img {
    width: 100px;

  }
</style>
