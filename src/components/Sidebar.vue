 
<template>
  <div class="w-56 bg-gray-800 text-white border-r border-blackblack fixed min-h-screen pt-8">
    <div class="search-container text-left p-4">
      <p>GENERAL</p>
    </div>

    <div class="sidebar-icons">
      <router-link
        to="/"
        class="sidebar-icon flex items-center px-4 py-2 text-grey no-underline cursor-pointer hover:bg-grey-darker"
      >
        <svg
          fill="currentColor"
          class="mr-3"
          height="24px"
          viewBox="0 0 482.239 482.239"
          width="24px"
        >
          <path d="m0 447.793h482.239v34.446h-482.239z" />
          <path
            d="m396.091 223.863-24.287-24.354-113.462 113.462v-312.971h-34.446v312.971l-113.495-113.496-24.22 24.354 154.938 155.073z"
          />
        </svg>
        <div class="text-white">Downloading</div>
      </router-link>
      <!-- end sidebar-icon -->
    </div>
    <!-- end sidebar-icons -->
  </div>
</template>

<script>
export default {
  name: "Sidebar"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
