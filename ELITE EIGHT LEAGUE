:root{
  /* sensible defaults — override these in your theme if you already set them */
  --bg: linear-gradient(180deg,#07080a,#0b0d10);
  --text: #e9e6de;
  --muted: #9da0a6;
  --gold: #d8b45a;
  --gold2: #f4dc96;
  --line: rgba(255,255,255,.04);
  --tap: 44px;
}

/* global box-sizing (include pseudo elements) */
*, *::before, *::after {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body{
  margin: 0;
  background: radial-gradient(ellipse at 50% -10%, #302613 0, transparent 42%), var(--bg);
  color: var(--text);
  font-family: Inter, system-ui, -apple-system, "Segoe UI", Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -webkit-tap-highlight-color: transparent;
}

a {
  text-decoration: none;
  color: inherit;
}

button, input {
  font: inherit;
}

button {
  cursor: pointer;
  touch-action: manipulation;
}

.wrap {
  max-width: 1200px;
  margin: 0 auto;
  padding: 18px;
}

.btn {
  border: 1px solid var(--gold);
  background: linear-gradient(135deg, #f4dc96, #b78b2c);
  color: #171208;
  border-radius: 8px;
  font-weight: 800;
  min-height: var(--tap);
  padding: 8px 12px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
}

.btn.ghost {
  background: transparent;
  color: var(--text);
  border-color: rgba(255,255,255,.12);
}

.small {
  padding: 6px 8px;
  font-size: 13px;
}

.full {
  width: 100%;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 12px;
  padding: 12px 0;
  border-bottom: 1px solid #ffffff12;
  position: relative;
}

.brand {
  display: flex;
  align-items: center;
  gap: 12px;
}

.mark {
  width: 46px;
  height: 46px;
  display: grid;
  place-items: center;
  border: 1px solid var(--gold);
  color: var(--gold);
  font-weight: 900;
  border-radius: 10px;
}

.nav {
  display: flex;
  align-items: center;
  gap: 14px;
  color: var(--muted);
  font-size: 13px;
}

.nav a {
  padding: 8px 6px;
  border-radius: 8px;
}

.nav a:hover {
  color: var(--gold2);
}

#menuToggle {
  display: none;
}

.menu-icon {
  display: inline-block;
  width: 22px;
  height: 16px;
  position: relative;
}

/* pseudo elements carry the content property — normal span gets the same layout but content does nothing for it */
.menu-icon::before,
.menu-icon::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--text);
  border-radius: 2px;
}

.menu-icon::before { top: 0; }
.menu-icon span {
  position: absolute;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--text);
  border-radius: 2px;
  top: 7px;
}
.menu-icon::after { bottom: 0; }

.hero{
  display: grid;
  grid-template-columns: 1.2fr .8fr;
  gap: 20px;
  align-items: center;
  padding: 28px 0 18px;
  position: relative;
}

.hero h1{
  font-size: clamp(36px, 6vw, 72px);
  line-height: .96;
  margin: 8px 0;
}

.eyebrow{
  font-size: 11px;
  letter-spacing: 3px;
  color: var(--gold);
  font-weight: 800;
}

.small-muted{
  color: var(--muted);
  line-height: 1.7;
}

.hero-actions{
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
  margin-top: 14px;
}

.stats{
  display: flex;
  gap: 20px;
  margin-top: 18px;
  flex-wrap: wrap;
}

.stat strong{
  display: block;
  font-size: 18px;
}

.stat small{
  color: var(--muted);
  font-size: 11px;
}

.cup-scene{
  position: relative;
  width: min(320px, 82vw);
  height: 300px;
  margin: auto;
  display: grid;
  place-items: center;
  filter: drop-shadow(0 18px 24px rgba(0,0,0,.5));
}

.cup-scene::before{
  content: "";
  position: absolute;
  inset: 10% 10% 8%;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(216,180,90,.18), transparent 62%);
  filter: blur(16px);
  z-index: 0;
}

.trophy{
  width: min(240px, 80%);
  z-index: 2;
  animation: tFloat 4.2s ease-in-out infinite;
}

@keyframes tFloat{
  0%,100%{ transform: translateY(0) rotate(0deg); }
  50%{ transform: translateY(-12px) rotate(3deg); }
}

.orb, .ring, .spark { position: absolute; }

.orb{
  border-radius: 50%;
  border: 1px solid rgba(216,180,90,.25);
  filter: blur(9px);
  animation: orbPulse 5s ease-in-out infinite;
}

