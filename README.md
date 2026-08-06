<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }

  .bio-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 28px;
    padding: 40px 16px;
    font-family: 'Segoe UI', 'Trebuchet MS', sans-serif;
  }

  .liquid-box {
    position: relative;
    width: 100%;
    max-width: 420px;
    background: linear-gradient(135deg, rgba(34,211,238,0.10), rgba(255,255,255,0.03));
    backdrop-filter: blur(22px) saturate(160%);
    -webkit-backdrop-filter: blur(22px) saturate(160%);
    border: 1px solid rgba(34,211,238,0.35);
    border-radius: 28px;
    box-shadow:
      0 8px 32px rgba(34,211,238,0.18),
      inset 0 0 24px rgba(34,211,238,0.06),
      inset 0 1px 0 rgba(255,255,255,0.15);
    padding: 28px 24px;
    overflow: hidden;
  }

  .liquid-box::before {
    content: "";
    position: absolute;
    top: -60%;
    left: -30%;
    width: 160%;
    height: 160%;
    background: radial-gradient(circle at 30% 30%, rgba(34,211,238,0.20), transparent 55%);
    pointer-events: none;
  }

  /* ---- Liquid 1 : Profil ---- */
  #liquid1 {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 14px;
  }

  .avatar {
    width: 130px;
    height: 130px;
    border-radius: 32px;
    object-fit: cover;
    border: 2px solid rgba(34,211,238,0.55);
    box-shadow: 0 0 26px rgba(34,211,238,0.45), 0 0 0 6px rgba(34,211,238,0.06);
    position: relative;
    z-index: 1;
  }

  .username {
    font-size: 26px;
    font-weight: 700;
    color: #e6feff;
    text-shadow: 0 0 14px rgba(34,211,238,0.75);
    letter-spacing: 0.5px;
    position: relative;
    z-index: 1;
  }

  .typewriter-line {
    font-size: 16px;
    font-weight: 500;
    color: #67f5ff;
    min-height: 22px;
    position: relative;
    z-index: 1;
  }

  .typewriter-line .cursor {
    display: inline-block;
    width: 2px;
    margin-left: 2px;
    background: #67f5ff;
    animation: blink 0.9s steps(1) infinite;
    box-shadow: 0 0 8px rgba(103,245,255,0.9);
  }

  @keyframes blink {
    0%, 49% { opacity: 1; }
    50%, 100% { opacity: 0; }
  }

  /* ---- Liquid 2 : GitHub stats ---- */
  #liquid2 {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 14px;
  }

  .section-title {
    font-size: 14px;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: #7fecff;
    opacity: 0.85;
    position: relative;
    z-index: 1;
  }

  .gh-stats-img {
    width: 100%;
    border-radius: 16px;
    position: relative;
    z-index: 1;
  }

  /* ---- Liquid 3 : Tech stack ---- */
  #liquid3 {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 18px;
  }

  .tech-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 16px;
    position: relative;
    z-index: 1;
  }

  .tech-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 6px;
    width: 68px;
  }

  .tech-item img {
    width: 42px;
    height: 42px;
    filter: drop-shadow(0 0 10px rgba(34,211,238,0.55));
    transition: transform 0.25s ease, filter 0.25s ease;
  }

  .tech-item:hover img {
    transform: translateY(-4px) scale(1.08);
    filter: drop-shadow(0 0 16px rgba(34,211,238,0.9));
  }

  .tech-item span {
    font-size: 11px;
    color: #b9fbff;
    opacity: 0.85;
  }
</style>

<div class="bio-wrapper">

  <div class="liquid-box" id="liquid1">
    <img class="avatar" src="https://yt3.ggpht.com/i21awVZzeV03hEZuHh2RLdAFzgtsugzYZ5KH_emhLBxEkCvqSzbs5VhZhC5KWNkUnpa3fdJApQ=s600-c-k-c0x00ffffff-no-rj-rp-mo" alt="profil foto">
    <div class="username">bnBurned</div>
    <div class="typewriter-line" id="typewriter"><span id="tw-text"></span><span class="cursor">&nbsp;</span></div>
  </div>

  <div class="liquid-box" id="liquid2">
    <div class="section-title">GitHub İstatistikleri</div>
    <img class="gh-stats-img" src="https://github-readme-stats.vercel.app/api?username=BnBurned&show_icons=true&theme=tokyonight&hide_border=true&bg_color=00000000&title_color=22d3ee&icon_color=22d3ee&text_color=b9fbff" alt="github stats">
    <img class="gh-stats-img" src="https://github-readme-streak-stats.herokuapp.com/?user=BnBurned&theme=tokyonight&hide_border=true&background=00000000&ring=22d3ee&fire=22d3ee&currStreakLabel=22d3ee" alt="github streak">
  </div>

  <div class="liquid-box" id="liquid3">
    <div class="section-title">Kullandığım Diller</div>
    <div class="tech-grid">
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="html">
        <span>HTML</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="css">
        <span>CSS</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="javascript">
        <span>JS</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="java">
        <span>Java</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" alt="angular">
        <span>Angular</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" alt="c">
        <span>C</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="c++">
        <span>C++</span>
      </div>
      <div class="tech-item">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original.svg" alt="golang">
        <span>Go</span>
      </div>
    </div>
  </div>

</div>

<script>
  (function () {
    const phrases = ["I Am A Coder", "I Like Coding", "Just Coding", "Vibe Coding"];
    const el = document.getElementById('tw-text');
    let phraseIndex = 0;
    let charIndex = 0;
    let deleting = false;

    function tick() {
      const current = phrases[phraseIndex];

      if (!deleting) {
        charIndex++;
        el.textContent = current.slice(0, charIndex);
        if (charIndex === current.length) {
          deleting = true;
          setTimeout(tick, 1400);
          return;
        }
      } else {
        charIndex--;
        el.textContent = current.slice(0, charIndex);
        if (charIndex === 0) {
          deleting = false;
          phraseIndex = (phraseIndex + 1) % phrases.length;
        }
      }

      setTimeout(tick, deleting ? 45 : 85);
    }

    tick();
  })();
</script>
