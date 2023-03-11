<template>
  <div>
    <header>
      <slot name="header">
        <nav>
          <ul>
            <li>
              <NuxtLink to="/">Isndex</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/about">About</NuxtLink>
            </li>
          </ul>
        </nav>
      </slot>
    </header>
    <main>
      <slot />
    </main>
  </div>
</template>
<script setup>
const route = useRoute();

function getRoute() {
  return route.name;
}
</script>
