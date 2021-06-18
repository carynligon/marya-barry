<template>
  <nav class="footer-nav column container">
    <ul class="column social-links">
      <li>
        <a
          href="https://www.instagram.com/makeupwithmarya/?hl=en"
          target="_blank"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
          >
            <path
              d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"
            />
          </svg>
        </a>
      </li>
      <li>
        <a
          href="https://www.linkedin.com/in/marya-barry-5a657494/"
          target="_blank"
        >
          <svg
            width="24px"
            height="24px"
            viewBox="0 0 24 24"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
          >
            <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
              <g transform="translate(-1256.000000, -2408.000000)">
                <g transform="translate(0.000000, 2350.000000)" fill="#FFFFFF">
                  <rect x="0" y="0" width="1440" height="140" />
                </g>
                <g
                  class="icon-color"
                  transform="translate(1218.000000, 2408.000000)"
                  fill="#000000"
                  fill-rule="nonzero"
                >
                  <g transform="translate(38.000000, 0.000000)">
                    <path
                      d="M22.21,-3.2822406e-05 L1.79,-3.2822406e-05 C0.822252831,-0.0058182675 0.0271669105,0.762616728 0,1.73 L0,22.2 C0.0218553219,23.1697164 0.820102131,23.9412063 1.79,23.9301206 L22.21,23.9301206 C23.1798979,23.9412063 23.9781447,23.1697164 24,22.2 L24,1.73 C23.9728331,0.762616728 23.1777472,-0.0058182675 22.21,-3.2822406e-05 Z M7.11,20.41 L3.59,20.41 L3.59,9 L7.11,9 L7.11,20.41 Z M5.39,7.41 C4.26601551,7.41032794 3.34714934,6.5136566 3.32,5.39 C3.30021611,4.83517317 3.51194502,4.29708732 3.90451617,3.90451617 C4.29708732,3.51194502 4.83517317,3.30021611 5.39,3.32 C6.47480091,3.39553578 7.31621196,4.29757245 7.31621196,5.385 C7.31621196,6.47242755 6.47480091,7.37446422 5.39,7.45 L5.39,7.41 Z M20.48,20.34 L17,20.34 L17,14.76 C17,13.43 17,11.7 15.14,11.7 C13.28,11.7 13,13.16 13,14.63 L13,20.28 L9.44,20.28 L9.44,9 L12.76,9 L12.76,10.5 L12.83,10.5 C13.523693,9.29528214 14.8312251,8.57787513 16.22,8.64 C19.81,8.64 20.48,11.04 20.48,14.09 L20.48,20.34 Z"
                    />
                  </g>
                </g>
              </g>
            </g>
          </svg>
        </a>
      </li>
    </ul>
    <div class="coolest-person-ever column">
      👩‍💻 Website built by
      <a href="http://carynligon.com" target="_blank">Caryn Ligon</a>
    </div>
  </nav>
</template>

<style scoped>
.footer-nav {
  --width: 12;
  align-items: center;
  flex-direction: row-reverse;
  margin-top: 7.5rem;
  margin-bottom: var(--spacer-xl);
  padding-left: 0;
}
.coolest-person-ever {
  --width: 10;
}
.coolest-person-ever a {
  text-decoration: none;
}
.coolest-person-ever a:hover {
  text-decoration: underline;
}
.social-links {
  --width: 2;
  display: flex;
  justify-content: flex-end;
}
.social-links svg {
  display: block;
}
.social-links li {
  align-items: center;
  display: flex;
  margin: 0 var(--spacer-xs);
}
.social-links li:first-of-type {
  margin-left: 0;
}
.social-links img {
  height: 1.5rem;
  width: 1.5rem;
}
.icon-color {
  fill: var(--black);
}
svg:hover .icon-color {
  fill: var(--links);
}
@media (max-width: 768px) {
  .coolest-person-ever {
    --width: 8;
  }
  .social-links {
    --width: 4;
  }
}
@media (max-width: 576px) {
  .footer-nav {
    margin-top: var(--spacer-3xl);
  }
  .coolest-person-ever,
  .social-links {
    justify-content: center;
    margin: 0 auto;
    text-align: center;
    --width: 12;
  }
  .social-links {
    margin-bottom: var(--spacer-sm);
  }
}
</style>
