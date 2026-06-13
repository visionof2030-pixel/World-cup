<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
  <title>🏆 متتبع كأس العالم 2026 – مدرسة سعيد بن العاص</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(135deg, #0b2b2f 0%, #05181c 100%);
      font-family: 'Segoe UI', 'Cairo', system-ui, -apple-system, 'Roboto', sans-serif;
      padding: 16px;
      min-height: 100vh;
      color: #f0f9ff;
    }

    .app-container {
      max-width: 1200px;
      margin: 0 auto;
    }

    .hero {
      background: rgba(0, 15, 20, 0.65);
      backdrop-filter: blur(14px);
      border-radius: 56px;
      padding: 20px 24px;
      margin-bottom: 28px;
      text-align: center;
      border: 1px solid rgba(255, 180, 70, 0.5);
      box-shadow: 0 20px 35px -12px rgba(0,0,0,0.4);
    }

    .hero h1 {
      font-size: 1.9rem;
      background: linear-gradient(120deg, #FFE6B0, #FFB347);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      letter-spacing: -0.5px;
      margin-bottom: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
    }

    .hero h1 span {
      font-size: 2rem;
    }

    .school-badge {
      background: #1e4a5f;
      display: inline-block;
      padding: 8px 20px;
      border-radius: 60px;
      font-size: 0.9rem;
      font-weight: 600;
      color: #ffdfa5;
      box-shadow: inset 0 1px 2px #ffffff30, 0 4px 10px rgba(0,0,0,0.2);
      backdrop-filter: blur(4px);
      margin-top: 8px;
    }

    .control-panel {
      background: rgba(0, 22, 30, 0.7);
      backdrop-filter: blur(12px);
      border-radius: 60px;
      padding: 12px 20px;
      display: flex;
      flex-wrap: wrap;
      gap: 14px;
      margin-bottom: 32px;
      border: 1px solid #ffb34740;
    }

    .search-group {
      flex: 2;
      min-width: 160px;
    }

    .search-group input {
      width: 100%;
      padding: 14px 22px;
      border-radius: 50px;
      border: none;
      background: #fef7e0;
      font-size: 1rem;
      font-weight: 500;
      text-align: right;
      outline: none;
      transition: 0.2s;
      color: #1e2f36;
    }

    .search-group input:focus {
      box-shadow: 0 0 0 3px #ffb347;
      background: #fffaf0;
    }

    .round-group {
      flex: 1;
      min-width: 150px;
    }

    .round-group select {
      width: 100%;
      padding: 14px 16px;
      border-radius: 50px;
      border: none;
      background: #fef7e0;
      font-weight: bold;
      font-size: 0.9rem;
      cursor: pointer;
      text-align: center;
      outline: none;
    }

    .stats-card {
      background: #00000055;
      border-radius: 60px;
      padding: 8px 22px;
      display: flex;
      align-items: center;
      font-weight: bold;
      gap: 10px;
      font-size: 1rem;
      backdrop-filter: blur(4px);
      white-space: nowrap;
    }

    .matches-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
      gap: 22px;
    }

    .match-card {
      background: linear-gradient(145deg, #0e3843, #06232b);
      border-radius: 40px;
      padding: 18px;
      transition: all 0.25s ease;
      border: 1px solid #ffc97a30;
      box-shadow: 0 15px 30px -10px rgba(0,0,0,0.4);
      display: flex;
      flex-direction: column;
      gap: 14px;
    }

    .match-card.live-card {
      border: 2px solid #ff3a2f;
      background: linear-gradient(145deg, #1c4a55, #0a2e36);
      box-shadow: 0 0 15px rgba(255, 58, 47, 0.4);
    }

    .teams {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      background: #021d24a0;
      padding: 12px 12px;
      border-radius: 60px;
      font-weight: 800;
    }

    .team {
      background: #00000055;
      padding: 8px 12px;
      border-radius: 50px;
      font-size: 1rem;
      flex: 1;
      text-align: center;
      font-weight: 700;
      white-space: nowrap;
      overflow-x: auto;
      -webkit-overflow-scrolling: touch;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
    }

    .team span:first-child {
      font-size: 1.3rem;
    }

    .vs {
      background: #FFB347;
      color: #1e2a2f;
      padding: 5px 12px;
      border-radius: 40px;
      font-weight: bold;
      font-size: 0.85rem;
    }

    .info-row {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 4px;
    }

    .round-tag {
      background: #263b44;
      padding: 5px 14px;
      border-radius: 60px;
      font-size: 0.75rem;
      font-weight: bold;
      color: #FFE0A3;
      border-right: 3px solid #ffb347;
    }

    .countdown-timer {
      background: #00000070;
      font-family: 'JetBrains Mono', monospace;
      font-size: 1.2rem;
      font-weight: bold;
      direction: ltr;
      text-align: center;
      padding: 8px 12px;
      border-radius: 60px;
      backdrop-filter: blur(4px);
    }

    .live-status {
      background: #d32f2f;
      color: white;
      font-weight: bold;
      padding: 6px 16px;
      border-radius: 40px;
      font-size: 0.85rem;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      animation: pulse 1.2s infinite;
    }

    @keyframes pulse {
      0% { opacity: 0.7; background: #b71c1c; }
      50% { opacity: 1; background: #f44336; box-shadow: 0 0 8px red; }
      100% { opacity: 0.7; background: #b71c1c; }
    }

    .empty-state {
      grid-column: 1 / -1;
      text-align: center;
      background: #102e36b3;
      padding: 48px 20px;
      border-radius: 70px;
      font-size: 1.3rem;
      backdrop-filter: blur(8px);
    }

    footer {
      margin-top: 48px;
      text-align: center;
      font-size: 0.75rem;
      color: #90b8c2;
      border-top: 1px dashed #ffb34760;
      padding-top: 24px;
    }

    @media (max-width: 550px) {
      body { padding: 12px; }
      .hero h1 { font-size: 1.4rem; }
      .team { font-size: 0.85rem; white-space: normal; word-break: keep-all; }
      .countdown-timer { font-size: 0.9rem; }
      .control-panel { border-radius: 40px; padding: 12px; }
      .stats-card { padding: 6px 18px; font-size: 0.8rem; }
    }
  </style>
</head>
<body>
<div class="app-container">
  <div class="hero">
    <h1><span>🏆</span> كأس العالم 2026 <span>⚽</span></h1>
    <div class="school-badge">📢 تابع كأس العالم في غرفة معلمي مدرسة سعيد بن العاص</div>
    <p style="margin-top: 12px; font-size: 0.85rem; opacity: 0.9;">⏳ العد التنازلي + متابعة المباريات الحية 🔴 + أعلام الدول 🏁</p>
  </div>

  <div class="control-panel">
    <div class="search-group">
      <input type="text" id="searchTeamInput" placeholder="🔍 ابحث عن منتخب ... (مصر، البرازيل، السعودية)" autocomplete="off">
    </div>
    <div class="round-group">
      <select id="roundFilter">
        <option value="all">🌍 جميع الجولات</option>
        <option value="first">🟢 الجولة الأولى</option>
        <option value="second">🟩 الجولة الثانية</option>
        <option value="third">🟥 الجولة الثالثة</option>
      </select>
    </div>
    <div class="stats-card" id="matchesCounter">🕒 جار التحميل</div>
  </div>

  <div id="matchesContainer" class="matches-grid">
    <div class="empty-state">✨ جاري تحديث المباريات ✨</div>
  </div>
  <footer>🔄 تحديث تلقائي كل ثانية | المباريات المُباشرة تظهر بحد أحمر وعلامة LIVE 🔴 | توقيت مكة المكرمة (UTC+3)</footer>
</div>

<script>
  // =========================
  // 🧠 Core functions (World Cup Tracker)
  // =========================
  function now() {
    return new Date().getTime();
  }

  function matchTime(timeISO) {
    return new Date(timeISO).getTime();
  }

  // مدة المباراة بالمللي ثانية (105 دقيقة)
  const MATCH_DURATION_MS = 105 * 60 * 1000;

  function getMatchStatus(match) {
    const start = matchTime(match.timeISO);
    const end = start + MATCH_DURATION_MS;
    const current = now();
    
    if (current < start) {
      const diff = start - current;
      const h = Math.floor(diff / (1000 * 60 * 60));
      const m = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      const s = Math.floor((diff % (1000 * 60)) / 1000);
      return { type: 'upcoming', text: `⏱️ ${h}h ${m}m ${s}s`, live: false };
    } 
    else if (current >= start && current <= end) {
      return { type: 'live', text: '🔴 تُلعب الآن 🔴', live: true };
    } 
    else {
      return { type: 'finished', text: '✅ انتهت', live: false };
    }
  }

  function upcomingMatches(matchesArray) {
    return matchesArray.filter(m => (matchTime(m.timeISO) + MATCH_DURATION_MS) > now());
  }

  function searchTeam(matchesArray, teamName) {
    if (!teamName.trim()) return matchesArray;
    return matchesArray.filter(m => m.team1.includes(teamName) || m.team2.includes(teamName));
  }

  function filterRound(matchesArray, roundKey) {
    if (roundKey === "all") return matchesArray;
    return matchesArray.filter(m => m.round === roundKey);
  }

  function autoUpdate(renderCallback) {
    setInterval(renderCallback, 1000);
  }

  // =========================
  // 🏁 أعلام الدول (إيموجي)
  // =========================
  function getFlag(teamName) {
    const flagMap = {
      "المكسيك": "🇲🇽", "جنوب أفريقيا": "🇿🇦", "الأرجنتين": "🇦🇷", "الجزائر": "🇩🇿",
      "النمسا": "🇦🇹", "الأردن": "🇯🇴", "البرتغال": "🇵🇹", "الكونغو الديمقراطية": "🇨🇩",
      "كوريا الجنوبية": "🇰🇷", "التشيك": "🇨🇿", "كندا": "🇨🇦", "البوسنة والهرسك": "🇧🇦",
      "أمريكا": "🇺🇸", "العراق": "🇮🇶", "سويسرا": "🇨🇭", "قطر": "🇶🇦",
      "البرازيل": "🇧🇷", "المغرب": "🇲🇦", "هايتي": "🇭🇹", "إسكتلندا": "🏴󠁧󠁢󠁳󠁣󠁴󠁿",
      "أستراليا": "🇦🇺", "تركيا": "🇹🇷", "ألمانيا": "🇩🇪", "كوسوفو": "🇽🇰",
      "اليابان": "🇯🇵", "هولندا": "🇳🇱", "الإكوادور": "🇪🇨", "ساحل العاج": "🇨🇮",
      "السويد": "🇸🇪", "تونس": "🇹🇳", "إسبانيا": "🇪🇸", "الرأس الأخضر": "🇨🇻",
      "مصر": "🇪🇬", "بلجيكا": "🇧🇪", "السعودية": "🇸🇦", "أوروغواي": "🇺🇾",
      "إيران": "🇮🇷", "نيوزيلندا": "🇳🇿", "السنغال": "🇸🇳", "فرنسا": "🇫🇷",
      "النرويج": "🇳🇴", "إنجلترا": "🏴󠁧󠁢󠁥󠁮󠁧󠁿", "كرواتيا": "🇭🇷", "بنما": "🇵🇦",
      "كولومبيا": "🇨🇴", "أوزبكستان": "🇺🇿", "غانا": "🇬🇭", "باراغواي": "🇵🇾"
    };
    // معالجة إسكتلندا، إنجلترا بعلم إيموجي علم اسكتلندا غير مدعوم عالمياً في كل الأجهزة لكننا نستخدم العلم الأسكتلندي التقريبي
    if (teamName === "إسكتلندا") return "🏴󠁧󠁢󠁳󠁣󠁴󠁿";
    if (teamName === "إنجلترا") return "🏴󠁧󠁢󠁥󠁮󠁧󠁿";
    return flagMap[teamName] || "🏁";
  }

  // =========================
  // 📅 بيانات المباريات كاملة
  // =========================
  const rawMatches = [
    { team1: "المكسيك", team2: "جنوب أفريقيا", time: "2026-06-11T22:00:00", round: "first" },
    { team1: "الأرجنتين", team2: "الجزائر", time: "2026-06-11T04:00:00", round: "first" },
    { team1: "النمسا", team2: "الأردن", time: "2026-06-11T07:00:00", round: "first" },
    { team1: "البرتغال", team2: "الكونغو الديمقراطية", time: "2026-06-11T20:00:00", round: "first" },
    { team1: "كوريا الجنوبية", team2: "التشيك", time: "2026-06-12T05:00:00", round: "first" },
    { team1: "كندا", team2: "البوسنة والهرسك", time: "2026-06-12T22:00:00", round: "first" },
    { team1: "أمريكا", team2: "العراق", time: "2026-06-13T04:00:00", round: "first" },
    { team1: "سويسرا", team2: "قطر", time: "2026-06-13T22:00:00", round: "first" },
    { team1: "البرازيل", team2: "المغرب", time: "2026-06-14T01:00:00", round: "first" },
    { team1: "هايتي", team2: "إسكتلندا", time: "2026-06-14T04:00:00", round: "first" },
    { team1: "أستراليا", team2: "تركيا", time: "2026-06-14T07:00:00", round: "first" },
    { team1: "ألمانيا", team2: "كوسوفو", time: "2026-06-14T20:00:00", round: "first" },
    { team1: "اليابان", team2: "هولندا", time: "2026-06-14T23:00:00", round: "first" },
    { team1: "الإكوادور", team2: "ساحل العاج", time: "2026-06-15T02:00:00", round: "first" },
    { team1: "السويد", team2: "تونس", time: "2026-06-15T05:00:00", round: "first" },
    { team1: "إسبانيا", team2: "الرأس الأخضر", time: "2026-06-15T19:00:00", round: "first" },
    { team1: "مصر", team2: "بلجيكا", time: "2026-06-15T22:00:00", round: "first" },
    { team1: "السعودية", team2: "أوروغواي", time: "2026-06-16T01:00:00", round: "first" },
    { team1: "إيران", team2: "نيوزيلندا", time: "2026-06-16T04:00:00", round: "first" },
    { team1: "السنغال", team2: "فرنسا", time: "2026-06-16T22:00:00", round: "first" },
    { team1: "النرويج", team2: "العراق", time: "2026-06-17T01:00:00", round: "first" },
    { team1: "الجزائر", team2: "الأرجنتين", time: "2026-06-17T04:00:00", round: "first" },
    { team1: "الأردن", team2: "النمسا", time: "2026-06-17T07:00:00", round: "first" },
    { team1: "البرتغال", team2: "كرواتيا", time: "2026-06-17T20:00:00", round: "first" },
    { team1: "إنجلترا", team2: "كرواتيا", time: "2026-06-17T23:00:00", round: "first" },
    { team1: "جنوب أفريقيا", team2: "التشيك", time: "2026-06-18T19:00:00", round: "second" },
    { team1: "سويسرا", team2: "البوسنة والهرسك", time: "2026-06-18T22:00:00", round: "second" },
    { team1: "قطر", team2: "كندا", time: "2026-06-19T01:00:00", round: "second" },
    { team1: "المكسيك", team2: "كوريا الجنوبية", time: "2026-06-19T04:00:00", round: "second" },
    { team1: "أستراليا", team2: "أمريكا", time: "2026-06-19T22:00:00", round: "second" },
    { team1: "المغرب", team2: "إسكتلندا", time: "2026-06-20T01:00:00", round: "second" },
    { team1: "البرازيل", team2: "هايتي", time: "2026-06-20T03:30:00", round: "second" },
    { team1: "تركيا", team2: "باراغواي", time: "2026-06-20T06:00:00", round: "second" },
    { team1: "السويد", team2: "هولندا", time: "2026-06-20T20:00:00", round: "second" },
    { team1: "ساحل العاج", team2: "ألمانيا", time: "2026-06-20T23:00:00", round: "second" },
    { team1: "الإكوادور", team2: "كوسوفو", time: "2026-06-21T03:00:00", round: "second" },
    { team1: "اليابان", team2: "تونس", time: "2026-06-21T07:00:00", round: "second" },
    { team1: "إسبانيا", team2: "السعودية", time: "2026-06-21T19:00:00", round: "second" },
    { team1: "بلجيكا", team2: "إيران", time: "2026-06-21T22:00:00", round: "second" },
    { team1: "أوروجواي", team2: "الرأس الأخضر", time: "2026-06-22T01:00:00", round: "second" },
    { team1: "مصر", team2: "نيوزيلندا", time: "2026-06-22T04:00:00", round: "second" },
    { team1: "الأرجنتين", team2: "النمسا", time: "2026-06-22T20:00:00", round: "second" },
    { team1: "العراق", team2: "فرنسا", time: "2026-06-23T00:00:00", round: "second" },
    { team1: "النرويج", team2: "السنغال", time: "2026-06-23T03:00:00", round: "second" },
    { team1: "الأردن", team2: "الجزائر", time: "2026-06-23T06:00:00", round: "second" },
    { team1: "البرتغال", team2: "أوزبكستان", time: "2026-06-23T20:00:00", round: "second" },
    { team1: "إنجلترا", team2: "غانا", time: "2026-06-23T23:00:00", round: "second" },
    { team1: "بنما", team2: "كرواتيا", time: "2026-06-24T02:00:00", round: "second" },
    { team1: "كولومبيا", team2: "الكونغو الديمقراطية", time: "2026-06-24T05:00:00", round: "second" },
    { team1: "كندا", team2: "سويسرا", time: "2026-06-24T22:00:00", round: "third" },
    { team1: "قطر", team2: "البوسنة والهرسك", time: "2026-06-24T22:00:00", round: "third" },
    { team1: "المغرب", team2: "هايتي", time: "2026-06-25T01:00:00", round: "third" },
    { team1: "اسكتلندا", team2: "البرازيل", time: "2026-06-25T01:00:00", round: "third" },
    { team1: "جنوب أفريقيا", team2: "كوريا الجنوبية", time: "2026-06-25T04:00:00", round: "third" },
    { team1: "المكسيك", team2: "التشيك", time: "2026-06-25T04:00:00", round: "third" },
    { team1: "كوسوفو", team2: "ساحل العاج", time: "2026-06-25T23:00:00", round: "third" },
    { team1: "ألمانيا", team2: "الإكوادور", time: "2026-06-25T23:00:00", round: "third" },
    { team1: "هولندا", team2: "تونس", time: "2026-06-26T02:00:00", round: "third" },
    { team1: "اليابان", team2: "السويد", time: "2026-06-26T02:00:00", round: "third" },
    { team1: "أمريكا", team2: "تركيا", time: "2026-06-26T05:00:00", round: "third" },
    { team1: "أستراليا", team2: "باراغواي", time: "2026-06-26T05:00:00", round: "third" },
    { team1: "فرنسا", team2: "النرويج", time: "2026-06-26T22:00:00", round: "third" },
    { team1: "السنغال", team2: "العراق", time: "2026-06-26T22:00:00", round: "third" },
    { team1: "السعودية", team2: "الرأس الأخضر", time: "2026-06-27T03:00:00", round: "third" },
    { team1: "إسبانيا", team2: "أوروجواي", time: "2026-06-27T03:00:00", round: "third" },
    { team1: "إيران", team2: "مصر", time: "2026-06-27T06:00:00", round: "third" },
    { team1: "نيوزيلندا", team2: "بلجيكا", time: "2026-06-27T06:00:00", round: "third" },
    { team1: "إنجلترا", team2: "بنما", time: "2026-06-28T00:00:00", round: "third" },
    { team1: "كرواتيا", team2: "غانا", time: "2026-06-28T00:00:00", round: "third" },
    { team1: "البرتغال", team2: "كولومبيا", time: "2026-06-28T02:30:00", round: "third" },
    { team1: "الكونغو الديمقراطية", team2: "أوزبكستان", time: "2026-06-28T02:30:00", round: "third" },
    { team1: "الجزائر", team2: "النمسا", time: "2026-06-28T05:00:00", round: "third" },
    { team1: "الأردن", team2: "الأرجنتين", time: "2026-06-28T05:00:00", round: "third" }
  ];

  const matches = rawMatches.map(m => ({
    ...m,
    timeISO: m.time + "+03:00",
    roundLabel: m.round === 'first' ? 'الجولة الأولى' : (m.round === 'second' ? 'الجولة الثانية' : 'الجولة الثالثة')
  }));

  // عرض الواجهة الرئيسية مع الأعلام
  function renderMatchesUI() {
    let activeMatches = upcomingMatches(matches);
    const searchVal = document.getElementById('searchTeamInput').value.trim();
    if (searchVal !== "") activeMatches = searchTeam(activeMatches, searchVal);
    const roundVal = document.getElementById('roundFilter').value;
    activeMatches = filterRound(activeMatches, roundVal);
    activeMatches.sort((a,b) => matchTime(a.timeISO) - matchTime(b.timeISO));
    
    const container = document.getElementById('matchesContainer');
    const counterSpan = document.getElementById('matchesCounter');
    counterSpan.innerHTML = `🏟️ ${activeMatches.length} مباراة (حية / قادمة)`;
    
    if (activeMatches.length === 0) {
      container.innerHTML = `<div class="empty-state">📭 لا توجد مباريات قادمة أو حية حسب الفلتر<br>⚡ غير البحث أو الجولة</div>`;
      return;
    }
    
    container.innerHTML = activeMatches.map(match => {
      const status = getMatchStatus(match);
      const isLive = status.live;
      const statusText = status.text;
      const extraClass = isLive ? 'live-card' : '';
      const flag1 = getFlag(match.team1);
      const flag2 = getFlag(match.team2);
      
      return `
        <div class="match-card ${extraClass}">
          <div class="teams">
            <div class="team"><span>${flag1}</span> <span>${match.team1}</span></div>
            <span class="vs">🆚</span>
            <div class="team"><span>${flag2}</span> <span>${match.team2}</span></div>
          </div>
          <div class="info-row">
            <span class="round-tag">🏅 ${match.roundLabel}</span>
            <div class="countdown-timer ${isLive ? 'live-status' : ''}" style="${isLive ? 'background: none; padding: 0;' : ''}">
              ${isLive ? '<span style="background:#d32f2f; padding:6px 14px; border-radius:40px; animation: pulse 1.2s infinite;">🔴 تُلعب الآن 🔴</span>' : statusText}
            </div>
          </div>
        </div>
      `;
    }).join('');
  }
  
  function bindEvents() {
    document.getElementById('searchTeamInput').addEventListener('input', () => renderMatchesUI());
    document.getElementById('roundFilter').addEventListener('change', () => renderMatchesUI());
  }
  
  function startLiveUpdates() {
    autoUpdate(() => renderMatchesUI());
  }
  
  function init() {
    bindEvents();
    renderMatchesUI();
    startLiveUpdates();
  }
  
  init();
</script>
</body>
</html>