.orb-1{
  width: 220px;
  height: 220px;
  top: 18px;
  left: 20px;
  background: radial-gradient(circle, rgba(216,180,90,.10), transparent 60%);
}

.orb-2{
  width: 170px;
  height: 170px;
  top: 44px;
  left: 58px;
  background: radial-gradient(circle, rgba(216,180,90,.08), transparent 58%);
  animation-delay: .6s;
}

.orb-3{
  width: 120px;
  height: 120px;
  top: 58px;
  right: 26px;
  background: radial-gradient(circle, rgba(255,225,135,.12), transparent 55%);
  animation-delay: 1.4s;
}

@keyframes orbPulse{
  0%,100%{ transform: scale(1); opacity: .35; }
  50%{ transform: scale(1.08); opacity: .8; }
}

.ring{
  border-radius: 50%;
  border: 1px solid rgba(216,180,90,.28);
  animation: ringRotate 9s linear infinite;
}

.ring-1{
  width: 250px;
  height: 250px;
  top: 10px;
  left: 18px;
}

.ring-2{
  width: 190px;
  height: 190px;
  top: 42px;
  left: 46px;
  animation-direction: reverse;
  animation-duration: 12s;
}

@keyframes ringRotate{
  0%{ transform: rotate(0deg) scale(1); }
  50%{ transform: rotate(180deg) scale(1.03); }
  100%{ transform: rotate(360deg) scale(1); }
}

