<template>
  <div class="profile-page">
    <section class="profile-layout">
      <aside class="left-panel">
        <div class="avatar">J</div>
        <h1 class="name">{{ name }}</h1>
        <p class="role">Web Developer</p>

        <div class="actions">
          <a
              :href="gitHubUrl"
              target="_blank"
              rel="noopener noreferrer"
              class="icon-btn github-btn"
              aria-label="GitHub 홈페이지로 이동"
              title="GitHub"
          >
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path

                  fill="currentColor"
                  d="M12 .5a12 12 0 0 0-3.79 23.39c.6.11.82-.26.82-.58v-2.04c-3.34.73-4.04-1.42-4.04-1.42-.55-1.38-1.33-1.74-1.33-1.74-1.09-.74.08-.73.08-.73 1.2.09 1.84 1.25 1.84 1.25 1.08 1.84 2.82 1.31 3.5 1 .11-.78.42-1.31.76-1.61-2.66-.31-5.46-1.35-5.46-6 0-1.33.47-2.42 1.24-3.27-.13-.31-.54-1.57.12-3.26 0 0 1.01-.33 3.3 1.25a11.3 11.3 0 0 1 6 0c2.29-1.58 3.29-1.25 3.29-1.25.67 1.69.26 2.95.13 3.26.77.85 1.24 1.94 1.24 3.27 0 4.66-2.81 5.69-5.49 5.99.43.37.81 1.1.81 2.23v3.3c0 .32.22.7.83.58A12 12 0 0 0 12 .5Z"
              />
            </svg>
          </a>
        </div>
      </aside>

      <main class="right-panel">
        <h2 class="section-title">About</h2>
        <p class="bio">
          사용자 중심의 웹 서비스를 개발하는 웹개발자입니다.
          Vue 기반의 반응형 UI 구현, 성능 최적화, 유지보수하기 쉬운 구조 설계를 중요하게 생각합니다.
          문제를 빠르게 파악하고 안정적인 코드로 해결하는 것을 목표로 합니다.
        </p>
      </main>
    </section>
  </div>
</template>

<script setup>
import { ref } from "vue";

// 이름
const name = ref("JinBoung");
// gitHub 주소
const gitHubUrl = "https://github.com/jbb4223";
</script>