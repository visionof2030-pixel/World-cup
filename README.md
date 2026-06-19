<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
  <title>🏆 كأس العالم 2026 – متتبع المباريات + توقعات + ترتيب</title>
  <style>
    /* ========== الأنماط الأساسية ========== */
    * { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
    body { background: radial-gradient(circle at 10% 20%, #0a1f24, #030c10); font-family: 'Segoe UI', 'Cairo', 'Inter', system-ui, -apple-system, 'Roboto', sans-serif; padding: 20px 12px; min-height: 100vh; color: #f0f9ff; font-size: 14px; }
    .app-container { max-width: 1200px; margin: 0 auto; width: 100%; }
    
    /* ===== الهيدر العلوي الكامل مع خلفية الصورة ===== */
    .main-header {
      width: 100%;
      height: 80px;
      min-height: 80px;
      padding: 0;
      border-radius: 80px 89px 0 0;
      overflow: hidden;
      margin-bottom: 0;
      position: relative;
      background-image: url('https://i.ibb.co/7dmWpzn2/IMG-3949.png');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
    }
    
    /* طبقة شفافة فوق الخلفية */
    .main-header::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(10, 20, 25, 0.5);
      border-radius: 48px 48px 0 0;
    }
    
    /* ===== البار العلوي ===== */
    .upper-bar {
      background: rgba(10, 20, 25, 0.92);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      border-radius: 0 0 48px 48px;
      padding: 0 24px;
      margin-bottom: 16px;
      position: relative;
      height: 80px;
      min-height: 80px;
      border: 1px solid rgba(255, 255, 255, 0.08);
      border-top: none;
      box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
      display: flex;
      align-items: center;
    }
    .upper-bar .bar-content {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 12px;
      width: 100%;
    }
    .upper-bar .title-section h1 {
      font-size: 1.3rem;
      font-weight: 800;
      color: #FFE6B0;
      text-shadow: 0 2px 15px rgba(0, 0, 0, 0.5);
      letter-spacing: -0.5px;
      margin: 0;
    }
    .upper-bar .developer-credit {
      font-size: 0.7rem;
      color: rgba(255, 230, 176, 0.8);
      text-align: center;
      margin-top: 2px;
      font-style: italic;
      letter-spacing: 0.5px;
      text-shadow: 0 1px 10px rgba(0, 0, 0, 0.3);
    }
    .upper-bar .header-actions {
      display: flex;
      gap: 8px;
      align-items: center;
    }
    .upper-bar .bar-btn {
      background: rgba(255, 255, 255, 0.08);
      color: #FFE6B0;
      border: 1px solid rgba(255, 255, 255, 0.15);
      padding: 8px 16px;
      border-radius: 12px;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      gap: 6px;
      backdrop-filter: blur(10px);
      font-size: 0.8rem;
      text-shadow: 0 1px 10px rgba(0, 0, 0, 0.2);
    }
    .upper-bar .bar-btn:hover {
      background: rgba(255, 255, 255, 0.15);
      transform: translateY(-2px);
      box-shadow: 0 0 25px rgba(255, 180, 70, 0.2);
      border-color: rgba(255, 180, 70, 0.3);
    }
    
    /* ===== شريط الأخبار المتحرك ===== */
    .news-ticker-wrapper {
      background: linear-gradient(90deg, rgba(26, 47, 47, 0.9), rgba(42, 65, 75, 0.9), rgba(26, 47, 47, 0.9));
      border: 1px solid rgba(255, 180, 70, 0.2);
      border-radius: 60px;
      padding: 6px 16px;
      margin-bottom: 16px;
      overflow: hidden;
      position: relative;
      box-shadow: 0 0 20px rgba(255, 180, 70, 0.05);
      backdrop-filter: blur(10px);
    }
    .news-ticker {
      display: inline-block;
      white-space: nowrap;
      animation: tickerScroll 42s linear infinite;
      font-size: 0.8rem;
      color: #FFE6B0;
      font-weight: 500;
      letter-spacing: 0.3px;
    }
    .news-ticker span {
      display: inline-block;
      padding: 0 16px;
    }
    .news-ticker .separator {
      color: #ffb34760;
    }
    @keyframes tickerScroll {
      0% { transform: translateX(-100%); }
      100% { transform: translateX(100%); }
    }
    .news-ticker-wrapper:hover .news-ticker {
      animation-play-state: paused;
    }
    
    .hero {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(20px);
      border-radius: 48px;
      padding: 20px;
      margin-bottom: 28px;
      text-align: center;
      border: 1px solid rgba(255, 200, 100, 0.3);
      box-shadow: 0 15px 35px rgba(0,0,0,0.2);
    }
    .hero h1 { 
      font-size: 1.8rem; 
      background: linear-gradient(135deg, #FFE6B0, #FFA559, #FF6A3D); 
      -webkit-background-clip: text; 
      background-clip: text; 
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
    
    /* ===== إخفاء النص العلوي "World-cup" ===== */
    /* هذا يستهدف أي نص يظهر في أعلى الصفحة من الصورة */
    .main-header .header-text,
    .main-header h1,
    .main-header .world-cup-text,
    .main-header [class*="world"],
    .main-header [class*="cup"] {
      display: none !important;
    }
    
    /* تغطية الجزء العلوي بالكامل */
    .main-header {
      position: relative;
    }
    
    /* طبقة إضافية لتغطية أي نص علوي */
    .main-header::after {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(10, 20, 25, 0.3);
      border-radius: 48px 48px 0 0;
      pointer-events: none;
    }
    
    .leaderboard-section { background: rgba(18, 38, 44, 0.85); backdrop-filter: blur(12px); border-radius: 32px; padding: 20px; margin-bottom: 28px; border: 2px solid rgba(255, 180, 70, 0.4); box-shadow: 0 0 30px rgba(255, 180, 70, 0.1); }
    .leaderboard-section .section-title { font-size: 1.5rem; font-weight: 800; color: #FFE6B0; text-align: center; margin-bottom: 16px; letter-spacing: -0.5px; }
    .leaderboard-section .section-title .trophy { font-size: 1.8rem; }
    .leaderboard-grid { display: grid; grid-template-columns: 1fr; gap: 10px; }
    .leaderboard-item { background: rgba(0, 0, 0, 0.3); backdrop-filter: blur(8px); border-radius: 24px; padding: 14px 18px; border: 1px solid rgba(255, 180, 70, 0.2); transition: 0.2s; display: flex; justify-content: space-between; align-items: center; }
    .leaderboard-item:hover { transform: translateX(-4px); border-color: #ffb347aa; }
    .leaderboard-item .rank { font-size: 1.2rem; font-weight: 800; color: #ffb347; min-width: 50px; }
    .leaderboard-item .rank.gold { color: #FFD700; }
    .leaderboard-item .rank.silver { color: #C0C0C0; }
    .leaderboard-item .rank.bronze { color: #CD7F32; }
    .leaderboard-item .player-name { font-size: 1rem; font-weight: 600; flex: 1; margin: 0 12px; }
    .leaderboard-item .player-name .avatar-small { display: inline-block; width: 28px; height: 28px; border-radius: 50%; background: linear-gradient(135deg, #ffb347, #ff8c1a); text-align: center; line-height: 28px; font-weight: 800; color: #1a2f2f; margin-left: 8px; font-size: 0.8rem; }
    .leaderboard-item .points { background: linear-gradient(135deg, #ffb347, #ff8c1a); padding: 4px 18px; border-radius: 40px; font-weight: 800; color: #1a2f2f; font-size: 0.9rem; min-width: 60px; text-align: center; }
    .leaderboard-item .medal { font-size: 1.5rem; margin-left: 8px; }
    
    .control-panel { background: rgba(10, 25, 30, 0.6); backdrop-filter: blur(16px); border-radius: 80px; padding: 8px 20px; display: flex; flex-wrap: wrap; align-items: center; gap: 12px; margin-bottom: 28px; border: 1px solid rgba(255, 200, 100, 0.25); }
    .search-group { flex: 2; min-width: 160px; }
    .search-group input { width: 100%; padding: 12px 20px; border-radius: 60px; border: none; background: #fef9e6; text-align: right; outline: none; font-size: 0.85rem; font-weight: 500; transition: 0.2s; box-shadow: 0 2px 6px rgba(0,0,0,0.1); }
    .search-group input:focus { transform: scale(0.98); box-shadow: 0 0 0 2px #ffb347; }
    .round-group { flex: 1; min-width: 130px; }
    .round-group select { width: 100%; padding: 12px 12px; border-radius: 60px; background: #fef9e6; font-weight: bold; cursor: pointer; font-size: 0.8rem; border: none; outline: none; font-family: inherit; }
    .tabs { display: flex; flex-wrap: wrap; gap: 12px; margin: 20px 0 24px; justify-content: center; }
    .tab-btn { background: rgba(20, 40, 48, 0.7); backdrop-filter: blur(8px); border: 1px solid rgba(255, 180, 70, 0.4); padding: 10px 20px; border-radius: 60px; font-size: 0.85rem; font-weight: 600; cursor: pointer; color: #ffefa6; transition: all 0.2s ease; display: inline-flex; align-items: center; gap: 8px; letter-spacing: 0.3px; }
    .tab-btn i { font-style: normal; font-size: 1.1rem; }
    .tab-btn.active { background: linear-gradient(105deg, #ffb347, #ff8c1a); color: #1a2f2f; border-color: #ffdd99; box-shadow: 0 8px 18px rgba(255, 140, 26, 0.25); }
    .tab-btn:hover:not(.active) { background: rgba(255, 180, 70, 0.2); border-color: #ffb347; transform: translateY(-2px); }
    .tab-content { display: none; animation: fadeSlide 0.25s ease; }
    .tab-content.active { display: block; }
    @keyframes fadeSlide { from { opacity: 0; transform: translateY(6px); } to { opacity: 1; transform: translateY(0); } }
    .matches-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(330px, 1fr)); gap: 22px; }
    .match-card { background: rgba(18, 38, 44, 0.75); backdrop-filter: blur(12px); border-radius: 32px; padding: 16px; border: 1px solid rgba(255, 180, 70, 0.3); transition: all 0.25s; box-shadow: 0 12px 24px -12px rgba(0,0,0,0.4); }
    .match-card:hover { transform: translateY(-3px); border-color: #ffb347aa; box-shadow: 0 20px 30px -12px black; }
    .match-card.live-card { border: 2px solid #ff4d4d; background: linear-gradient(135deg, #2a414b, #0f2e36); box-shadow: 0 0 12px rgba(255, 60, 30, 0.4); }
    
    .teams-score { display: flex; justify-content: space-between; align-items: center; gap: 8px; background: rgba(0, 0, 0, 0.3); padding: 10px 12px; border-radius: 80px; }
    .team { background: rgba(0, 0, 0, 0.4); padding: 6px 12px; border-radius: 60px; flex: 1; text-align: center; display: flex; align-items: center; justify-content: center; gap: 8px; font-weight: 700; font-size: 0.85rem; white-space: nowrap; overflow-x: auto; }
    .team span:first-child { font-size: 1.2rem; }
    
    .score-display { background: linear-gradient(135deg, #ffb347, #ff8c1a); padding: 4px 16px; border-radius: 40px; font-weight: 800; font-size: 1rem; color: #1a2f2f; min-width: 50px; text-align: center; box-shadow: 0 0 15px rgba(255, 180, 70, 0.3); letter-spacing: 1px; border: 1px solid rgba(255, 200, 100, 0.5); }
    .score-display.finished { background: linear-gradient(135deg, #4CAF50, #45a049); box-shadow: 0 0 15px rgba(76, 175, 80, 0.3); border-color: rgba(76, 175, 80, 0.5); }
    .score-display.live-score { background: linear-gradient(135deg, #ff4444, #cc0000); animation: scorePulse 1s infinite; box-shadow: 0 0 20px rgba(255, 68, 68, 0.5); border-color: rgba(255, 68, 68, 0.7); }
    @keyframes scorePulse { 0% { transform: scale(1); } 50% { transform: scale(1.05); } 100% { transform: scale(1); } }
    
    .vs-badge { background: rgba(255, 180, 70, 0.2); padding: 2px 8px; border-radius: 20px; font-size: 0.6rem; color: #ffb347; font-weight: 600; }
    
    .datetime-row { display: flex; justify-content: space-between; gap: 10px; background: rgba(0, 0, 0, 0.35); padding: 8px 14px; border-radius: 50px; flex-wrap: wrap; margin-top: 6px; }
    .match-day { background: #1e4a5f; padding: 4px 12px; border-radius: 40px; font-size: 0.7rem; font-weight: 600; }
    .match-full-date { background: rgba(0, 0, 0, 0.5); padding: 4px 12px; border-radius: 40px; font-size: 0.7rem; display: flex; gap: 6px; align-items: baseline; }
    .info-row { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 10px; margin-top: 4px; }
    .round-tag { background: #2f5663; padding: 4px 14px; border-radius: 60px; font-size: 0.7rem; font-weight: 500; }
    .countdown-timer { background: #00000070; font-family: monospace; font-size: 0.9rem; font-weight: bold; padding: 4px 14px; border-radius: 60px; text-align: center; letter-spacing: 0.5px; }
    .live-status { animation: pulse 1.2s infinite; background: #d32f2f; }
    @keyframes pulse { 0% { opacity: 0.75; background: #b71c1c; box-shadow: 0 0 0 0 #ff5e5e; } 50% { opacity: 1; background: #f44336; box-shadow: 0 0 0 3px rgba(255, 68, 34, 0.4); } 100% { opacity: 0.75; background: #b71c1c; } }
    
    .empty-state { grid-column: 1/-1; text-align: center; background: rgba(12, 34, 40, 0.7); backdrop-filter: blur(8px); padding: 40px 20px; border-radius: 60px; font-size: 1rem; border: 1px dashed #ffb34780; }
    .filter-bar { margin-bottom: 24px; background: rgba(0, 0, 0, 0.25); padding: 8px 16px; border-radius: 80px; display: flex; }
    .filter-bar input { background: #fef7e0; border: none; padding: 12px 20px; border-radius: 60px; width: 100%; font-size: 0.85rem; outline: none; }
    .groups-container { display: grid; grid-template-columns: repeat(auto-fill, minmax(360px, 1fr)); gap: 24px; }
    .group-card { background: rgba(30, 60, 72, 0.65); backdrop-filter: blur(12px); border-radius: 32px; padding: 16px; border: 1px solid #ffb34760; transition: 0.2s; }
    .group-title { font-size: 1.4rem; font-weight: 800; text-align: center; margin-bottom: 16px; color: #FFE6B0; letter-spacing: -0.5px; }
    .standings-table { width: 100%; border-collapse: collapse; font-size: 0.7rem; min-width: 320px; }
    .standings-table th, .standings-table td { padding: 8px 4px; text-align: center; }
    .standings-table th { background: #1e4655; color: #FFE0A3; font-weight: 700; border-radius: 16px 16px 0 0; }
    .standings-table td { background-color: #f3f7f9; color: #11242a; font-weight: 600; border-bottom: 1px solid #cddce0; }
    .team-name-td { text-align: right; display: flex; align-items: center; gap: 6px; justify-content: flex-start; }
    .quick-search-results { background: rgba(0, 25, 30, 0.92); backdrop-filter: blur(24px); border-radius: 36px; padding: 20px; margin-bottom: 24px; border: 1px solid #ffb347cc; }
    .quick-search-title { font-size: 1.2rem; font-weight: 700; margin-bottom: 16px; border-right: 4px solid #ffb347; padding-right: 16px; }
    .quick-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(260px, 1fr)); gap: 16px; }
    .quick-match-card { background: #0f3e4a; border-radius: 28px; padding: 12px; transition: 0.1s; }
    .quick-match-teams { display: flex; justify-content: space-between; align-items: center; gap: 8px; font-weight: bold; font-size: 0.85rem; }

    .predict-trigger-btn { display: block; width: 100%; margin-top: 12px; padding: 12px 16px; background: linear-gradient(135deg, rgba(255, 180, 70, 0.15), rgba(255, 140, 26, 0.08)); border: 2px solid rgba(255, 180, 70, 0.4); border-radius: 60px; color: #FFE6B0; font-size: 0.9rem; font-weight: 700; cursor: pointer; transition: all 0.3s ease; text-align: center; letter-spacing: 0.5px; box-shadow: 0 0 20px rgba(255, 180, 70, 0.05); backdrop-filter: blur(4px); }
    .predict-trigger-btn:hover:not(.already-predicted):not(.live-blocked) { background: linear-gradient(135deg, rgba(255, 180, 70, 0.25), rgba(255, 140, 26, 0.15)); border-color: #ffb347; box-shadow: 0 0 30px rgba(255, 180, 70, 0.15); transform: scale(1.01); }
    .predict-trigger-btn:active { transform: scale(0.97); }
    .predict-trigger-btn .icon { font-size: 1.1rem; margin-left: 8px; }
    .predict-trigger-btn .arrow { font-size: 0.8rem; margin-right: 8px; opacity: 0.7; }
    .predict-trigger-btn.live-blocked { opacity: 0.5; cursor: not-allowed; border-color: rgba(255, 68, 68, 0.3); background: rgba(255, 68, 68, 0.05); }
    .predict-trigger-btn.live-blocked:hover { transform: none; box-shadow: none; }
    .predict-trigger-btn.already-predicted { 
      opacity: 0.8; 
      border-color: #4CAF50; 
      background: rgba(76, 175, 80, 0.15);
      cursor: default;
      color: #8bc34a;
    }
    .predict-trigger-btn.already-predicted:hover {
      transform: none;
      box-shadow: none;
    }
    .predict-trigger-btn .already-icon {
      color: #4CAF50;
      margin-left: 6px;
    }

    .modal-overlay { display: none; position: fixed; top: 0; left: 0; right: 0; bottom: 0; background: rgba(0, 0, 0, 0.7); backdrop-filter: blur(12px); z-index: 9999; justify-content: center; align-items: center; animation: modalFadeIn 0.3s ease; }
    .modal-overlay.active { display: flex; }
    @keyframes modalFadeIn { from { opacity: 0; transform: scale(0.9); } to { opacity: 1; transform: scale(1); } }
    .modal-content { background: linear-gradient(145deg, rgba(18, 38, 44, 0.95), rgba(10, 25, 30, 0.98)); backdrop-filter: blur(24px); border-radius: 40px; padding: 30px; max-width: 480px; width: 95%; max-height: 90vh; overflow-y: auto; border: 1px solid rgba(255, 180, 70, 0.3); box-shadow: 0 30px 80px rgba(0, 0, 0, 0.6), 0 0 40px rgba(255, 180, 70, 0.05); position: relative; }
    .modal-close { position: absolute; top: 16px; left: 16px; background: rgba(255, 255, 255, 0.05); border: none; color: #98bdc9; font-size: 1.5rem; cursor: pointer; width: 40px; height: 40px; border-radius: 50%; display: flex; align-items: center; justify-content: center; transition: 0.2s; }
    .modal-close:hover { background: rgba(255, 68, 68, 0.2); color: #ff6b6b; transform: rotate(90deg); }
    .modal-title { text-align: center; font-size: 1.2rem; font-weight: 700; color: #FFE6B0; margin-bottom: 20px; padding-top: 10px; }
    .modal-teams { display: flex; justify-content: center; align-items: center; gap: 12px; background: rgba(0, 0, 0, 0.3); padding: 14px; border-radius: 60px; margin-bottom: 16px; }
    .modal-teams .m-team { font-weight: 700; font-size: 1rem; display: flex; align-items: center; gap: 6px; }
    .modal-teams .m-team span:first-child { font-size: 1.4rem; }
    .modal-teams .m-vs { background: rgba(255, 180, 70, 0.2); padding: 2px 12px; border-radius: 20px; font-size: 0.7rem; color: #ffb347; font-weight: 600; }
    .modal-datetime { text-align: center; font-size: 0.8rem; color: #98bdc9; margin-bottom: 20px; background: rgba(0, 0, 0, 0.2); padding: 6px 12px; border-radius: 40px; display: inline-block; width: 100%; }
    .modal-predict-options { display: flex; flex-direction: column; gap: 10px; margin-bottom: 16px; }
    .modal-predict-options label { display: flex; align-items: center; gap: 12px; background: rgba(255, 255, 255, 0.03); padding: 12px 16px; border-radius: 60px; cursor: pointer; transition: 0.2s; border: 2px solid transparent; }
    .modal-predict-options label:hover { background: rgba(255, 255, 255, 0.06); border-color: rgba(255, 180, 70, 0.2); }
    .modal-predict-options input[type="radio"] { appearance: none; width: 20px; height: 20px; border: 2px solid #555; border-radius: 50%; position: relative; cursor: pointer; flex-shrink: 0; transition: 0.2s; }
    .modal-predict-options input[type="radio"]:checked { border-color: #ffb347; background: #ffb347; }
    .modal-predict-options input[type="radio"]:checked::after { content: '✓'; position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: #1a2f2f; font-size: 12px; font-weight: 800; }
    .modal-predict-options .option-label { font-weight: 600; font-size: 0.9rem; }
    .modal-predict-options .option-sub { font-size: 0.7rem; color: #98bdc9; }
    .modal-user-input { margin-bottom: 16px; }
    .modal-user-input input { width: 100%; padding: 12px 16px; border-radius: 60px; border: 2px solid rgba(255, 255, 255, 0.1); background: rgba(255, 255, 255, 0.05); color: #f0f9ff; font-size: 0.9rem; outline: none; transition: 0.2s; }
    .modal-user-input input:focus { border-color: #ffb347; background: rgba(255, 255, 255, 0.08); box-shadow: 0 0 20px rgba(255, 180, 70, 0.05); }
    .modal-user-input input::placeholder { color: #666; }
    .modal-submit-btn { width: 100%; padding: 14px; border: none; border-radius: 60px; background: linear-gradient(135deg, #ffb347, #ff8c1a); color: #1a2f2f; font-weight: 800; font-size: 1rem; cursor: pointer; transition: 0.3s; display: flex; align-items: center; justify-content: center; gap: 10px; }
    .modal-submit-btn:hover { transform: scale(1.02); box-shadow: 0 0 30px rgba(255, 180, 70, 0.3); }
    .modal-submit-btn:active { transform: scale(0.97); }
    .modal-submit-btn:disabled { opacity: 0.5; cursor: not-allowed; transform: none; }
    .modal-message { margin-top: 12px; text-align: center; font-size: 0.9rem; font-weight: 600; padding: 8px 12px; border-radius: 40px; }
    .modal-message.success { color: #8bc34a; background: rgba(139,195,74,0.1); }
    .modal-message.error { color: #ff5252; background: rgba(255,82,82,0.1); }
    .modal-message.warning { color: #ffb347; background: rgba(255,179,71,0.1); }

    .prediction-card { background: rgba(18, 38, 44, 0.75); backdrop-filter: blur(12px); border-radius: 32px; padding: 16px; border: 1px solid rgba(255, 180, 70, 0.3); transition: 0.2s; }
    .prediction-card:hover { transform: translateY(-2px); border-color: #ffb347aa; }
    .prediction-card .user-name { display: flex; align-items: center; gap: 8px; margin-bottom: 10px; padding-bottom: 8px; border-bottom: 1px solid rgba(255, 180, 70, 0.2); font-size: 0.95rem; }
    .prediction-card .user-name .avatar { background: linear-gradient(135deg, #ffb347, #ff8c1a); width: 32px; height: 32px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 800; color: #1a2f2f; font-size: 0.9rem; }
    .prediction-card .pred-detail { display: flex; justify-content: space-between; align-items: center; margin-top: 4px; font-size: 0.85rem; }
    .prediction-card .match-info { font-size: 0.75rem; color: #98bdc9; margin-top: 6px; padding-top: 6px; border-top: 1px solid rgba(255,255,255,0.05); }
    .prediction-badge { background: linear-gradient(135deg, #ffb347, #ff8c1a); padding: 6px 20px; border-radius: 40px; font-weight: 800; color: #1a2f2f; display: inline-block; font-size: 0.85rem; box-shadow: 0 0 15px rgba(255, 180, 70, 0.2); border: 1px solid rgba(255, 200, 100, 0.3); letter-spacing: 0.5px; }
    .prediction-badge.home { background: linear-gradient(135deg, #4CAF50, #45a049); border-color: rgba(76, 175, 80, 0.5); color: white; }
    .prediction-badge.away { background: linear-gradient(135deg, #f44336, #d32f2f); border-color: rgba(244, 67, 54, 0.5); color: white; }
    .prediction-badge.draw { background: linear-gradient(135deg, #FF9800, #F57C00); border-color: rgba(255, 152, 0, 0.5); color: white; }

    .loading-spinner { display: inline-block; width: 20px; height: 20px; border: 3px solid rgba(255,255,255,0.3); border-radius: 50%; border-top-color: #ffb347; animation: spin 1s ease-in-out infinite; margin-left: 8px; }
    @keyframes spin { to { transform: rotate(360deg); } }

    footer { margin-top: 45px; text-align: center; font-size: 0.7rem; color: #98bdc9; border-top: 1px solid #ffb34760; padding-top: 20px; }

    @media (max-width: 550px) {
      body { padding: 12px; }
      .hero h1 { font-size: 1.3rem; }
      .tab-btn { padding: 6px 14px; font-size: 0.75rem; gap: 4px; }
      .team { font-size: 0.7rem; white-space: normal; }
      .team span:first-child { font-size: 1rem; }
      .countdown-timer { font-size: 0.75rem; }
      .matches-grid { gap: 14px; }
      .teams-score { flex-wrap: wrap; justify-content: center; }
      .team { min-width: 80px; }
      .prediction-card .pred-detail { flex-direction: column; gap: 8px; align-items: flex-start; }
      .leaderboard-item { flex-wrap: wrap; gap: 8px; }
      .leaderboard-item .player-name { margin: 0; width: 100%; }
      .news-ticker { font-size: 0.65rem; }
      .upper-bar { padding: 0 16px; height: 70px; min-height: 70px; }
      .upper-bar .title-section h1 { font-size: 1rem; }
      .upper-bar .bar-btn { padding: 4px 10px; font-size: 0.7rem; }
      .upper-bar .developer-credit { font-size: 0.6rem; }
      .leaderboard-section .section-title { font-size: 1.2rem; }
      .modal-content { padding: 20px; }
      .modal-teams { flex-wrap: wrap; }
      .main-header { height: 70px; min-height: 70px; }
    }
  </style>
</head>
<body>
<div class="app-container">
  
  <!-- ===== الهيدر العلوي الكامل مع خلفية الصورة ===== -->
  <div class="main-header"></div>
  
  <!-- ===== البار العلوي ===== -->
  <div class="upper-bar">
    <div class="bar-content">
      <div class="title-section">
        <h1>🏆 كأس العالم 2026</h1>
        <div class="developer-credit">⚡ غرفة معلمي سعيد بن العاص</div>
      </div>
      <div class="header-actions">
        <button class="bar-btn" onclick="location.reload()">
          <i class="fas fa-sync-alt"></i>
          <span style="display: none;">تحديث</span>
        </button>
      </div>
    </div>
  </div>
  
  <!-- ===== شريط الأخبار المتحرك ===== -->
  <div class="news-ticker-wrapper">
    <div class="news-ticker">
      <span>🗳️ طريقة التوقع: اختر المباراة → اختر (فوز الفريق الأول / فوز الفريق الثاني / تعادل) → اكتب اسمك → اضغط حفظ التوقع ✨</span>
      <span class="separator">|</span>
      <span>التوقعات تظهر للجميع مباشرة ويتم احتساب النقاط تلقائياً 🏆</span>
      <span class="separator">|</span>
      <span>⛔ لا يمكن التوقع على المباريات الجارية</span>
      <span class="separator">|</span>
      <span>🗳️ طريقة التوقع: اختر المباراة → اختر (فوز الفريق الأول / فوز الفريق الثاني / تعادل) → اكتب اسمك → اضغط حفظ التوقع ✨</span>
      <span class="separator">|</span>
      <span>التوقعات تظهر للجميع مباشرة ويتم احتساب النقاط تلقائياً 🏆</span>
    </div>
  </div>

  <!-- ===== ترتيب أصحاب التوقعات الصحيحة ===== -->
  <div class="leaderboard-section" id="leaderboardSection">
    <div class="section-title">
      <span class="trophy">🏆</span> ترتيب أصحاب التوقعات الصحيحة
    </div>
    <div id="leaderboardContainer" class="leaderboard-grid">
      <div class="empty-state">⏳ جاري تحميل الترتيب...</div>
    </div>
  </div>

  <div class="hero">
    <h1>🏆 كأس العالم 2026 ⚡</h1>
    <div class="school-badge">📢 غرفة معلمي سعيد بن العاص</div>
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
    <button class="tab-btn" data-tab="predictions"><i>🗳️</i> جميع التوقعات</button>
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

  <div id="predictionsTab" class="tab-content">
    <h3 style="margin: 0 0 16px 0; color: #FFE6B0;">🗳️ جميع توقعات اللاعبين</h3>
    <div id="allPredictions" class="matches-grid"><div class="empty-state">📭 جاري تحميل التوقعات...</div></div>
  </div>

  <footer>🔄 التحديث التلقائي | التوقعات محفوظة في Supabase</footer>
</div>

<!-- ===== نافذة التوقع المنبثقة ===== -->
<div class="modal-overlay" id="predictionModal">
  <div class="modal-content">
    <button class="modal-close" id="modalCloseBtn">✕</button>
    <div class="modal-title">📝 توقع نتيجة المباراة</div>
    
    <div class="modal-teams" id="modalTeams">
      <div class="m-team"><span>🏁</span> <span id="modalTeam1">الفريق الأول</span></div>
      <div class="m-vs">🆚</div>
      <div class="m-team"><span>🏁</span> <span id="modalTeam2">الفريق الثاني</span></div>
    </div>
    
    <div class="modal-datetime" id="modalDateTime">📅 التاريخ والوقت</div>
    
    <div class="modal-predict-options" id="modalOptions">
      <label>
        <input type="radio" name="prediction" value="HOME">
        <span class="option-label">🏆 <span id="optTeam1">الفريق الأول</span></span>
        <span class="option-sub">فوز</span>
      </label>
      <label>
        <input type="radio" name="prediction" value="AWAY">
        <span class="option-label">🏆 <span id="optTeam2">الفريق الثاني</span></span>
        <span class="option-sub">فوز</span>
      </label>
      <label>
        <input type="radio" name="prediction" value="DRAW">
        <span class="option-label">🤝 تعادل</span>
        <span class="option-sub">النتيجة متساوية</span>
      </label>
    </div>
    
    <div class="modal-user-input">
      <input type="text" id="modalUserName" placeholder="👤 أدخل اسمك" maxlength="30">
    </div>
    
    <button class="modal-submit-btn" id="modalSubmitBtn">
      💾 حفظ التوقع
    </button>
    
    <div class="modal-message" id="modalMessage"></div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
<script>
  // ... باقي الكود كما هو (للاختصار تم حذفه لكنه موجود في الملف الأصلي)
  console.log("✅ تم تطبيق الهيدر بارتفاع 80px وتغطية النص العلوي");
</script>
</body>
</html>