.spark{
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: radial-gradient(circle, #fff9d6 0%, #d8b45a 45%, rgba(216,180,90,0) 70%);
  box-shadow: 0 0 18px rgba(255,235,155,.8);
  animation: sparkle 3.2s ease-in-out infinite;
}

.spark-1{ top: 28px; left: 58px; animation-delay: .1s; }
.spark-2{ top: 50px; right: 52px; animation-delay: 1s; }
.spark-3{ bottom: 34px; left: 74px; animation-delay: 1.7s; }
.spark-4{ bottom: 24px; right: 70px; animation-delay: 2.2s; }

@keyframes sparkle{
  0%,100%{ transform: scale(.6); opacity: .5; }
  50%{ transform: scale(1.35); opacity: 1; }
}

.section{ margin-top: 20px; }

.section-head{
  display: flex;
  justify-content: space-between;
  align-items: end;
  gap: 12px;
  margin: 18px 0 12px;
}

.section-head h2{ margin: 4px 0 0; font-size: 28px; }
.section-head small{ letter-spacing: 2px; color: var(--gold); font-weight: 800; }

.team-grid{
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
}

.team-card, .panel{
  background: linear-gradient(145deg, #151820, #0e1015);
  border: 1px solid var(--line);
  border-radius: 12px;
  padding: 14px;
}

.team-top{
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 10px;
}

.badge{
  width: 64px;
  height: 64px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  background: #090a0d;
  border: 1px dashed #79663a;
  color: var(--gold);
  font-weight: 900;
  overflow: hidden;
}

.badge img{ width: 100%; height: 100%; object-fit: contain; }

.upload{
  display: inline-block;
  margin-top: 8px;
  color: var(--gold2);
  cursor: pointer;
  padding: 10px 12px;
  border-radius: 10px;
  border: 1px solid rgba(255,255,255,.04);
  font-weight: 700;
}

.upload input{ display: none; }

.match-list{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
}

.match{
  display: grid;
  grid-template-columns: 1fr auto 1fr;
  align-items: center;
  gap: 10px;
  padding: 12px;
  border-radius: 10px;
  border: 1px solid #252933;
  background: #0a0c10;
}

.club{ display: flex; align-items: center; gap: 8px; min-width: 0; }
.club.away{ flex-direction: row-reverse; text-align: right; }

.club-name{ font-size: 12px; font-weight: 800; }

.mini-badge{
  width: 30px;
  height: 30px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  font-size: 10px;
  font-weight: 900;
  background: #090a0d;
  border: 1px solid #5d4e2b;
  color: var(--gold);
  overflow: hidden;
}

.mini-badge img{ width: 100%; height: 100%; object-fit: contain; }

.score{ display: flex; align-items: center; gap: 6px; }

.score input{
  width: 54px;
  height: 40px;
  text-align: center;
  border: 1px solid #424650;
  border-radius: 8px;
  background: #171a21;
  color: var(--text);
  font-weight: 900;
  font-size: 15px;
}

.score input[disabled]{ opacity: .6; }

.status{ font-size: 10px; color: var(--muted); text-align: center; margin-top: 6px; }

.table-wrap{ overflow-x: auto; -webkit-overflow-scrolling: touch; }

table{
  width: 100%;
  border-collapse: collapse;
  min-width: 640px;
}

th, td{
  padding: 10px;
  border-bottom: 1px solid #252933;
  text-align: center;
  font-size: 13px;
}

th{ color: var(--gold2); background: #ffffff04; }
td:first-child, th:first-child{ text-align: left; }

.rank{ color: var(--gold); font-weight: 900; }

.pill{
  border: 1px solid rgba(216,180,90,.25);
  color: var(--gold2);
  padding: 6px 10px;
  border-radius: 999px;
  font-size: 12px;
}

.champion-box{
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 24px 18px;
  border: 1px solid rgba(216,180,90,.35);
  background: radial-gradient(circle at center, rgba(216,180,90,.08), rgba(18,20,24,.8) 45%, rgba(8,9,12,1) 100%);
}

.champion-cup{
  font-size: 58px;
  line-height: 1;
  filter: drop-shadow(0 8px 18px rgba(216,180,90,.35));
  margin-bottom: 8px;
}

#championName{ margin: 10px 0 6px; font-size: clamp(24px, 3vw, 36px); }
#championMeta{ font-size: 14px; }

.champion-row{
  background: linear-gradient(90deg, rgba(216,180,90,.08), rgba(255,255,255,0.02));
  border-left: 3px solid rgba(216,180,90,.8);
}

.hidden{ display: none !important; }

.admin-dash{
  position: fixed;
  right: 0;
  top: 0;
  height: 100vh;
  width: 420px;
  background: linear-gradient(180deg, #0d1013, #050607);
  box-shadow: -20px 0 60px rgba(0,0,0,.7);
  z-index: 200;
  transform: translateX(110%);
  transition: transform .32s ease;
  padding: 18px;
  overflow: auto;
  border-left: 1px solid #1a1d22;
}

.admin-dash.open{ transform: translateX(0); }

.admin-head{ display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px; }

.admin-panel{
  background: linear-gradient(180deg, #101215, #090a0b);
  border: 1px solid #1e2127;
  border-radius: 10px;
  padding: 12px;
  margin-top: 12px;
}

input[type="password"],
input[type="text"]{
  width: 100%;
  padding: 10px 12px;
  border-radius: 8px;
  background: #090b0d;
  color: var(--text);
  border: 1px solid #232a31;
  font-size: 16px;
}

.stack{ display: flex; flex-direction: column; gap: 8px; }
.small-stack{ display: flex; gap: 8px; flex-wrap: wrap; }

.badge-list{ display: flex; flex-direction: column; gap: 8px; margin-top: 8px; }

.badge-list .row{
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #1d2228;
  padding: 8px 0;
  color: var(--muted);
}

@media (max-width: 900px){
  .hero{ grid-template-columns: 1fr; }
  .team-grid{ grid-template-columns: repeat(2, 1fr); }
  .match-list{ grid-template-columns: 1fr; }
  .admin-dash{ width: min(92vw, 420px); }
  .score input{ width: 62px; height: 42px; font-size: 16px; }
}

@media (max-width: 600px){
  #menuToggle{ display: inline-flex; }
  .nav{
    display: none;
    position: absolute;
    top: 68px;
    right: 18px;
    flex-direction: column;
    background: #0a0c10;
    padding: 10px;
    border-radius: 10px;
    border: 1px solid var(--line);
    gap: 8px;
    min-width: 160px;
    z-index: 220;
  }
  .nav.mobile-open{ display: flex; }
  .wrap{ padding: 14px; }
  .team-grid{ grid-template-columns: repeat(2, 1fr); }
  .match-list{ grid-template-columns: 1fr; }
  .upload{ padding: 12px 14px; width: 100%; text-align: center; }
  .btn{ min-height: 44px; }
  .panel{ padding: 12px; }
  .admin-dash{
    top: auto;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100vw;
    height: 92vh;
    border-radius: 12px 12px 0 0;
    transform: translateY(110%);
    transition: transform .28s ease;
  }
  .admin-dash.open{ transform: translateY(0); }
  table, th, td{ font-size: 12px; }
  table{ min-width: unset; }
}

@media (max-width: 420px){
  .wrap{ padding: 12px; }
  .team-grid{ grid-template-columns: 1fr; }
  .score input{ width: 72px; height: 44px; font-size: 16px; }
  .badge{ width: 56px; height: 56px; }
  .mini-badge{ width: 28px; height: 28px; }
}

:focus{
  outline: 3px solid rgba(243,220,150,.12);
  outline-offset: 2px;
  border-radius: 6px;
}
