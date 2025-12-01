<template>
  <div class="min-h-screen bg-gray-100">
    <header class="bg-blue-600 text-white p-4">
      <h1 class="text-xl">MyTask Dashboard</h1>
    </header>
    <main class="p-4">
      <h2 class="text-lg font-semibold">Your Tasks</h2>
      <ul class="list-disc pl-5">
        <li v-for="task in tasks" :key="task.id">{{ task.name }}</li>
      </ul>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tasks: [
        { id: 1, name: 'Task 1' },
        { id: 2, name: 'Task 2' },
        { id: 3, name: 'Task 3' }
      ]
    };
  }
};
</script>