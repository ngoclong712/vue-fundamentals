<script setup>
    import { useToast } from 'vue-toastification';

    const toast = useToast();

    const showSuccess = () => {
        console.log('success clicked');
        toast.success('success');
    }

    const showError = () => {
        console.log('error clicked');
        toast.error('error');
    }
</script>

<template>
    <div class="p-6">
    <h1 class="text-2xl font-bold mb-4">Test Toast Page</h1>
    <button 
      class="px-4 py-2 bg-green-500 text-white rounded mr-4"
      @click="showSuccess"
    >
      Show Success
    </button>

    <button 
      class="px-4 py-2 bg-red-500 text-white rounded"
      @click="showError"
    >
      Show Error
    </button>
  </div>
</template>