<template>
  <Head title="Users" />
    <h1 class="text-3xl">Users</h1>

  <ul>
    <li v-for="user in users" :key="user" v-text="user.name"></li>
  </ul>

    <!-- time and refresh button - showing prevent scrolling on load -->
    <!-- <div style="margin-top: 400px">
        <p>The current time is {{ time }}.</p>

        <div style="margin-top: 400px">
            <p>The current time is {{ time }}.</p>

            <Link href="/users" class="text-blue-500" preserve-scroll>
                Refresh
            </Link>
        </div>
        <Link href="/users" class="text-blue-500" preserve-scroll>
            Refresh
        </Link> 
    </div> -->
</template>

<script setup>
defineProps(['users'])
// defineProps(['time'])
</script>
