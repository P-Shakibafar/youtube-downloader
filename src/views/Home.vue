<template>
  <div class="relative bg-gray-900 text-white flex-1 ml-56">
    <div class="absolute bottom-0 right-0 p-6">
      <button
        @click="open = true"
        class="bg-green-500 hover:bg-grey text-grey-darkest font-bold py-4 px-4 rounded-full inline-flex items-center"
      >
        <svg
          class="fill-current w-4 h-4"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          viewBox="0 0 512 512"
        >
          <path
            d="M492,236H276V20c0-11.046-8.954-20-20-20c-11.046,0-20,8.954-20,20v216H20c-11.046,0-20,8.954-20,20s8.954,20,20,20h216
			v216c0,11.046,8.954,20,20,20s20-8.954,20-20V276h216c11.046,0,20-8.954,20-20C512,244.954,503.046,236,492,236z"
          />
        </svg>
      </button>
    </div>
    <Modal :open="open" @close="open = false">
      <div class="max-w-lg w-full bg-gray-900 rounded-lg shadow-2xl px-6 py-6">
        <h2
          class="font-semibold text-white text-2xl leading-tight border-b-2 border-gray-200 pb-4"
        >Add Link</h2>
        <p
          class="mt-4 text-gray-100"
        >Are you absolutely sure you want to cancel your subscription and delete your account? This action cannot be undone.</p>
        <div class="mt-6">
          <button
            type="button"
            @click="open = false"
            class="px-4 py-2 text-white font-semibold bg-green-500 hover:bg-green-600 border border-transparent rounded focus:outline-none focus:shadow-outline"
          >Download</button>
          <button
            @click="open = false"
            class="ml-4 px-4 py-2 text-gray-800 font-semibold bg-white hover:bg-gray-100 border rounded focus:outline-none focus:shadow-outline"
          >Cancel</button>
        </div>
      </div>
    </Modal>
  </div>
</template>

<script>
import Modal from "../components/Modal";
export default {
  name: "Home",
  components: {
    Modal
  },
  data() {
    return {
      open: false
    };
  }
};
</script>
