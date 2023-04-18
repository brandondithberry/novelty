<template>
  <div class="header w-full bg-white p-4">
    <div class="header-container flex mx-auto max-w-screen-xl justify-between items-center px-4 sm:px-6 lg:px-8">
      <div class="logo">
        <img src="img/logo.png" alt="Logo" class="h-8" />
      </div>
      <div class="menu">
        <!-- Use the hidden class on smaller screens -->
        <ul class="hidden sm:flex text-lg text-center justify-between items-center space-x-6 font-medium">
          <li><a href="#">Services</a></li>
          <li><a href="#">Work</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
        <!-- Add a mobile menu icon and a hidden menu list -->
        <button class="sm:hidden ml-auto">
          <svg class="w-6 h-6 fill-current" viewBox="0 0 24 24">
            <path
              d="M4 6h16M4 12h16M4 18h16"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
        <ul class="hidden absolute top-full right-0 bg-white shadow-lg text-lg text-center py-4 space-y-4 font-medium">
          <li><a href="#">Services</a></li>
          <li><a href="#">Work</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
          <a href="#" class="btn">Get Started</a>
        </ul>
      </div>
      <a href="#" class="btn text-base hidden sm:block">Get Started</a>
    </div>
  </div>
</template>

<style scoped>
.menu li a {
  @apply text-gray-500 hover:text-black;
}

.logo img {
  height: 40px;
}

/* Show the mobile menu list when the button is clicked */
.menu button:focus + ul,
.menu button:focus-within + ul {
  display: block;
}

/* Style the mobile menu list */
.menu ul {
  @apply left-0 z-50;
}
</style>
