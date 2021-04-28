<template>
    <v-app>
        <app-navigation></app-navigation>

        <v-content transition="slide-x-transition">
            <router-view></router-view>
            <PendingUserList></PendingUserList>
        </v-content>
    </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';
import PendingUserList from '@/components/PendingUserList';
export default {
    name: 'App',
    components: {
        AppNavigation,
        PendingUserList
    }
};
</script>

<style>
</style>