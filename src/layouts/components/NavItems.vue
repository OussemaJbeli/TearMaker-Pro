<script setup>
import VerticalNavSectionTitle from '@/@layouts/components/VerticalNavSectionTitle.vue';
import VerticalNavGroup from '@layouts/components/VerticalNavGroup.vue';
import VerticalNavLink from '@layouts/components/VerticalNavLink.vue';
</script>

<template>
  <!-- 👉 Dashboards -->
  <VerticalNavSectionTitle
    :item="{
      heading: 'Dashboards',
    }"
  />
  <VerticalNavLink
    :item="{
      title: 'Dashboard',
      icon: 'ri-home-smile-line',
      to: '/dashboard',
    }"
  />
  <!-- 👉 User Interface -->
  <VerticalNavSectionTitle
    :item="{
      heading: 'User Interface',
    }"
  />
  <VerticalNavGroup
    :item="{
      title: 'My Lists',
      icon: 'ri-home-smile-line',
    }"
  >
    <VerticalNavLink
      :item="{
        title: 'Games',
        icon: 'ri-gamepad-line',
        to: '/:pathMatch(.*)*',
      }"
    />
    <VerticalNavLink
      :item="{
        title: 'Anime',
        icon: 'ri-bear-smile-line',
        to: '/:pathMatch(.*)*',
      }"
    />
    <VerticalNavLink
      :item="{
        title: 'Movies',
        icon: 'ri-clapperboard-line',
        to: '/:pathMatch(.*)*',
      }"
    />
    <VerticalNavLink
      :item="{
        title: 'Series',
        icon: 'ri-movie-2-line',
        to: '/:pathMatch(.*)*',
      }"
    />
    <VerticalNavLink
      :item="{
        title: 'Books',
        icon: 'ri-bookmark-line',
        to: '/:pathMatch(.*)*',
      }"
    />

  </VerticalNavGroup>

  <!-- 👉 User Profil -->
  <VerticalNavSectionTitle
    :item="{
      heading: 'User Profile',
    }"
  />

  <VerticalNavLink
    :item="{
      title: 'Account Settings',
      icon: 'ri-user-settings-line',
      to: '/account-settings',
    }"
  />

  <!-- 👉 Others -->
  <VerticalNavSectionTitle
    :item="{
      heading: 'Others',
    }"
  />
  <VerticalNavLink
    :item="{
      title: 'Documentation',
      icon: 'ri-article-line',
      href: '/:pathMatch(.*)*',
      target: '_blank',
    }"
  />
  <VerticalNavLink
    :item="{
      title: 'Raise Support',
      href: '/:pathMatch(.*)*',
      icon: 'ri-lifebuoy-line',
      target: '_blank',
    }"
  />
</template>
