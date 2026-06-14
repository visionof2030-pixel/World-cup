<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
  <title>🏆 كأس العالم 2026 – متتبع المباريات | مدرسة سعيد بن العاص</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      -webkit-tap-highlight-color: transparent;
    }

    body {
      background: radial-gradient(circle at 10% 20%, #0a1f24, #030c10);
      font-family: 'Segoe UI', 'Cairo', 'Inter', system-ui, -apple-system, 'Roboto', sans-serif;
      padding: 20px 12px;
      min-height: 100vh;
      color: #f0f9ff;
      font-size: 14px;
    }

    .app-container {
      max-width: 1200px;
      margin: 0 auto;
      width: 100%;
    }

    .hero {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(20px);
      border-radius: 48px;
      padding: 20px 20px;
      margin-bottom: 28px;
      text-align: center;
      border: 1px solid rgba(255, 200, 100, 0.3);
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
    }

    .hero h1 {
      font-size: 1.8rem;
      background: linear-gradient(135deg, #FFE6B0, #FFA559, #FF6A3D);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      margin-bottom: 8px;
      letter-spacing: -0.5px;
    }

    .school-badge {
      background: rgba(30, 74, 95, 0.7);
      backdrop-filter: blur(4px);
      display: inline-block;
      padding: 6px 20px;
      border-radius: 60px;
      font-size: 0.75rem;
      font-weight: 500;
      border: 1px solid #ffb34760;
    }

    .control-panel {
      background: rgba(10, 25, 30, 0.6);
      backdrop-filter: blur(16px);
      border-radius: 80px;
      padding: 8px 20px;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 12px;
      margin-bottom: 28px;
      border: 1px solid rgba(255, 200, 100, 0.25);
    }

    .search-group {
      flex: 2;
      min-width: 160px;
    }

    .search-group input {
      width: 100%;
      padding: 12px 20px;
      border-radius: 60px;
      border: none;
      background: #fef9e6;
      text-align: right;
      outline: none;
      font-size: 0.85rem;
      font-weight: 500;
      transition: 0.2s;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .search-group input:focus {
      transform: scale(0.98);
      box-shadow: 0 0 0 2px #ffb347;
    }

    .round-group {
      flex: 1;
      min-width: 130px;
    }

    .round-group select {
      width: 100%;
      padding: 12px 12px;
      border-radius: 60px;
      background: #fef9e6;
      font-weight: bold;
      cursor: pointer;
      font-size: 0.8rem;
      border: none;
      outline: none;
      font-family: inherit;
    }

    .tabs {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin: 20px 0 24px;
      justify-content: center;
    }

    .tab-btn {
      background: rgba(20, 40, 48, 0.7);
      backdrop-filter: blur(8px);
      border: 1px solid rgba(255, 180, 70, 0.4);
      padding: 10px 20px;
      border-radius: 60px;
      font-size: 0.85rem;
      font-weight: 600;
      cursor: pointer;
      color: #ffefa6;
      transition: all 0.2s ease;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      letter-spacing: 0.3px;
    }

    .tab-btn i { font-style: normal; font-size: 1.1rem; }

    .tab-btn.active {
      background: linear-gradient(105deg, #ffb347, #ff8c1a);
      color: #1a2f2f;
      border-color: #ffdd99;
      box-shadow: 0 8px 18px rgba(255, 140, 26, 0.25);
    }

    .tab-btn:hover:not(.active) {
      background: rgba(255, 180, 70, 0.2);
      border-color: #ffb347;
      transform: translateY(-2px);
    }

    .tab-content {
      display: none;
      animation: fadeSlide 0.25s ease;
    }

    .tab-content.active {
      display: block;
    }

    @keyframes fadeSlide {
      from { opacity: 0; transform: translateY(6px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .matches-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(330px, 1fr));
      gap: 22px;
    }

    .match-card {
      background: rgba(18, 38, 44, 0.75);
      backdrop-filter: blur(12px);
      border-radius: 32px;
      padding: 16px;
      border: 1px solid rgba(255, 180, 70, 0.3);
      transition: all 0.25s;
      box-shadow: 0 12px 24px -12px rgba(0,0,0,0.4);
    }

    .match-card:hover {
      transform: translateY(-3px);
      border-color: #ffb347aa;
      box-shadow: 0 20px 30px -12px black;
    }

    .match-card.live-card {
      border: 2px solid #ff4d4d;
      background: linear-gradient(135deg, #2a414b, #0f2e36);
      box-shadow: 0 0 12px rgba(255, 60, 30, 0.4);
    }

    .teams {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 8px;
      background: rgba(0, 0, 0, 0.3);
      padding: 10px 12px;
      border-radius: 80px;
    }

    .team {
      background: rgba(0, 0, 0, 0.4);
      padding: 6px 12px;
      border-radius: 60px;
      flex: 1;
      text-align: center;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      font-weight: 700;
      font-size: 0.85rem;
      white-space: nowrap;
      overflow-x: auto;
    }

    .team span:first-child { font-size: 1.2rem; }

    .vs {
      background: #ffb347;
      padding: 4px 12px;
      border-radius: 40px;
      font-weight: bold;
      font-size: 0.7rem;
      color: #1e2a2a;
    }

    .datetime-row {
      display: flex;
      justify-content: space-between;
      gap: 10px;
      background: rgba(0, 0, 0, 0.35);
      padding: 8px 14px;
      border-radius: 50px;
      flex-wrap: wrap;
      margin-top: 6px;
    }

    .match-day {
      background: #1e4a5f;
      padding: 4px 12px;
      border-radius: 40px;
      font-size: 0.7rem;
      font-weight: 600;
    }

    .match-full-date {
      background: rgba(0, 0, 0, 0.5);
      padding: 4px 12px;
      border-radius: 40px;
      font-size: 0.7rem;
      display: flex;
      gap: 6px;
      align-items: baseline;
    }

    .info-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 4px;
    }

    .round-tag {
      background: #2f5663;
      padding: 4px 14px;
      border-radius: 60px;
      font-size: 0.7rem;
      font-weight: 500;
    }

    .countdown-timer {
      background: #00000070;
      font-family: monospace;
      font-size: 0.9rem;
      font-weight: bold;
      padding: 4px 14px;
      border-radius: 60px;
      text-align: center;
      letter-spacing: 0.5px;
    }

    .live-status {
      animation: pulse 1.2s infinite;
      background: #d32f2f;
    }

    @keyframes pulse {
      0% { opacity: 0.75; background: #b71c1c; box-shadow: 0 0 0 0 #ff5e5e; }
      50% { opacity: 1; background: #f44336; box-shadow: 0 0 0 3px rgba(255, 68, 34, 0.4); }
      100% { opacity: 0.75; background: #b71c1c; }
    }

    .empty-state {
      grid-column: 1/-1;
      text-align: center;
      background: rgba(12, 34, 40, 0.7);
      backdrop-filter: blur(8px);
      padding: 40px 20px;
      border-radius: 60px;
      font-size: 1rem;
      border: 1px dashed #ffb34780;
    }

    .filter-bar {
      margin-bottom: 24px;
      background: rgba(0, 0, 0, 0.25);
      padding: 8px 16px;
      border-radius: 80px;
      display: flex;
    }

    .filter-bar input {
      background: #fef7e0;
      border: none;
      padding: 12px 20px;
      border-radius: 60px;
      width: 100%;
      font-size: 0.85rem;
      outline: none;
    }

    .groups-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(360px, 1fr));
      gap: 24px;
    }

    .group-card {
      background: rgba(30, 60, 72, 0.65);
      backdrop-filter: blur(12px);
      border-radius: 32px;
      padding: 16px;
      border: 1px solid #ffb34760;
      transition: 0.2s;
    }

    .group-title {
      font-size: 1.4rem;
      font-weight: 800;
      text-align: center;
      margin-bottom: 16px;
      color: #FFE6B0;
      letter-spacing: -0.5px;
    }

    .standings-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.7rem;
      min-width: 320px;
    }

    .standings-table th, .standings-table td {
      padding: 8px 4px;
      text-align: center;
    }

    .standings-table th {
      background: #1e4655;
      color: #FFE0A3;
      font-weight: 700;
      border-radius: 16px 16px 0 0;
    }

    .standings-table td {
      background-color: #f3f7f9;
      color: #11242a;
      font-weight: 600;
      border-bottom: 1px solid #cddce0;
    }

    .team-name-td {
      text-align: right;
      display: flex;
      align-items: center;
      gap: 6px;
      justify-content: flex-start;
    }

    .quick-search-results {
      background: rgba(0, 25, 30, 0.92);
      backdrop-filter: blur(24px);
      border-radius: 36px;
      padding: 20px;
      margin-bottom: 24px;
      border: 1px solid #ffb347cc;
    }

    .quick-search-title {
      font-size: 1.2rem;
      font-weight: 700;
      margin-bottom: 16px;
      border-right: 4px solid #ffb347;
      padding-right: 16px;
    }

    .quick-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 16px;
    }

    .quick-match-card {
      background: #0f3e4a;
      border-radius: 28px;
      padding: 12px;
      transition: 0.1s;
    }

    .quick-match-teams {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 8px;
      font-weight: bold;
      font-size: 0.85rem;
    }

    footer {
      margin-top: 45px;
      text-align: center;
      font-size: 0.7rem;
      color: #98bdc9;
      border-top: 1px solid #ffb34760;
      padding-top: 20px;
    }

    @media (max-width: 550px) {
      body { padding: 12px; }
      .hero h1 { font-size: 1.3rem; }
      .tab-btn { padding: 6px 14px; font-size: 0.75rem; gap: 4px; }
      .team { font-size: 0.7rem; white-space: normal; }
      .team span:first-child { font-size: 1rem; }
      .countdown-timer { font-size: 0.75rem; }
      .matches-grid { gap: 14px; }
    }
  </style>
</head>
<body>
<div class="app-container">
  <div class="hero">
    <h1>🏆 كأس العالم 2026 ⚡</h1>
    <div class="school-badge">📢 غرفة معلمي سعيد بن العاص | ترتيب مباشر من الـ API</div>
  </div>

  <div class="control-panel">
    <div class="search-group">
      <input type="text" id="globalSearchInput" placeholder="🔍 ابحث عن منتخب (مباريات قادمة أو سابقة)" autocomplete="off">
    </div>
    <div class="round-group">
      <select id="roundFilter">
        <option value="all">🌍 جميع الجولات</option>
        <option value="first">🟢 الجولة الأولى</option>
        <option value="second">🟩 الجولة الثانية</option>
        <option value="third">🟥 الجولة الثالثة</option>
      </select>
    </div>
  </div>

  <div id="quickSearchResults" class="quick-search-results">
    <div class="quick-search-title">🔍 نتائج البحث عن "<span id="searchKeyword"></span>"</div>
    <div id="quickResultsContainer" class="quick-grid"></div>
  </div>

  <div class="tabs">
    <button class="tab-btn active" data-tab="upcoming"><i>⚡</i> القادمة والجارية</button>
    <button class="tab-btn" data-tab="previous"><i>📋</i> المباريات السابقة</button>
    <button class="tab-btn" data-tab="standings"><i>📊</i> ترتيب المجموعات</button>
  </div>

  <div id="upcomingTab" class="tab-content active">
    <div id="matchesContainer" class="matches-grid"><div class="empty-state">✨ جاري تحميل المباريات ✨</div></div>
  </div>

  <div id="previousTab" class="tab-content">
    <div class="filter-bar">
      <input type="text" id="prevSearchInput" placeholder="🔍 بحث في المباريات السابقة...">
    </div>
    <div id="previousMatchesContainer" class="matches-grid"><div class="empty-state">📋 جاري تحميل المباريات السابقة...</div></div>
  </div>

  <div id="standingsTab" class="tab-content">
    <div id="standingsContainer" class="groups-container"><div class="empty-state">📊 جاري حساب الترتيب من نتائج API...</div></div>
  </div>

  <footer>🔄 التحديث التلقائي | الترتيب يُحسب حصرياً من نتائج المباريات المنتهية (API)</footer>
</div>

<script>
  // ======================= الدوال الأساسية =========================
  function now() { return new Date().getTime(); }
  function matchTime(t) { return new Date(t).getTime(); }
  const MATCH_DURATION = 105 * 60 * 1000;
  function getMatchStatus(m) {
    const start = matchTime(m.timeISO);
    const end = start + MATCH_DURATION;
    const cur = now();
    if (cur < start) {
      const diff = start - cur;
      const h = Math.floor(diff/3600000);
      const min = Math.floor((diff%3600000)/60000);
      const s = Math.floor((diff%60000)/1000);
      return { live: false, text: `⏱️ ${h}h ${min}m ${s}s` };
    } else if (cur <= end) return { live: true, text: "🔴 تُلعب الآن 🔴" };
    else return { live: false, text: "✅ انتهت" };
  }
  function upcomingMatches(arr) { return arr.filter(m => (matchTime(m.timeISO)+MATCH_DURATION) > now()); }
  function filterRound(arr, r) { if (r==="all") return arr; return arr.filter(m => m.round === r); }

  function getFlag(name) {
    const map = {
      "المكسيك":"🇲🇽","جنوب أفريقيا":"🇿🇦","الأرجنتين":"🇦🇷","الجزائر":"🇩🇿","النمسا":"🇦🇹","الأردن":"🇯🇴","البرتغال":"🇵🇹","الكونغو الديمقراطية":"🇨🇩","كوريا الجنوبية":"🇰🇷","التشيك":"🇨🇿","كندا":"🇨🇦","البوسنة والهرسك":"🇧🇦","أمريكا":"🇺🇸","العراق":"🇮🇶","سويسرا":"🇨🇭","قطر":"🇶🇦","البرازيل":"🇧🇷","المغرب":"🇲🇦","هايتي":"🇭🇹","إسكتلندا":"🏴󠁧󠁢󠁳󠁣󠁴󠁿","أستراليا":"🇦🇺","تركيا":"🇹🇷","ألمانيا":"🇩🇪","كوراساو":"🇨🇼","اليابان":"🇯🇵","هولندا":"🇳🇱","الإكوادور":"🇪🇨","ساحل العاج":"🇨🇮","السويد":"🇸🇪","تونس":"🇹🇳","إسبانيا":"🇪🇸","الرأس الأخضر":"🇨🇻","مصر":"🇪🇬","بلجيكا":"🇧🇪","السعودية":"🇸🇦","أوروغواي":"🇺🇾","إيران":"🇮🇷","نيوزيلندا":"🇳🇿","السنغال":"🇸🇳","فرنسا":"🇫🇷","النرويج":"🇳🇴","إنجلترا":"🏴󠁧󠁢󠁥󠁮󠁧󠁿","كرواتيا":"🇭🇷","بنما":"🇵🇦","كولومبيا":"🇨🇴","أوزبكستان":"🇺🇿","غانا":"🇬🇭","باراغواي":"🇵🇾"
    };
    return map[name] || "🏁";
  }

  function getDay(t) { return ['الأحد','الاثنين','الثلاثاء','الأربعاء','الخميس','الجمعة','السبت'][new Date(t).getDay()]; }
  function getDateFmt(t) {
    const d = new Date(t);
    const months = ['يناير','فبراير','مارس','أبريل','مايو','يونيو','يوليو','أغسطس','سبتمبر','أكتوبر','نوفمبر','ديسمبر'];
    return `${d.getDate()} ${months[d.getMonth()]} ${d.getFullYear()}`;
  }
  function getTimeFromISO(t) {
    const d = new Date(t);
    let hours = d.getHours();
    let minutes = d.getMinutes();
    hours = hours < 10 ? '0'+hours : hours;
    minutes = minutes < 10 ? '0'+minutes : minutes;
    return `${hours}:${minutes}`;
  }
  function getDateTimeDisplay(t) { return `${getDateFmt(t)} - ${getTimeFromISO(t)}`; }

  // ------------------- بيانات المباريات القادمة (نفس السابق) -----------------
  const rawMatches = [ /* مجموعة المباريات الكاملة كما في الطلبات السابقة تم اختصارها للطول لكنها كاملة في الكود الأصلي */
    { team1:"المكسيك", team2:"جنوب أفريقيا", time:"2026-06-11T22:00:00", round:"first" },{ team1:"الأرجنتين", team2:"الجزائر", time:"2026-06-11T04:00:00", round:"first" },
    { team1:"النمسا", team2:"الأردن", time:"2026-06-11T07:00:00", round:"first" },{ team1:"البرتغال", team2:"الكونغو الديمقراطية", time:"2026-06-11T20:00:00", round:"first" },
    { team1:"كوريا الجنوبية", team2:"التشيك", time:"2026-06-12T05:00:00", round:"first" },{ team1:"كندا", team2:"البوسنة والهرسك", time:"2026-06-12T22:00:00", round:"first" },
    { team1:"أمريكا", team2:"العراق", time:"2026-06-13T04:00:00", round:"first" },{ team1:"سويسرا", team2:"قطر", time:"2026-06-13T22:00:00", round:"first" },
    { team1:"البرازيل", team2:"المغرب", time:"2026-06-14T01:00:00", round:"first" },{ team1:"هايتي", team2:"إسكتلندا", time:"2026-06-14T04:00:00", round:"first" },
    { team1:"أستراليا", team2:"تركيا", time:"2026-06-14T07:00:00", round:"first" },{ team1:"ألمانيا", team2:"كوراساو", time:"2026-06-14T20:00:00", round:"first" },
    { team1:"اليابان", team2:"هولندا", time:"2026-06-14T23:00:00", round:"first" },{ team1:"الإكوادور", team2:"ساحل العاج", time:"2026-06-15T02:00:00", round:"first" },
    { team1:"السويد", team2:"تونس", time:"2026-06-15T05:00:00", round:"first" },{ team1:"إسبانيا", team2:"الرأس الأخضر", time:"2026-06-15T19:00:00", round:"first" },
    { team1:"مصر", team2:"بلجيكا", time:"2026-06-15T22:00:00", round:"first" },{ team1:"السعودية", team2:"أوروغواي", time:"2026-06-16T01:00:00", round:"first" },
    { team1:"إيران", team2:"نيوزيلندا", time:"2026-06-16T04:00:00", round:"first" },{ team1:"السنغال", team2:"فرنسا", time:"2026-06-16T22:00:00", round:"first" },
    { team1:"النرويج", team2:"العراق", time:"2026-06-17T01:00:00", round:"first" },{ team1:"الجزائر", team2:"الأرجنتين", time:"2026-06-17T04:00:00", round:"first" },
    { team1:"الأردن", team2:"النمسا", time:"2026-06-17T07:00:00", round:"first" },{ team1:"البرتغال", team2:"كرواتيا", time:"2026-06-17T20:00:00", round:"first" },
    { team1:"إنجلترا", team2:"كرواتيا", time:"2026-06-17T23:00:00", round:"first" },{ team1:"جنوب أفريقيا", team2:"التشيك", time:"2026-06-18T19:00:00", round:"second" },
    { team1:"سويسرا", team2:"البوسنة والهرسك", time:"2026-06-18T22:00:00", round:"second" },{ team1:"قطر", team2:"كندا", time:"2026-06-19T01:00:00", round:"second" },
    { team1:"المكسيك", team2:"كوريا الجنوبية", time:"2026-06-19T04:00:00", round:"second" },{ team1:"أستراليا", team2:"أمريكا", time:"2026-06-19T22:00:00", round:"second" },
    { team1:"المغرب", team2:"إسكتلندا", time:"2026-06-20T01:00:00", round:"second" },{ team1:"البرازيل", team2:"هايتي", time:"2026-06-20T03:30:00", round:"second" },
    { team1:"تركيا", team2:"باراغواي", time:"2026-06-20T06:00:00", round:"second" },{ team1:"السويد", team2:"هولندا", time:"2026-06-20T20:00:00", round:"second" },
    { team1:"ساحل العاج", team2:"ألمانيا", time:"2026-06-20T23:00:00", round:"second" },{ team1:"الإكوادور", team2:"كوراساو", time:"2026-06-21T03:00:00", round:"second" },
    { team1:"اليابان", team2:"تونس", time:"2026-06-21T07:00:00", round:"second" },{ team1:"إسبانيا", team2:"السعودية", time:"2026-06-21T19:00:00", round:"second" },
    { team1:"بلجيكا", team2:"إيران", time:"2026-06-21T22:00:00", round:"second" },{ team1:"أوروجواي", team2:"الرأس الأخضر", time:"2026-06-22T01:00:00", round:"second" },
    { team1:"مصر", team2:"نيوزيلندا", time:"2026-06-22T04:00:00", round:"second" },{ team1:"الأرجنتين", team2:"النمسا", time:"2026-06-22T20:00:00", round:"second" },
    { team1:"العراق", team2:"فرنسا", time:"2026-06-23T00:00:00", round:"second" },{ team1:"النرويج", team2:"السنغال", time:"2026-06-23T03:00:00", round:"second" },
    { team1:"الأردن", team2:"الجزائر", time:"2026-06-23T06:00:00", round:"second" },{ team1:"البرتغال", team2:"أوزبكستان", time:"2026-06-23T20:00:00", round:"second" },
    { team1:"إنجلترا", team2:"غانا", time:"2026-06-23T23:00:00", round:"second" },{ team1:"بنما", team2:"كرواتيا", time:"2026-06-24T02:00:00", round:"second" },
    { team1:"كولومبيا", team2:"الكونغو الديمقراطية", time:"2026-06-24T05:00:00", round:"second" },{ team1:"كندا", team2:"سويسرا", time:"2026-06-24T22:00:00", round:"third" },
    { team1:"قطر", team2:"البوسنة والهرسك", time:"2026-06-24T22:00:00", round:"third" },{ team1:"المغرب", team2:"هايتي", time:"2026-06-25T01:00:00", round:"third" },
    { team1:"اسكتلندا", team2:"البرازيل", time:"2026-06-25T01:00:00", round:"third" },{ team1:"جنوب أفريقيا", team2:"كوريا الجنوبية", time:"2026-06-25T04:00:00", round:"third" },
    { team1:"المكسيك", team2:"التشيك", time:"2026-06-25T04:00:00", round:"third" },{ team1:"كوراساو", team2:"ساحل العاج", time:"2026-06-25T23:00:00", round:"third" },
    { team1:"ألمانيا", team2:"الإكوادور", time:"2026-06-25T23:00:00", round:"third" },{ team1:"هولندا", team2:"تونس", time:"2026-06-26T02:00:00", round:"third" },
    { team1:"اليابان", team2:"السويد", time:"2026-06-26T02:00:00", round:"third" },{ team1:"أمريكا", team2:"تركيا", time:"2026-06-26T05:00:00", round:"third" },
    { team1:"أستراليا", team2:"باراغواي", time:"2026-06-26T05:00:00", round:"third" },{ team1:"فرنسا", team2:"النرويج", time:"2026-06-26T22:00:00", round:"third" },
    { team1:"السنغال", team2:"العراق", time:"2026-06-26T22:00:00", round:"third" },{ team1:"السعودية", team2:"الرأس الأخضر", time:"2026-06-27T03:00:00", round:"third" },
    { team1:"إسبانيا", team2:"أوروغواي", time:"2026-06-27T03:00:00", round:"third" },{ team1:"إيران", team2:"مصر", time:"2026-06-27T06:00:00", round:"third" },
    { team1:"نيوزيلندا", team2:"بلجيكا", time:"2026-06-27T06:00:00", round:"third" },{ team1:"إنجلترا", team2:"بنما", time:"2026-06-28T00:00:00", round:"third" },
    { team1:"كرواتيا", team2:"غانا", time:"2026-06-28T00:00:00", round:"third" },{ team1:"البرتغال", team2:"كولومبيا", time:"2026-06-28T02:30:00", round:"third" },
    { team1:"الكونغو الديمقراطية", team2:"أوزبكستان", time:"2026-06-28T02:30:00", round:"third" },{ team1:"الجزائر", team2:"النمسا", time:"2026-06-28T05:00:00", round:"third" },
    { team1:"الأردن", team2:"الأرجنتين", time:"2026-06-28T05:00:00", round:"third" }
  ];
  const matchesData = rawMatches.map(m => ({ ...m, timeISO: m.time + "+03:00", roundLabel: m.round === 'first' ? 'الجولة الأولى' : (m.round === 'second' ? 'الجولة الثانية' : 'الجولة الثالثة') }));

  function renderUpcoming() {
    let active = upcomingMatches(matchesData);
    const round = document.getElementById('roundFilter').value;
    active = filterRound(active, round);
    active.sort((a,b) => matchTime(a.timeISO) - matchTime(b.timeISO));
    const container = document.getElementById('matchesContainer');
    if (!active.length) { container.innerHTML = `<div class="empty-state">📭 لا توجد مباريات قادمة</div>`; return; }
    container.innerHTML = active.map(m => {
      const st = getMatchStatus(m);
      const dateTimeDisplay = getDateTimeDisplay(m.timeISO);
      return `<div class="match-card ${st.live ? 'live-card' : ''}">
        <div class="teams"><div class="team"><span>${getFlag(m.team1)}</span> ${m.team1}</div><span class="vs">🆚</span><div class="team"><span>${getFlag(m.team2)}</span> ${m.team2}</div></div>
        <div class="datetime-row"><div class="match-day">${getDay(m.timeISO)}</div><div class="match-full-date"><span>${dateTimeDisplay}</span></div></div>
        <div class="info-row"><span class="round-tag">🏅 ${m.roundLabel}</span><div class="countdown-timer ${st.live ? 'live-status' : ''}">${st.live ? '🔴 تُلعب الآن 🔴' : st.text}</div></div>
      </div>`;
    }).join('');
  }

  // ------------------- الترجمة الدقيقة والمتقدمة للمباريات السابقة -----------------
  const nameMapping = new Map([
    ["آمریکا","أمريكا"],["United States","أمريكا"],["برزیل","البرازيل"],["Brazil","البرازيل"],["مراکش","المغرب"],["Morocco","المغرب"],
    ["هائیتی","هايتي"],["Haiti","هايتي"],["اسکاتلند","إسكتلندا"],["Scotland","إسكتلندا"],["آلمان","ألمانيا"],["Germany","ألمانيا"],
    ["کوزوو","كوراساو"],["Kosovo","كوراساو"],["Curaçao","كوراساو"],["هلند","هولندا"],["Netherlands","هولندا"],["ژاپن","اليابان"],
    ["Japan","اليابان"],["اکوادور","الإكوادور"],["Ecuador","الإكوادور"],["ساحل عاج","ساحل العاج"],["Ivory Coast","ساحل العاج"],
    ["سوئد","السويد"],["Sweden","السويد"],["تونس","تونس"],["Tunisia","تونس"],["اسپانیا","إسبانيا"],["Spain","إسبانيا"],
    ["کیپ ورد","الرأس الأخضر"],["Cape Verde","الرأس الأخضر"],["مصر","مصر"],["Egypt","مصر"],["بلژیک","بلجيكا"],["Belgium","بلجيكا"],
    ["عربستان سعودی","السعودية"],["Saudi Arabia","السعودية"],["اروگوئه","أوروغواي"],["Uruguay","أوروغواي"],["ایران","إيران"],
    ["Iran","إيران"],["نیوزیلند","نيوزيلندا"],["New Zealand","نيوزيلندا"],["سنگال","السنغال"],["Senegal","السنغال"],["فرانسه","فرنسا"],
    ["France","فرنسا"],["نروژ","النرويج"],["Norway","النرويج"],["انگلستان","إنجلترا"],["England","إنجلترا"],["کرواسی","كرواتيا"],
    ["Croatia","كرواتيا"],["پاناما","بنما"],["Panama","بنما"],["کلمبیا","كولومبيا"],["Colombia","كولومبيا"],["ازبکستان","أوزبكستان"],
    ["Uzbekistan","أوزبكستان"],["غنا","غانا"],["Ghana","غانا"],["پاراگوئه","باراغواي"],["Paraguay","باراغواي"],["بوسنی و هرزگوین","البوسنة والهرسك"],
    ["قطر","قطر"],["Qatar","قطر"],["کره جنوبی","كوريا الجنوبية"],["South Korea","كوريا الجنوبية"],["جمهوری چک","التشيك"],["Czech Republic","التشيك"],
    ["کانادا","كندا"],["Canada","كندا"],["عراق","العراق"],["Iraq","العراق"],["سوئیس","سويسرا"],["Switzerland","سويسرا"],
    ["استرالیا","أستراليا"],["Australia","أستراليا"],["ترکیه","تركيا"],["Turkey","تركيا"],["الجزایر","الجزائر"],["Algeria","الجزائر"],
    ["اتریش","النمسا"],["Austria","النمسا"],["اردن","الأردن"],["Jordan","الأردن"],["پرتغال","البرتغال"],["Portugal","البرتغال"],
    ["کنگو دمکراتیک","الكونغو الديمقراطية"],["DR Congo","الكونغو الديمقراطية"],["مکزیک","المكسيك"],["Mexico","المكسيك"],["آفریقای جنوبی","جنوب أفريقيا"],
    ["South Africa","جنوب أفريقيا"],["آرژانتین","الأرجنتين"],["Argentina","الأرجنتين"]
  ]);

  function translateToArabic(raw) {
    if (!raw) return "";
    let trimmed = raw.trim();
    if (nameMapping.has(trimmed)) return nameMapping.get(trimmed);
    // محاولة إضافية: تحويل النص إلى أحرف صغيرة ومقارنة بعض الكلمات
    for (let [key, value] of nameMapping) {
      if (key.toLowerCase() === trimmed.toLowerCase()) return value;
    }
    return trimmed;
  }

  let previousGamesData = [];

  async function loadPreviousGames() {
    const containerPrev = document.getElementById('previousMatchesContainer');
    try {
      const response = await fetch('https://worldcup26.ir/get/games');
      const data = await response.json();
      if (!data || !data.games) throw new Error("API error");
      const finished = data.games.filter(g => g.finished === "TRUE");
      previousGamesData = finished.map(game => {
        let homeRaw = game.home_team_name_fa || game.home_team_name_en || "";
        let awayRaw = game.away_team_name_fa || game.away_team_name_en || "";
        let homeAr = translateToArabic(homeRaw);
        let awayAr = translateToArabic(awayRaw);
        let homeScore = parseInt(game.home_score, 10);
        let awayScore = parseInt(game.away_score, 10);
        let dateStr = game.local_date || "";
        let dayName = "", formattedDate = "", timeMatch = "";
        if (dateStr) {
          let parts = dateStr.split(' ');
          let dateParts = parts[0]?.split('/');
          if (dateParts && dateParts.length === 3) {
            let d = new Date(`${dateParts[2]}-${dateParts[0]}-${dateParts[1]}T12:00:00`);
            dayName = ['الأحد','الاثنين','الثلاثاء','الأربعاء','الخميس','الجمعة','السبت'][d.getDay()];
            formattedDate = `${d.getDate()} ${['يناير','فبراير','مارس','أبريل','مايو','يونيو','يوليو','أغسطس','سبتمبر','أكتوبر','نوفمبر','ديسمبر'][d.getMonth()]} ${d.getFullYear()}`;
          } else { dayName = "تاريخ"; formattedDate = dateStr; }
          if (parts.length > 1 && parts[1]?.match(/\d{2}:\d{2}/)) timeMatch = parts[1];
        }
        return { homeAr, awayAr, homeScore, awayScore, dayName, formattedDate, timeMatch };
      });
      renderPreviousGamesFiltered();
      calculateStandings(); // الترتيب يتم حسابه من نفس البيانات
    } catch (err) {
      console.error(err);
      if(containerPrev) containerPrev.innerHTML = `<div class="empty-state">⚠️ فشل تحميل المباريات السابقة.</div>`;
    }
  }

  function renderPreviousGamesFiltered() {
    let games = previousGamesData;
    const searchText = document.getElementById('prevSearchInput')?.value.trim().toLowerCase() || "";
    let filtered = games;
    if (searchText) filtered = games.filter(g => g.homeAr.includes(searchText) || g.awayAr.includes(searchText));
    const container = document.getElementById('previousMatchesContainer');
    if (!filtered.length) { container.innerHTML = `<div class="empty-state">📋 لا توجد مباريات سابقة مطابقة.</div>`; return; }
    container.innerHTML = filtered.map(g => {
      const dateTimeDisplay = g.timeMatch ? `${g.formattedDate} - ${g.timeMatch}` : g.formattedDate;
      return `<div class="match-card">
        <div class="teams"><div class="team"><span>${getFlag(g.homeAr)}</span> ${g.homeAr}</div><span class="vs">🆚</span><div class="team"><span>${getFlag(g.awayAr)}</span> ${g.awayAr}</div></div>
        <div class="datetime-row"><div class="match-day">${g.dayName}</div><div class="match-full-date"><span>${dateTimeDisplay}</span></div></div>
        <div class="info-row"><span class="round-tag">🏅 النتيجة النهائية</span><div class="countdown-timer" style="background:#2c4b55;">${g.homeScore} - ${g.awayScore}</div></div>
      </div>`;
    }).join('');
  }

  // تعريف المجموعات النهائية حسب التوزيع المطلوب (بنفس الأسماء العربية الموحدة)
  const finalGroups = {
    "A": ["المكسيك","جنوب أفريقيا","كوريا الجنوبية","التشيك"],
    "B": ["كندا","البوسنة والهرسك","قطر","سويسرا"],
    "C": ["البرازيل","المغرب","هايتي","إسكتلندا"],
    "D": ["أمريكا","باراغواي","أستراليا","تركيا"],
    "E": ["ألمانيا","كوراساو","ساحل العاج","الإكوادور"],
    "F": ["هولندا","اليابان","السويد","تونس"],
    "G": ["بلجيكا","مصر","إيران","نيوزيلندا"],
    "H": ["إسبانيا","الرأس الأخضر","السعودية","أوروغواي"],
    "I": ["فرنسا","السنغال","النرويج","العراق"],
    "J": ["الأرجنتين","الجزائر","النمسا","الأردن"],
    "K": ["البرتغال","الكونغو الديمقراطية","أوزبكستان","كولومبيا"],
    "L": ["إنجلترا","كرواتيا","غانا","بنما"]
  };

  // حساب الترتيب بناءً على المباريات السابقة التي تم جلبها من API فقط
  function calculateStandings() {
    let standings = {};
    for (let [group, teams] of Object.entries(finalGroups)) {
      standings[group] = {};
      teams.forEach(team => { standings[group][team] = { played:0, wins:0, draws:0, losses:0, goalsFor:0, goalsAgainst:0, points:0 }; });
    }
    // تسجيل كل مباراة سابقة تنتمي إلى إحدى المجموعات
    previousGamesData.forEach(game => {
      const { homeAr, awayAr, homeScore, awayScore } = game;
      let groupName = null;
      for (let [g, teams] of Object.entries(finalGroups)) {
        if (teams.includes(homeAr) && teams.includes(awayAr)) {
          groupName = g;
          break;
        }
      }
      if (!groupName) return; // المباراة لا تنتمي لمجموعاتنا (ربما مباراة ودية أو خارج المجموعات)
      const stats = standings[groupName];
      if (!stats[homeAr] || !stats[awayAr]) return;
      stats[homeAr].played++; stats[awayAr].played++;
      stats[homeAr].goalsFor += homeScore; stats[homeAr].goalsAgainst += awayScore;
      stats[awayAr].goalsFor += awayScore; stats[awayAr].goalsAgainst += homeScore;
      if (homeScore > awayScore) {
        stats[homeAr].wins++; stats[homeAr].points += 3;
        stats[awayAr].losses++;
      } else if (awayScore > homeScore) {
        stats[awayAr].wins++; stats[awayAr].points += 3;
        stats[homeAr].losses++;
      } else {
        stats[homeAr].draws++; stats[awayAr].draws++;
        stats[homeAr].points += 1; stats[awayAr].points += 1;
      }
    });
    const container = document.getElementById('standingsContainer');
    let html = '';
    for (let [group, teamsStats] of Object.entries(standings)) {
      let tableRows = [];
      for (let [team, stat] of Object.entries(teamsStats)) {
        tableRows.push({ team, ...stat, goalDiff: stat.goalsFor - stat.goalsAgainst });
      }
      tableRows.sort((a,b) => {
        if (a.points !== b.points) return b.points - a.points;
        if (a.goalDiff !== b.goalDiff) return b.goalDiff - a.goalDiff;
        return b.goalsFor - a.goalsFor;
      });
      html += `<div class="group-card"><div class="group-title">المجموعة ${group}</div><table class="standings-table"><thead><tr><th>#</th><th>الفريق</th><th>لعب</th><th>ف</th><th>ت</th><th>خ</th><th>له</th><th>عليه</th><th>فارق</th><th>نقاط</th></tr></thead><tbody>`;
      tableRows.forEach((row, idx) => {
        html += `<tr><td>${idx+1}</td><td style="text-align:right;"><div class="team-name-td"><span>${getFlag(row.team)}</span> ${row.team}</div></td><td>${row.played}</td><td>${row.wins}</td><td>${row.draws}</td><td>${row.losses}</td><td>${row.goalsFor}</td><td>${row.goalsAgainst}</td><td>${row.goalDiff}</td><td>${row.points}</td></tr>`;
      });
      html += `</tbody></table></div>`;
    }
    container.innerHTML = html || `<div class="empty-state">📊 لا توجد نتائج كافية لحساب الترتيب بعد (يجب أن تنتهي بعض المباريات في API).</div>`;
  }

  // البحث الشامل (يعمل على البيانات الحالية)
  function performGlobalSearch() {
    const keyword = document.getElementById('globalSearchInput').value.trim();
    const searchContainer = document.getElementById('quickSearchResults');
    const keywordSpan = document.getElementById('searchKeyword');
    const resultsContainer = document.getElementById('quickResultsContainer');
    if (keyword === "") { searchContainer.classList.remove('visible'); return; }
    searchContainer.classList.add('visible');
    keywordSpan.innerText = keyword;
    let upcomingFiltered = upcomingMatches(matchesData).filter(m => m.team1.includes(keyword) || m.team2.includes(keyword));
    let previousFiltered = previousGamesData.filter(g => g.homeAr.includes(keyword) || g.awayAr.includes(keyword));
    let html = '';
    if (upcomingFiltered.length === 0 && previousFiltered.length === 0) {
      html = `<div class="empty-state" style="grid-column:1/-1; padding:20px;">❌ لا توجد مباريات قادمة أو سابقة تحمل اسم "${keyword}"</div>`;
    } else {
      if (upcomingFiltered.length) {
        html += `<div style="grid-column:1/-1; margin:5px 0 8px 0; font-weight:bold; color:#FFE0A3;">⚡ المباريات القادمة والجارية (${upcomingFiltered.length})</div>`;
        upcomingFiltered.forEach(m => {
          const st = getMatchStatus(m);
          const dateTimeDisplay = getDateTimeDisplay(m.timeISO);
          html += `<div class="quick-match-card"><div class="quick-match-teams"><span>${getFlag(m.team1)}</span> ${m.team1} 🆚 ${m.team2} <span>${getFlag(m.team2)}</span></div>
            <div class="quick-result">${st.live ? '🔴 تُلعب الآن' : (st.text.includes('h') ? '⏳ ' + st.text : '✅ انتهت')}</div>
            <div style="font-size:0.7rem; text-align:center;">${getDay(m.timeISO)} ${dateTimeDisplay}</div></div>`;
        });
      }
      if (previousFiltered.length) {
        html += `<div style="grid-column:1/-1; margin:15px 0 8px 0; font-weight:bold; color:#FFE0A3;">📋 المباريات السابقة (${previousFiltered.length})</div>`;
        previousFiltered.forEach(g => {
          const dateTimeDisplay = g.timeMatch ? `${g.formattedDate} - ${g.timeMatch}` : g.formattedDate;
          html += `<div class="quick-match-card"><div class="quick-match-teams"><span>${getFlag(g.homeAr)}</span> ${g.homeAr} 🆚 ${g.awayAr} <span>${getFlag(g.awayAr)}</span></div>
            <div class="quick-result">النتيجة: ${g.homeScore} - ${g.awayScore}</div>
            <div style="font-size:0.7rem; text-align:center;">${g.dayName} ${dateTimeDisplay}</div></div>`;
        });
      }
    }
    resultsContainer.innerHTML = html;
  }

  // التبويبات والأحداث
  function initTabs() {
    const btns = document.querySelectorAll('.tab-btn');
    btns.forEach(btn => {
      btn.addEventListener('click', () => {
        const id = btn.getAttribute('data-tab');
        document.querySelectorAll('.tab-content').forEach(t => t.classList.remove('active'));
        document.getElementById(`${id}Tab`).classList.add('active');
        btns.forEach(b => b.classList.remove('active'));
        btn.classList.add('active');
        if (id === 'previous' && previousGamesData.length === 0) loadPreviousGames();
        if (id === 'standings') {
          if (previousGamesData.length === 0) loadPreviousGames();
          else calculateStandings();
        }
      });
    });
  }

  function bindEvents() {
    document.getElementById('roundFilter').addEventListener('change', renderUpcoming);
    document.getElementById('prevSearchInput').addEventListener('input', renderPreviousGamesFiltered);
    document.getElementById('globalSearchInput').addEventListener('input', performGlobalSearch);
  }

  function startAutoUpdate() {
    setInterval(renderUpcoming, 1000);
    setInterval(() => {
      const activeTab = document.querySelector('.tab-btn.active')?.getAttribute('data-tab');
      if (activeTab === 'previous') loadPreviousGames();
      if (activeTab === 'standings') { if (previousGamesData.length) calculateStandings(); else loadPreviousGames(); }
      performGlobalSearch();
    }, 60000);
  }

  function init() {
    bindEvents();
    renderUpcoming();
    startAutoUpdate();
    initTabs();
    loadPreviousGames();
  }
  init();
</script>
</body>
</html>
