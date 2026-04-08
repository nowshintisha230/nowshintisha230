<style>
@keyframes spin-slow { from{transform:rotate(0deg)} to{transform:rotate(360deg)} }
@keyframes blink-cursor { 0%,100%{opacity:1} 50%{opacity:0} }
@keyframes bounce-dot { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-4px)} }
@keyframes screen-flicker { 0%,100%{opacity:1} 92%{opacity:0.95} 95%{opacity:1} }
@keyframes float-icon { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-5px)} }
@keyframes wave-hand { 0%,100%{transform:rotate(0deg)} 20%{transform:rotate(18deg)} 40%{transform:rotate(-8deg)} 60%{transform:rotate(18deg)} 80%{transform:rotate(0deg)} }
@keyframes shimmer { 0%{left:-60%} 100%{left:120%} }
@keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

.banner-wrap {
  background: linear-gradient(135deg, #FFF0F8 0%, #F3EEFF 40%, #EAF6FF 100%);
  border-radius: 20px;
  padding: 0;
  overflow: hidden;
  position: relative;
  font-family: 'Segoe UI', Arial, sans-serif;
  width: 100%;
  max-width: 680px;
  margin: 0 auto;
}
.blob1 { position:absolute;top:-30px;left:-30px;width:160px;height:160px;background:#FFD6F0;border-radius:50% 40% 60% 50%;opacity:0.5; }
.blob2 { position:absolute;bottom:-20px;right:-20px;width:140px;height:140px;background:#D6E8FF;border-radius:60% 50% 40% 60%;opacity:0.5; }
.blob3 { position:absolute;top:40px;right:80px;width:80px;height:80px;background:#E8D6FF;border-radius:50%;opacity:0.35; }
.main-content { position:relative;display:flex;align-items:center;padding:32px 36px 28px;gap:28px; }
.left-col { flex:1;min-width:0; }
.right-col { width:160px;flex-shrink:0;display:flex;align-items:center;justify-content:center; }
.greeting-row { display:flex;align-items:center;gap:8px;margin-bottom:6px; }
.wave { display:inline-block;font-size:22px;animation:wave-hand 1.8s ease-in-out infinite;transform-origin:70% 70%; }
.hi-text { font-size:15px;color:#C06BB0;font-weight:500;letter-spacing:1px; }
.name-main { font-size:28px;font-weight:800;color:#6B2F8A;line-height:1.1;letter-spacing:0.5px;margin-bottom:2px; }
.name-sub { font-size:13px;font-weight:500;color:#A07BC0;letter-spacing:2px;margin-bottom:12px;text-transform:uppercase; }
.role-tag { display:inline-flex;align-items:center;gap:6px;background:#FFF;border:1.5px solid #E8B4F0;border-radius:20px;padding:5px 14px;margin-bottom:16px; }
.role-dot { width:8px;height:8px;background:#D45EAE;border-radius:50%;animation:bounce-dot 2s ease-in-out infinite; }
.role-text { font-size:12px;font-weight:600;color:#A0309A;letter-spacing:1.5px;text-transform:uppercase; }
.skills-row { display:flex;flex-wrap:wrap;gap:6px;margin-bottom:14px; }
.skill-pill { padding:4px 12px;border-radius:20px;font-size:11px;font-weight:600;letter-spacing:0.5px;border:1.5px solid transparent;position:relative;overflow:hidden; }
.skill-pill::after { content:'';position:absolute;top:0;left:-60%;width:40%;height:100%;background:rgba(255,255,255,0.5);transform:skewX(-20deg);animation:shimmer 3s ease-in-out infinite; }
.sp-pink { background:#FDE8F7;border-color:#F0A0D8;color:#9C2A80; }
.sp-purple { background:#EEE6FF;border-color:#C8A8F0;color:#5E2D9C; }
.sp-blue { background:#E4F0FF;border-color:#90C0F8;color:#1A5EA8; }
.sp-mint { background:#E2F8F2;border-color:#7DDFC0;color:#0E6E50; }
.sp-coral { background:#FFE9E2;border-color:#F8B09A;color:#A83010; }
.typing-row { display:flex;align-items:center;gap:4px; }
.typed-text { font-family:monospace;font-size:12px;color:#7040A0;font-weight:500; }
.cursor { display:inline-block;width:2px;height:14px;background:#D45EAE;animation:blink 1s steps(1) infinite;vertical-align:middle; }
.footer-strip { background:rgba(255,255,255,0.6);border-top:1px solid #EDD6F8;padding:8px 36px;display:flex;align-items:center;gap:10px; }
.footer-tag { font-size:10px;font-weight:600;color:#9060B0;letter-spacing:1px;text-transform:uppercase;opacity:0.7; }
.footer-divider { width:1px;height:12px;background:#D0A0E8;opacity:0.5; }
.open-badge { display:flex;align-items:center;gap:5px;margin-left:auto;background:#E8FFF3;border:1px solid #7DDFC0;border-radius:12px;padding:3px 10px; }
.open-dot { width:6px;height:6px;background:#22C55E;border-radius:50%;animation:blink 2s steps(1) infinite; }
.open-text { font-size:10px;font-weight:600;color:#0E6E50;letter-spacing:0.5px; }
</style>

<div class="banner-wrap">
  <div class="blob1"></div>
  <div class="blob2"></div>
  <div class="blob3"></div>

  <div class="main-content">
    <div class="left-col">
      <div class="greeting-row">
        <span class="wave">👋</span>
        <span class="hi-text">Hi there, I'm</span>
      </div>
      <div class="name-main">Nafisha Nowshin</div>
      <div class="name-sub">Tisha</div>
      <div class="role-tag">
        <span class="role-dot"></span>
        <span class="role-text">Frontend Developer</span>
      </div>
      <div class="skills-row">
        <span class="skill-pill sp-coral">HTML</span>
        <span class="skill-pill sp-blue">CSS</span>
        <span class="skill-pill sp-mint">Tailwind</span>
        <span class="skill-pill sp-pink">JavaScript</span>
        <span class="skill-pill sp-purple">React</span>
      </div>
      <div class="typing-row">
        <span class="typed-text" id="typed"></span>
        <span class="cursor"></span>
      </div>
    </div>

    <div class="right-col">
      <svg width="160" height="160" viewBox="0 0 160 160" xmlns="http://www.w3.org/2000/svg">
        <circle cx="80" cy="80" r="72" fill="none" stroke="#E8B4F0" stroke-width="1.5" stroke-dasharray="6 4"
          style="transform-origin:80px 80px;animation:spin-slow 14s linear infinite"/>
        <circle cx="80" cy="80" r="62" fill="none" stroke="#F4D0F8" stroke-width="1"/>
        <circle cx="80" cy="80" r="56" fill="#FFF0FC"/>
        <ellipse cx="80" cy="118" rx="22" ry="14" fill="#C879D8"/>
        <ellipse cx="80" cy="105" rx="12" ry="5" fill="#E0A0F0"/>
        <rect x="75" y="97" width="10" height="10" rx="4" fill="#F9C0D8"/>
        <ellipse cx="80" cy="88" rx="18" ry="19" fill="#F9C0D8"/>
        <ellipse cx="80" cy="72" rx="19" ry="10" fill="#4A2060"/>
        <ellipse cx="64" cy="85" rx="7" ry="14" fill="#4A2060"/>
        <ellipse cx="96" cy="85" rx="7" ry="14" fill="#4A2060"/>
        <ellipse cx="74" cy="70" rx="5" ry="3" fill="#7A4090" opacity="0.6"/>
        <ellipse cx="74" cy="88" rx="3.5" ry="4" fill="#2D1040"/>
        <ellipse cx="86" cy="88" rx="3.5" ry="4" fill="#2D1040"/>
        <circle cx="75.5" cy="86.5" r="1.2" fill="white"/>
        <circle cx="87.5" cy="86.5" r="1.2" fill="white"/>
        <path d="M71 85 Q73 83 75 84" fill="none" stroke="#2D1040" stroke-width="1.2" stroke-linecap="round"/>
        <path d="M83 85 Q85 83 87 84" fill="none" stroke="#2D1040" stroke-width="1.2" stroke-linecap="round"/>
        <circle cx="80" cy="93" r="1.2" fill="#E8A0C0" opacity="0.7"/>
        <path d="M75 97 Q80 101 85 97" fill="none" stroke="#C05090" stroke-width="1.5" stroke-linecap="round"/>
        <ellipse cx="70" cy="94" rx="4" ry="2.5" fill="#FFB0C8" opacity="0.5"/>
        <ellipse cx="90" cy="94" rx="4" ry="2.5" fill="#FFB0C8" opacity="0.5"/>
        <path d="M62 110 Q50 118 44 122" fill="none" stroke="#F9C0D8" stroke-width="7" stroke-linecap="round"/>
        <path d="M98 110 Q110 118 116 122" fill="none" stroke="#F9C0D8" stroke-width="7" stroke-linecap="round"/>
        <rect x="36" y="122" width="88" height="10" rx="3" fill="#B060D0"/>
        <rect x="42" y="98" width="76" height="26" rx="4" fill="#2D1040"/>
        <rect x="44" y="100" width="72" height="22" rx="3" fill="#1A0A30" style="animation:screen-flicker 4s ease-in-out infinite"/>
        <rect x="48" y="104" width="28" height="2.5" rx="1.2" fill="#F472B6" opacity="0.9"/>
        <rect x="50" y="109" width="40" height="2.5" rx="1.2" fill="#A78BFA" opacity="0.9"/>
        <rect x="50" y="114" width="20" height="2.5" rx="1.2" fill="#67E8F9" opacity="0.9"/>
        <rect x="80" y="114" width="22" height="2.5" rx="1.2" fill="#FCA5A5" opacity="0.7"/>
        <rect x="72" y="104" width="2" height="5" rx="1" fill="#F9FAFB"
          style="animation:blink-cursor 1s steps(1) infinite"/>
        <text x="18" y="58" font-size="13" style="animation:float-icon 2s ease-in-out infinite">✦</text>
        <text x="130" y="52" font-size="10" style="animation:float-icon 2s ease-in-out 0.5s infinite">✦</text>
        <text x="138" y="80" font-size="8" style="animation:float-icon 2s ease-in-out 1s infinite">◆</text>
        <text x="14" y="100" font-size="8" style="animation:float-icon 2s ease-in-out 1.5s infinite">◆</text>
        <circle cx="80" cy="16" r="4" fill="#F472B6" style="animation:bounce-dot 1.5s ease-in-out infinite"/>
        <circle cx="68" cy="14" r="3" fill="#A78BFA" style="animation:bounce-dot 1.5s ease-in-out 0.3s infinite"/>
        <circle cx="92" cy="14" r="3" fill="#67E8F9" style="animation:bounce-dot 1.5s ease-in-out 0.6s infinite"/>
      </svg>
    </div>
  </div>

  <div class="footer-strip">
    <span class="footer-tag">Building beautiful UIs</span>
    <div class="footer-divider"></div>
    <span class="footer-tag">Pixel-perfect designs</span>
    <div class="footer-divider"></div>
    <span class="footer-tag">Passionate about React</span>
    <div class="open-badge">
      <span class="open-dot"></span>
      <span class="open-text">Open to work</span>
    </div>
  </div>
</div>

<script>
const phrases = ["I craft pixel-perfect UIs","I love clean, minimal design","I build with React & Tailwind","I turn ideas into interfaces"];
let pi=0,ci=0,deleting=false;
const el=document.getElementById('typed');
function type(){
  const word=phrases[pi];
  if(!deleting){el.textContent=word.slice(0,++ci);if(ci===word.length){deleting=true;setTimeout(type,1800);return;}}
  else{el.textContent=word.slice(0,--ci);if(ci===0){deleting=false;pi=(pi+1)%phrases.length;setTimeout(type,400);return;}}
  setTimeout(type,deleting?40:70);
}
type();
</script>