<template>
  <div class="min-h-screen flex items-center justify-center bg-gray-100">
    <div class="bg-white shadow-lg rounded-2xl p-8 w-full max-w-sm">
      <h1 class="text-2xl font-bold mb-6 text-center">Login</h1>

      <form @submit.prevent="login">
        <div class="mb-4">
          <label class="block text-gray-700 mb-1">Username</label>
          <input
            v-model="username"
            type="text"
            class="w-full border rounded-lg px-3 py-2 focus:outline-none focus:ring focus:ring-blue-300"
            placeholder="Masukkan username"
            required
          />
        </div>

        <div class="mb-6">
          <label class="block text-gray-700 mb-1">Password</label>
          <input
            v-model="password"
            type="password"
            class="w-full border rounded-lg px-3 py-2 focus:outline-none focus:ring focus:ring-blue-300"
            placeholder="Masukkan password"
            required
          />
        </div>

        <button
          type="submit"
          class="w-full bg-blue-500 text-white font-semibold py-2 rounded-lg hover:bg-blue-600"
        >
          Login
        </button>
      </form>

      <p v-if="error" class="text-red-500 text-center mt-4">{{ error }}</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { useRouter } from 'vue-router'

const username = ref('')
const password = ref('')
const error = ref('')
const router = useRouter()

const login = () => {
  // contoh login sederhana
  if (username.value === 'admin' && password.value === '1234') {
    localStorage.setItem('loggedIn', 'true')
    router.push('/dashboard')
  } else {
    error.value = 'Username atau password salah!'
  }
}
</script>

<style scoped>
body {
  font-family: 'Poppins', sans-serif;
}
</style>
