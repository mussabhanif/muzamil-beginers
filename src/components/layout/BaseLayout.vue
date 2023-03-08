<script setup></script>

<template>
  <header class="bg-white shadow-sm flex flex-row items-center justify-between py-5">
    <!-- app logo -->
    <div>
      <img src="/favicon.ico" alt="" />
    </div>
    <!-- nav -->
    <nav>
      <ul class="flex flex-row items-center gap-3">
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
      </ul>
    </nav>
    <!-- actions -->
    <span>
      <slot name="header" />
    </span>
  </header>
  <!-- mian  -->
  <main class="flex">
    <slot> Hi i am default content.. </slot>
  </main>
  <footer>
    <slot name="footer" />
  </footer>
</template>
