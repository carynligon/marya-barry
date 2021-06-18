<template>
  <nav class="nav column container">
    <a href="/" class="home-link column"> <span>👋</span>Marya Barry </a>
    <ul class="nav-links column">
      <li>
        <a href="/bio">Bio</a>
      </li>
      <li>
        <a href="/reviews">Reviews</a>
      </li>
      <li>
        <a href="/photos">Photos</a>
      </li>
      <li>
        <a href="/resume">Resume</a>
      </li>
      <li>
        <a href="/contact">Contact</a>
      </li>
      <!-- <li>
        <a
          href="https://www.dropbox.com/s/k1ijp2npufbmeak/Derrick-Ligon-Resume.pdf?dl=0"
          target="_blank"
          >Resume</a
        >
      </li> -->
    </ul>
  </nav>
</template>

<style scoped>
.nav {
  --width: 12;
  align-items: center;
  display: flex;
  margin-top: var(--spacer-xl);
}
.home-link {
  --width: 9;
  color: var(--pink);
  font-size: var(--font-size-body-lg);
  font-weight: 600;
  text-decoration: none;
}
.home-link span {
  margin-right: 8px;
}
.nav-links {
  --width: 3;
  display: flex;
  justify-content: flex-end;
}
.nav-links li {
  margin: 0 0 0 2rem;
}
.nav-links li:first-of-type {
  margin-left: 0;
}
.nav-links a {
  color: var(--pink);
  text-decoration: none;
}
.nav-links a:hover {
  color: #43aa8b;
}
@media (max-width: 576px) {
  .nav-links {
    display: none;
  }
}
</style>
