<script lang="ts">
// Минималистичный компонент портфолио
</script>

<section class="container">
  <header class="titlebar app-window-drag-handle">
    <span>Портфолио</span>
  </header>
  <section class="main-area">
    <div class="avatar">
      <img src="/app-icons/finder/256.png" alt="Portfolio Icon" class="avatar-img" />
    </div>
    <div class="info animated">
      <h1 class="name">Ашраф Рустамов</h1>
      <p class="age">Возраст: <b>21 год</b></p>
      <p class="edu">Образование: <b>Колледж Hexlet</b></p>
      <p class="role">Frontend developer</p>
      <div class="skills">
        <span class="tag js">JavaScript</span>
        <span class="tag ts">TypeScript</span>
        <span class="tag node">NodeJS</span>
        <span class="tag react">React</span>
        <span class="tag svelte">Svelte</span>
        <span class="tag sqlite">SQLite</span>
        <span class="tag python">Python</span>
      </div>
      <div class="links">
        <a href="https://github.com/Asgysygs" class="link github" target="_blank" rel="noopener" title="Github">
          <svg viewBox="0 0 24 24" width="28" height="28" fill="currentColor"><path d="M12 2C6.477 2 2 6.484 2 12.021c0 4.428 2.865 8.184 6.839 9.504.5.092.682-.217.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.342-3.369-1.342-.454-1.154-1.11-1.462-1.11-1.462-.908-.62.069-.608.069-.608 1.004.07 1.532 1.032 1.532 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.339-2.221-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.987 1.029-2.687-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.025A9.564 9.564 0 0 1 12 6.844c.85.004 1.705.115 2.504.337 1.909-1.295 2.748-1.025 2.748-1.025.546 1.378.203 2.397.1 2.65.64.7 1.028 1.594 1.028 2.687 0 3.847-2.337 4.695-4.566 4.944.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.749 0 .267.18.577.688.48C19.138 20.2 22 16.448 22 12.021 22 6.484 17.523 2 12 2z"></path></svg>
        </a>
        <a href="https://t.me/ashr009" class="link telegram" target="_blank" rel="noopener" title="Telegram">
          <svg viewBox="0 0 24 24" width="28" height="28" fill="currentColor"><path d="M12 2C6.477 2 2 6.477 2 12c0 5.523 4.477 10 10 10s10-4.477 10-10c0-5.523-4.477-10-10-10zm3.93 7.36l-1.43 6.77c-.11.48-.39.6-.78.37l-2.16-1.6-.98.94c-.11.11-.2.2-.41.2l.15-2.13 3.88-3.5c.17-.15-.04-.24-.26-.09l-4.8 3.02-2.07-.65c-.45-.14-.46-.45.09-.67l8.1-3.13c.37-.14.7.09.58.66z"></path></svg>
        </a>
      </div>
    </div>
  </section>
</section>

<style>
.container {
  background: linear-gradient(135deg, #f8fafc 0%, #e0e7ef 100%);
  border-radius: inherit;
  min-height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  box-shadow: 0 2px 24px 0 rgba(60,60,60,0.07);
  max-width: 600px;
  width: 100%;
}
.titlebar {
  display: flex;
  padding: 1rem 1rem;
  justify-content: center;
  width: 100%;
  border-bottom: 1px solid #e5e7eb;
  font-weight: 500;
  font-size: 1.1rem;
  color: #3b3b3b;
  background: transparent;
}
.main-area {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  flex: 1;
  width: 100%;
  padding: 3.5rem 1rem 0.5rem 1rem;
}
.avatar {
  margin-bottom: 1.5rem;
  display: flex;
  justify-content: center;
}
.avatar img {
  width: 96px;
  height: 96px;
  border-radius: 50%;
  box-shadow: 0 2px 16px 0 rgba(60,60,60,0.10);
  background: #fff;
  object-fit: cover;
}
.info {
  text-align: center;
}
.info h1 {
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
  color: #1a202c;
}
.info p {
  font-size: 1.1rem;
  margin: 0.2rem 0;
  color: #374151;
}
.info b {
  color: #2563eb;
  font-weight: 600;
}
.info .role {
  margin-top: 1.2rem;
  font-size: 1.15rem;
  color: #0ea5e9;
  font-weight: 600;
  letter-spacing: 0.5px;
}
.skills {
  margin-top: 1rem;
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  justify-content: center;
}
.avatar-img {
  transition: transform 0.3s cubic-bezier(.4,2,.6,1), box-shadow 0.3s;
  will-change: transform, box-shadow;
}
.avatar-img:hover {
  transform: scale(1.08) rotate(-3deg);
  box-shadow: 0 4px 32px 0 #38bdf8cc, 0 1px 8px 0 #2563eb44;
}
.animated {
  animation: fadeInUp 0.8s cubic-bezier(.4,2,.6,1);
}
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(32px) scale(0.98);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}
.name {
  transition: color 0.2s, text-shadow 0.2s;
  cursor: pointer;
}
.name:hover {
  color: #f59e42;
  text-shadow: 0 2px 16px #fbbf24cc, 0 1px 8px #f59e4244;
}
.tag {
  display: inline-block;
  padding: 0.3em 0.9em;
  border-radius: 1em;
  font-size: 0.98rem;
  font-weight: 500;
  background: #f3f4f6;
  color: #2563eb;
  box-shadow: 0 1px 4px 0 rgba(60,60,60,0.06);
  transition: background 0.25s, color 0.25s, transform 0.25s, box-shadow 0.25s;
  cursor: pointer;
  position: relative;
  z-index: 1;
}
.tag:hover, .tag:focus-visible {
  transform: scale(1.13) translateY(-2px) rotate(-2deg);
  box-shadow: 0 4px 24px 0 #2563eb44, 0 1px 8px 0 #38bdf8cc;
  filter: brightness(1.1) saturate(1.2);
  z-index: 2;
}
.tag.js { background: #f7df1e; color: #222; }
.tag.ts { background: #3178c6; color: #fff; }
.tag.node { background: #68a063; color: #fff; }
.tag.react { background: #61dafb; color: #222; }
.tag.svelte { background: #ff3e00; color: #fff; }
.tag.sqlite { background: #003b57; color: #7ad6fb; }
.tag.python { background: #3776ab; color: #fff; }
.links {
  margin-top: 1.5rem;
  display: flex;
  gap: 1.2rem;
  justify-content: center;
}
.link {
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f3f4f6;
  border-radius: 50%;
  width: 48px;
  height: 48px;
  color: #2563eb;
  box-shadow: 0 1px 8px 0 #2563eb22;
  transition: background 0.2s, color 0.2s, box-shadow 0.2s, transform 0.2s;
  font-size: 1.5rem;
}
.link.github:hover {
  background: #222;
  color: #f7df1e;
  box-shadow: 0 2px 16px 0 #222a;
  transform: scale(1.13) rotate(-6deg);
}
.link.telegram:hover {
  background: #229ed9;
  color: #fff;
  box-shadow: 0 2px 16px 0 #229ed9aa;
  transform: scale(1.13) rotate(6deg);
}
</style> 