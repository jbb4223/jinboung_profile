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
        <div class="profile-hero">
          <p class="eyebrow">Frontend Profile</p>
          <h2 class="section-title">사용자 경험을 고민하는 웹 개발자</h2>
          <p class="bio">
            Vue 기반의 반응형 UI 구현과 유지보수하기 쉬운 구조 설계를 좋아합니다.
            작은 인터랙션과 안정적인 화면 흐름을 통해 사용자가 편하게 느끼는 웹 서비스를 만드는 것을 목표로 합니다.
          </p>
        </div>

        <div class="summary-grid">
          <article class="summary-card">
            <span class="summary-number">Vue</span>
            <strong>주요 기술</strong>
            <p>컴포넌트 기반 UI 설계와 상태 흐름을 고려한 화면 개발</p>
          </article>

          <article class="summary-card">
            <span class="summary-number">UI</span>
            <strong>관심 영역</strong>
            <p>반응형 레이아웃, 접근성, 사용성을 고려한 인터페이스</p>
          </article>

          <article class="summary-card">
            <span class="summary-number">Clean</span>
            <strong>개발 방식</strong>
            <p>읽기 쉽고 확장 가능한 코드 구조와 꾸준한 개선</p>
          </article>
        </div>

        <section class="skill-section">
          <h3>Tech Stack</h3>
          <div class="skill-list">
            <span>Vue 3</span>
            <span>JavaScript</span>
            <span>HTML</span>
            <span>CSS</span>
            <span>Vite</span>
            <span>GitHub</span>
          </div>
        </section>

        <section class="focus-section">
          <h3>Now Focusing On</h3>
          <ul>
            <li>컴포넌트 재사용성과 화면 구조 개선</li>
            <li>모바일에서도 자연스러운 반응형 UI 구성</li>
            <li>작은 프로젝트를 꾸준히 완성하며 개발 경험 쌓기</li>
          </ul>
        </section>
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