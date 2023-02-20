<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <nav class="navbar bg-body-tertiary fixed-top">
    <div class="container-fluid d-flex align-items-center">
      <a class="navbar-brand" href="#"><span class="logo">Logo</span></a>
      <ul class="topMenu mt-3">
        <RouterLink class="link p-1 text-white" to="/">Home</RouterLink>
        <RouterLink class="link p-1 text-white" to="/about">About</RouterLink>
        <RouterLink class="link p-1 text-white" to="/project">Projects</RouterLink>
        <RouterLink class="link p-1 text-white" to="/contact">Contact</RouterLink>
      </ul>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="offcanvas"
        data-bs-target="#offcanvasNavbar"
        aria-controls="offcanvasNavbar"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="offcanvas offcanvas-start"
        tabindex="-1"
        id="offcanvasNavbar"
        aria-labelledby="offcanvasNavbarLabel"
      >
        <div class="offcanvas-header">
          <h3 class="offcanvas-title" id="offcanvasNavbarLabel"><span class="logo">Logo</span></h3>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
          ></button>
        </div>
        <div class="offcanvas-body">
          <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
            <li class="nav-item">
              <a class="nav-link active p-1 text-white" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link p-1 text-white" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link p-1 text-white" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link p-1 text-white" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link p-1 text-white" href="#">Link</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
  <RouterView />
</template>

<style>

</style>
