<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>แบบทดสอบปฐมนิเทศน์พนักงาน</title>
<script src="https://cdn.jsdelivr.net/npm/qrcode/build/qrcode.min.js"></script>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;500;600;700&display=swap');

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --green: #0ea472;
    --green-light: #d1fae5;
    --green-dark: #065f46;
    --red-light: #fee2e2;
    --red-dark: #7f1d1d;
    --amber: #f59e0b;
    --bg: #f8f7f4;
    --card: #ffffff;
    --text: #1a1a1a;
    --muted: #6b7280;
    --border: #e5e7eb;
    --radius: 14px;
    --shadow: 0 2px 16px rgba(0,0,0,0.07);
  }

  html { font-size: 16px; }

  body {
    font-family: 'Sarabun', sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 24px 16px 60px;
  }

  /* ─── header strip ─── */
  .top-bar {
    width: 100%;
    max-width: 640px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 28px;
  }
  .brand {
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .brand-dot {
    width: 32px; height: 32px; border-radius: 10px;
    background: var(--green);
    display: flex; align-items: center; justify-content: center;
  }
  .brand-dot svg { width: 18px; height: 18px; fill: none; stroke: #fff; stroke-width: 2.2; stroke-linecap: round; }
  .brand-name { font-size: 15px; font-weight: 600; letter-spacing: -0.3px; }
  .brand-sub { font-size: 12px; color: var(--muted); }

  .qr-btn-top {
    display: flex; align-items: center; gap: 7px;
    background: linear-gradient(135deg, #7c3aed, #2563eb);
    border: none; border-radius: 10px; padding: 9px 16px;
    font-family: 'Sarabun', sans-serif; font-size: 13px; font-weight: 600;
    color: #fff; cursor: pointer;
    transition: opacity 0.15s, transform 0.1s;
    box-shadow: 0 3px 12px rgba(124,58,237,0.3);
  }
  .qr-btn-top:hover { opacity: 0.88; }
  .qr-btn-top:active { transform: scale(0.97); }
  .qr-btn-top svg { width: 16px; height: 16px; }

  /* ─── card ─── */
  .card {
    width: 100%; max-width: 640px;
    background: var(--card);
    border-radius: var(--radius);
    border: 1px solid var(--border);
    box-shadow: var(--shadow);
    overflow: hidden;
  }

  /* ─── progress ─── */
  .progress-track {
    height: 4px; background: #f0f0f0; width: 100%;
  }
  .progress-fill {
    height: 4px; background: var(--green);
    transition: width 0.5s cubic-bezier(.4,0,.2,1);
  }

  .card-body { padding: 28px 32px 32px; }

  .meta-row {
    display: flex; align-items: center; justify-content: space-between;
    margin-bottom: 20px;
  }
  .q-badge {
    font-size: 12px; font-weight: 600; letter-spacing: 0.5px;
    color: var(--green); text-transform: uppercase;
  }
  .score-badge {
    font-size: 13px; font-weight: 500; color: var(--muted);
  }
  .score-badge span { font-weight: 700; color: var(--text); }

  .q-text {
    font-size: 18px; font-weight: 600; line-height: 1.6;
    margin-bottom: 24px; color: var(--text);
  }

  /* ─── options ─── */
  .options { display: flex; flex-direction: column; gap: 10px; }

  .opt {
    display: flex; align-items: flex-start; gap: 14px;
    border: 1.5px solid var(--border);
    border-radius: 12px; padding: 14px 18px;
    cursor: pointer; background: var(--card);
    transition: border-color 0.15s, background 0.15s, transform 0.1s;
    text-align: left; font-family: 'Sarabun', sans-serif;
    font-size: 15px; color: var(--text); width: 100%;
  }
  .opt:hover:not(:disabled) {
    border-color: var(--green);
    background: #f0fdf9;
    transform: translateY(-1px);
  }
  .opt:disabled { cursor: default; }
  .opt.correct { background: var(--green-light); border-color: var(--green); color: var(--green-dark); }
  .opt.wrong { background: var(--red-light); border-color: #ef4444; color: var(--red-dark); }

  .opt-key {
    width: 26px; height: 26px; border-radius: 7px;
    background: #f3f4f6; display: flex; align-items: center; justify-content: center;
    font-size: 12px; font-weight: 700; flex-shrink: 0; margin-top: 1px;
    transition: background 0.15s, color 0.15s;
    color: var(--muted);
  }
  .opt.correct .opt-key { background: var(--green); color: #fff; }
  .opt.wrong .opt-key { background: #ef4444; color: #fff; }

  /* ─── feedback ─── */
  .feedback {
    display: none; margin-top: 16px;
    border-radius: 10px; padding: 12px 16px;
    font-size: 14px; line-height: 1.6;
    border-left: 4px solid transparent;
  }
  .feedback.show { display: flex; align-items: flex-start; gap: 10px; }
  .feedback.correct { background: var(--green-light); border-color: var(--green); color: var(--green-dark); }
  .feedback.wrong { background: var(--red-light); border-color: #ef4444; color: var(--red-dark); }
  .feedback-icon { flex-shrink: 0; font-size: 18px; line-height: 1.4; }

  /* ─── next button ─── */
  .next-wrap { margin-top: 24px; display: flex; justify-content: flex-end; }
  .next-btn {
    display: none; align-items: center; gap: 8px;
    background: var(--green); color: #fff;
    border: none; border-radius: 10px;
    padding: 12px 24px; font-family: 'Sarabun', sans-serif;
    font-size: 15px; font-weight: 600; cursor: pointer;
    transition: background 0.15s, transform 0.1s;
  }
  .next-btn.show { display: flex; }
  .next-btn:hover { background: #0a8a5e; }
  .next-btn:active { transform: scale(0.97); }
  .next-btn svg { width: 16px; height: 16px; }

  /* ─── result screen ─── */
  .result { display: none; }
  .result.show { display: block; }

  .result-hero {
    text-align: center; padding: 40px 32px 32px;
  }
  .donut-wrap {
    position: relative; width: 140px; height: 140px;
    margin: 0 auto 24px;
  }
  .donut-wrap svg { transform: rotate(-90deg); }
  .donut-label {
    position: absolute; top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
  .donut-score { font-size: 32px; font-weight: 700; color: var(--text); }
  .donut-total { font-size: 14px; color: var(--muted); }

  .result-grade {
    font-size: 22px; font-weight: 700; margin-bottom: 6px;
  }
  .result-msg { font-size: 15px; color: var(--muted); margin-bottom: 32px; }

  .grade-A { color: var(--green); }
  .grade-B { color: #0284c7; }
  .grade-C { color: var(--amber); }
  .grade-D { color: #ef4444; }

  /* ─── stats row ─── */
  .stats-row {
    display: grid; grid-template-columns: 1fr 1fr 1fr;
    gap: 12px; padding: 0 32px 28px;
  }
  .stat-card {
    background: #f8f7f4; border-radius: 12px;
    padding: 14px; text-align: center;
  }
  .stat-val { font-size: 22px; font-weight: 700; }
  .stat-lbl { font-size: 12px; color: var(--muted); margin-top: 2px; }
  .stat-correct .stat-val { color: var(--green); }
  .stat-wrong .stat-val { color: #ef4444; }
  .stat-pct .stat-val { color: var(--text); }

  /* ─── QR section ─── */
  .qr-section {
    border-top: 1px solid var(--border);
    padding: 32px 32px 36px;
    display: flex; flex-direction: column; align-items: center;
    gap: 14px;
    background: linear-gradient(160deg, #f0fdf9 0%, #eff6ff 50%, #fdf4ff 100%);
  }
  .qr-title {
    font-size: 16px; font-weight: 700; color: var(--text);
    display: flex; align-items: center; gap: 8px;
  }
  .qr-title-badge {
    font-size: 18px;
  }
  .qr-sub { font-size: 13px; color: var(--muted); text-align: center; max-width: 280px; line-height: 1.6; }
  .qr-frame {
    position: relative; padding: 5px; border-radius: 20px;
    background: linear-gradient(135deg, #06b6d4, #8b5cf6, #ec4899, #f59e0b);
    box-shadow: 0 8px 32px rgba(139,92,246,0.25);
  }
  .qr-inner {
    background: #fff; border-radius: 16px; padding: 14px;
    display: flex; flex-direction: column; align-items: center; gap: 8px;
  }
  #qr-canvas { border-radius: 8px; display: block; }
  .qr-label-strip {
    width: 100%; text-align: center;
    font-size: 11px; font-weight: 700; letter-spacing: 1.5px;
    color: #8b5cf6; text-transform: uppercase;
  }
  .qr-corners {
    position: absolute; inset: -1px; border-radius: 21px; pointer-events: none;
  }
  .qr-url {
    font-size: 11px; color: var(--muted);
    word-break: break-all; text-align: center;
    max-width: 300px; background: rgba(255,255,255,0.7);
    border-radius: 8px; padding: 6px 12px;
    border: 1px solid rgba(139,92,246,0.15);
  }
  .copy-btn {
    display: flex; align-items: center; gap: 7px;
    background: linear-gradient(135deg, #7c3aed, #2563eb);
    border: none; border-radius: 10px; padding: 10px 20px;
    font-family: 'Sarabun', sans-serif; font-size: 13px; font-weight: 600;
    color: #fff; cursor: pointer;
    transition: opacity 0.15s, transform 0.1s;
    box-shadow: 0 4px 14px rgba(124,58,237,0.3);
  }
  .copy-btn:hover { opacity: 0.88; }
  .copy-btn:active { transform: scale(0.97); }
  .copy-btn svg { width: 14px; height: 14px; }

  /* ─── result actions ─── */
  .result-actions {
    display: flex; gap: 10px; padding: 0 32px 32px; flex-wrap: wrap;
  }
  .btn-retry {
    flex: 1; display: flex; align-items: center; justify-content: center; gap: 8px;
    background: var(--green); color: #fff;
    border: none; border-radius: 10px; padding: 13px 20px;
    font-family: 'Sarabun', sans-serif; font-size: 15px; font-weight: 600;
    cursor: pointer; transition: background 0.15s;
    min-width: 160px;
  }
  .btn-retry:hover { background: #0a8a5e; }
  .btn-qr {
    display: flex; align-items: center; justify-content: center; gap: 8px;
    background: linear-gradient(135deg, #06b6d4, #8b5cf6);
    color: #fff;
    border: none; border-radius: 10px; padding: 13px 20px;
    font-family: 'Sarabun', sans-serif; font-size: 15px; font-weight: 600;
    cursor: pointer; transition: opacity 0.15s;
    box-shadow: 0 4px 14px rgba(139,92,246,0.3);
  }
  .btn-qr:hover { opacity: 0.88; }

  /* ─── QR modal ─── */
  .modal-backdrop {
    display: none; position: fixed; inset: 0;
    background: rgba(0,0,0,0.55); z-index: 100;
    align-items: center; justify-content: center;
    padding: 20px; backdrop-filter: blur(4px);
  }
  .modal-backdrop.open { display: flex; }
  .modal {
    background: #fff; border-radius: 24px;
    padding: 36px 28px 28px; max-width: 340px; width: 100%;
    text-align: center; position: relative;
    box-shadow: 0 24px 80px rgba(0,0,0,0.25);
  }
  .modal-close {
    position: absolute; top: 14px; right: 14px;
    background: #f3f4f6; border: none; border-radius: 8px;
    width: 32px; height: 32px; cursor: pointer; font-size: 18px;
    display: flex; align-items: center; justify-content: center;
    color: var(--muted);
  }
  .modal-close:hover { background: #e5e7eb; }
  .modal-emoji { font-size: 36px; margin-bottom: 10px; }
  .modal h3 { font-size: 18px; font-weight: 700; margin-bottom: 4px; color: var(--text); }
  .modal p { font-size: 13px; color: var(--muted); margin-bottom: 20px; }
  .modal-qr-frame {
    position: relative; padding: 4px; border-radius: 20px;
    background: linear-gradient(135deg, #06b6d4, #8b5cf6, #ec4899, #f59e0b);
    box-shadow: 0 8px 40px rgba(139,92,246,0.3);
    display: inline-block; margin-bottom: 16px;
  }
  .modal-qr-inner {
    background: #fff; border-radius: 17px; padding: 12px;
    display: flex; flex-direction: column; align-items: center; gap: 6px;
  }
  #qr-modal-canvas { border-radius: 8px; display: block; }
  .modal-qr-strip {
    font-size: 10px; font-weight: 700; letter-spacing: 1.5px;
    color: #8b5cf6; text-transform: uppercase;
  }
  .modal-url {
    font-size: 11px; color: var(--muted);
    word-break: break-all; margin-bottom: 16px;
    background: #f8f7f4; border-radius: 8px; padding: 8px 10px;
    border: 1px solid rgba(139,92,246,0.12);
  }
  .modal-copy {
    width: 100%; display: flex; align-items: center; justify-content: center; gap: 8px;
    background: linear-gradient(135deg, #7c3aed, #2563eb);
    color: #fff; border: none; border-radius: 12px;
    padding: 13px; font-family: 'Sarabun', sans-serif; font-size: 15px; font-weight: 600;
    cursor: pointer; transition: opacity 0.15s;
    box-shadow: 0 4px 16px rgba(124,58,237,0.3);
  }
  .modal-copy:hover { opacity: 0.88; }

  /* ─── intro screen ─── */
  .intro { display: block; }
  .intro-body { padding: 40px 32px; text-align: center; }
  .intro-icon {
    width: 64px; height: 64px; border-radius: 18px;
    background: linear-gradient(135deg, #0ea472, #059669);
    display: flex; align-items: center; justify-content: center;
    margin: 0 auto 20px;
  }
  .intro-icon svg { width: 32px; height: 32px; fill: none; stroke: #fff; stroke-width: 2; stroke-linecap: round; }
  .intro h2 { font-size: 22px; font-weight: 700; margin-bottom: 8px; }
  .intro-meta { font-size: 14px; color: var(--muted); margin-bottom: 28px; }
  .intro-chips {
    display: flex; flex-wrap: wrap; gap: 8px;
    justify-content: center; margin-bottom: 32px;
  }
  .chip {
    background: #f3f4f6; border-radius: 99px;
    padding: 5px 14px; font-size: 13px; color: var(--muted);
  }
  .start-btn {
    background: var(--green); color: #fff; border: none;
    border-radius: 12px; padding: 14px 36px;
    font-family: 'Sarabun', sans-serif; font-size: 16px; font-weight: 700;
    cursor: pointer; transition: background 0.15s, transform 0.1s;
    display: inline-flex; align-items: center; gap: 10px;
  }
  .start-btn:hover { background: #0a8a5e; }
  .start-btn:active { transform: scale(0.97); }

  @media (max-width: 520px) {
    .card-body, .result-hero { padding: 22px 20px 20px; }
    .stats-row { padding: 0 20px 20px; }
    .result-actions { padding: 0 20px 24px; }
    .qr-section { padding: 22px 20px; }
    .q-text { font-size: 16px; }
  }
</style>
</head>
<body>

<!-- top bar -->
<div class="top-bar">
  <div class="brand">
    <div class="brand-dot">
      <svg viewBox="0 0 24 24"><path d="M9 12l2 2 4-4M20 12a8 8 0 11-16 0 8 8 0 0116 0z"/></svg>
    </div>
    <div>
      <div class="brand-name">แบบทดสอบปฐมนิเทศน์พนักงาน</div>
      <div class="brand-sub">Employee Orientation Quiz</div>
    </div>
  </div>
  <button class="qr-btn-top" onclick="openQRModal()">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round">
      <rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/>
      <rect x="3" y="14" width="7" height="7"/>
      <path d="M14 14h.01M18 14h.01M14 18h.01M18 18h.01M14 21h4M21 14v4"/>
    </svg>
    แชร์ QR Code
  </button>
</div>

<!-- main card -->
<div class="card" id="app">

  <!-- intro -->
  <div class="intro" id="intro-screen">
    <div class="intro-body">
      <div class="intro-icon">
        <svg viewBox="0 0 24 24"><path d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-6 9l2 2 4-4"/></svg>
      </div>
      <h2>แบบทดสอบปฐมนิเทศน์พนักงาน</h2>
      <p class="intro-meta">20 ข้อ · เลือกคำตอบที่ถูกต้องที่สุด 1 ข้อ · มีเฉลยและคำอธิบาย</p>
      <div class="intro-chips">
        <span class="chip">นโยบายบริษัท</span>
        <span class="chip">กฎระเบียบ</span>
        <span class="chip">สวัสดิการ</span>
        <span class="chip">กองทุนสำรองเลี้ยงชีพ</span>
        <span class="chip">ประกันอุบัติเหตุ</span>
        <span class="chip">จรรยาบรรณ</span>
      </div>
      <button class="start-btn" onclick="startQuiz()">
        เริ่มทำแบบทดสอบ
        <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.5" stroke-linecap="round" width="18" height="18"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
      </button>
    </div>
  </div>

  <!-- quiz -->
  <div id="quiz-screen" style="display:none;">
    <div class="progress-track">
      <div class="progress-fill" id="prog" style="width:0%"></div>
    </div>
    <div class="card-body">
      <div class="meta-row">
        <div class="q-badge" id="q-badge">ข้อที่ 1</div>
        <div class="score-badge">คะแนน: <span id="live-score">0</span></div>
      </div>
      <div class="q-text" id="q-text"></div>
      <div class="options" id="options"></div>
      <div class="feedback" id="feedback">
        <span class="feedback-icon" id="fb-icon"></span>
        <span id="fb-text"></span>
      </div>
      <div class="next-wrap">
        <button class="next-btn" id="next-btn" onclick="nextQuestion()">
          ถัดไป
          <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.5" stroke-linecap="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
        </button>
      </div>
    </div>
  </div>

  <!-- result -->
  <div id="result-screen" style="display:none;">
    <div class="result-hero">
      <div class="donut-wrap">
        <svg width="140" height="140" viewBox="0 0 140 140">
          <circle cx="70" cy="70" r="58" fill="none" stroke="#f0f0f0" stroke-width="12"/>
          <circle cx="70" cy="70" r="58" fill="none" stroke-width="12"
            stroke-linecap="round" id="donut-arc"
            stroke-dasharray="364.4" stroke-dashoffset="364.4"/>
        </svg>
        <div class="donut-label">
          <div class="donut-score" id="res-score">0</div>
          <div class="donut-total">/ 20</div>
        </div>
      </div>
      <div class="result-grade" id="res-grade"></div>
      <div class="result-msg" id="res-msg"></div>
    </div>

    <div class="stats-row">
      <div class="stat-card stat-correct">
        <div class="stat-val" id="stat-correct">0</div>
        <div class="stat-lbl">ตอบถูก</div>
      </div>
      <div class="stat-card stat-wrong">
        <div class="stat-val" id="stat-wrong">0</div>
        <div class="stat-lbl">ตอบผิด</div>
      </div>
      <div class="stat-card stat-pct">
        <div class="stat-val" id="stat-pct">0%</div>
        <div class="stat-lbl">คะแนน</div>
      </div>
    </div>

    <div class="result-actions">
      <button class="btn-retry" onclick="startQuiz()">
        <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.2" stroke-linecap="round" width="18" height="18"><path d="M1 4v6h6M23 20v-6h-6"/><path d="M20.49 9A9 9 0 005.64 5.64L1 10M23 14l-4.64 4.36A9 9 0 013.51 15"/></svg>
        เริ่มใหม่อีกครั้ง
      </button>
      <button class="btn-qr" onclick="openQRModal()">
        <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2" stroke-linecap="round" width="18" height="18">
          <rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/>
          <rect x="3" y="14" width="7" height="7"/>
          <path d="M14 14h.01M18 14h.01M14 18h.01M18 18h.01"/>
        </svg>
        แชร์ QR
      </button>
    </div>

    <div class="qr-section">
      <div class="qr-title"><span class="qr-title-badge">📲</span> แชร์แบบทดสอบให้เพื่อนร่วมงาน</div>
      <div class="qr-sub">สแกน QR Code เพื่อเปิดแบบทดสอบปฐมนิเทศน์บนอุปกรณ์อื่น</div>
      <div class="qr-frame">
        <div class="qr-inner">
          <canvas id="qr-canvas" width="180" height="180"></canvas>
          <div class="qr-label-strip">✦ SCAN ME ✦</div>
        </div>
      </div>
      <div class="qr-url" id="qr-url-text"></div>
      <button class="copy-btn" onclick="copyLink()">
        <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2" stroke-linecap="round"><rect x="9" y="9" width="13" height="13" rx="2"/><path d="M5 15H4a2 2 0 01-2-2V4a2 2 0 012-2h9a2 2 0 012 2v1"/></svg>
        <span id="copy-txt">คัดลอกลิงก์</span>
      </button>
    </div>
  </div>
</div>

<!-- QR modal (available anytime) -->
<div class="modal-backdrop" id="qr-modal" onclick="closeQRModal(event)">
  <div class="modal">
    <button class="modal-close" onclick="closeQRModal(null, true)">✕</button>
    <div class="modal-emoji">🎯</div>
    <h3>แชร์แบบทดสอบปฐมนิเทศน์</h3>
    <p>ให้เพื่อนร่วมงานสแกน QR Code เพื่อทำแบบทดสอบ</p>
    <div class="modal-qr-frame">
      <div class="modal-qr-inner">
        <canvas id="qr-modal-canvas" width="200" height="200"></canvas>
        <div class="modal-qr-strip">✦ SCAN ME ✦</div>
      </div>
    </div>
    <div class="modal-url" id="modal-url-text"></div>
    <button class="modal-copy" onclick="copyLink(true)">
      <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2" stroke-linecap="round" width="16" height="16"><rect x="9" y="9" width="13" height="13" rx="2"/><path d="M5 15H4a2 2 0 01-2-2V4a2 2 0 012-2h9a2 2 0 012 2v1"/></svg>
      <span id="modal-copy-txt">คัดลอกลิงก์</span>
    </button>
  </div>
</div>

<script>
const QUESTIONS = [
  { q:"วิสัยทัศน์ของบริษัทมุ่งสู่การเป็นบริษัทชั้นนำในธุรกิจใด?", opts:["ธุรกิจก่อสร้าง","ธุรกิจพลังงาน","ธุรกิจขนส่ง","ธุรกิจอาหาร"], ans:1, exp:"วิสัยทัศน์ระบุว่า \"มุ่งสู่การเป็นบริษัทคู่สัญญาผู้บริการชั้นนำในธุรกิจพลังงานของไทยและภูมิภาค\"" },
  { q:"นโยบายข้อใดส่งเสริมการใช้ Stop Work Authority (SWA)?", opts:["การจัดการความเสี่ยงแบบบูรณาการ","การพัฒนาศักยภาพบุคลากร","เสริมสร้างวัฒนธรรม QSHE","ขับเคลื่อนการพัฒนาอย่างต่อเนื่อง"], ans:2, exp:"นโยบายข้อ 4 'เสริมสร้างวัฒนธรรม QSHE' ระบุถึงการสนับสนุนการใช้สิทธิ Stop Work Authority" },
  { q:"ความเร็วสูงสุดของยานพาหนะภายในบริษัทคือเท่าไร?", opts:["10 กม./ชม.","15 กม./ชม.","20 กม./ชม.","30 กม./ชม."], ans:2, exp:"กฎข้อ 10 ยานพาหนะทุกชนิดต้องใช้ความเร็วไม่เกิน 20 กม./ชม." },
  { q:"หากพบสภาพที่ไม่ปลอดภัยต้องแจ้งใคร?", opts:["ผู้จัดการฝ่าย","เจ้าหน้าที่ความปลอดภัย","ฝ่ายทรัพยากรบุคคล","เพื่อนร่วมงาน"], ans:1, exp:"กฎข้อ 13 ระบุว่าหากพบสภาพที่ไม่ปลอดภัยให้แจ้งเจ้าหน้าที่ความปลอดภัยฯ" },
  { q:"การละทิ้งหน้าที่กี่วันติดต่อกันโดยไม่มีเหตุผลอันสมควรเป็นเหตุไล่ออก?", opts:["1 วัน","2 วัน","3 วัน","5 วัน"], ans:2, exp:"การละทิ้งหน้าที่ 3 วันติดต่อกันโดยไม่มีเหตุผลอันสมควร เป็นเหตุให้ไล่ออก" },
  { q:"เงินช่วยเหลือการสมรสของพนักงานคือเท่าไร?", opts:["1,000 บาท","1,500 บาท","2,000 บาท","3,000 บาท"], ans:2, exp:"สวัสดิการระบุเงินช่วยเหลือเพื่อการสมรสพนักงาน 2,000 บาท" },
  { q:"บริษัทสมทบกองทุนสำรองเลี้ยงชีพในอัตราเท่าใด?", opts:["1%","2%","3%","5%"], ans:1, exp:"บริษัทสมทบ 2% ส่วนพนักงานเลือกออมได้ 2-15%" },
  { q:"พนักงานอายุสมาชิกกองทุนครบ 4 ปีแต่ไม่ถึง 5 ปี ได้รับสิทธิเงินสมทบกี่เปอร์เซ็นต์?", opts:["50%","60%","75%","100%"], ans:2, exp:"ครบ 4 ปีแต่น้อยกว่า 5 ปี ได้รับสิทธิ 75% ของเงินสมทบจากบริษัท" },
  { q:"ค่าสินไหมทดแทนกรณีเสียชีวิตจากอุบัติเหตุทั่วไปสูงสุดเท่าไร?", opts:["250,000 บาท","350,000 บาท","450,000 บาท","500,000 บาท"], ans:3, exp:"กรณีเสียชีวิต สูญเสียอวัยวะ ทุพพลภาพถาวร ได้รับไม่เกิน 500,000 บาท" },
  { q:"ค่ารักษาพยาบาลต่อครั้งจากประกันอุบัติเหตุสูงสุดเท่าไร?", opts:["20,000 บาท","30,000 บาท","40,000 บาท","50,000 บาท"], ans:3, exp:"ค่ารักษาพยาบาลต่อครั้งได้รับค่าสินไหมไม่เกิน 50,000 บาท" },
  { q:"กรณีใดที่พนักงานได้รับสิทธิเงินสมทบกองทุน 100% เต็ม?", opts:["ลาออกจากงาน","ครบ 5 ปีและลาออก","เสียชีวิต ทุพพลภาพ หรือเกษียณ","ครบ 3 ปีในกองทุน"], ans:2, exp:"ได้รับ 100% ในกรณีเสียชีวิต เกษียณ หรือทุพพลภาพ" },
  { q:"พนักงานระดับ 1-9 ได้รับค่าเบี้ยเลี้ยงเดินทางนอกสถานที่สูงสุดวันละเท่าไร?", opts:["150 บาท","200 บาท","250 บาท","300 บาท"], ans:1, exp:"พนักงานระดับ 1-9 ค่าเบี้ยเลี้ยงตามที่จ่ายจริง ไม่เกิน 200 บาท/วัน" },
  { q:"พนักงานระดับ 10 ขึ้นไป ค่าที่พักนอกสถานที่สูงสุดวันละเท่าไร?", opts:["800 บาท","1,000 บาท","1,200 บาท","1,500 บาท"], ans:1, exp:"พนักงานระดับ 10 ขึ้นไป ค่าที่พักตามที่จ่ายจริง ไม่เกิน 1,000 บาท/วัน" },
  { q:"จรรยาบรรณธุรกิจของบริษัทมีทั้งหมดกี่หมวด?", opts:["8 หมวด","9 หมวด","10 หมวด","11 หมวด"], ans:3, exp:"จรรยาบรรณธุรกิจกำหนดไว้ 11 หมวด" },
  { q:"พฤติกรรมใดเป็นเหตุของการลงโทษไล่ออก?", opts:["มาสายบ่อยครั้ง","รายงานเท็จต่อผู้บังคับบัญชา","แต่งกายไม่เหมาะสม","ผลงานต่ำกว่ามาตรฐาน"], ans:1, exp:"รายงานเท็จต่อผู้บังคับบัญชาเป็นเหตุให้ไล่ออกตามระเบียบบริษัท" },
  { q:"ของเยี่ยมไข้พนักงานมีมูลค่าเท่าไร?", opts:["500 บาท","800 บาท","1,000 บาท","1,500 บาท"], ans:2, exp:"สวัสดิการระบุของเยี่ยมไข้พนักงาน 1,000 บาท" },
  { q:"เงินช่วยเหลืออุปสมบทพนักงานคือเท่าไร?", opts:["500 บาท","1,000 บาท","2,000 บาท","3,000 บาท"], ans:1, exp:"เงินช่วยเหลือเพื่อการอุปสมบทพนักงาน 1,000 บาท" },
  { q:"ประกันอุบัติเหตุกลุ่มของบริษัทอยู่ในเครืออะไร?", opts:["เมืองไทยประกันภัย","กรุงเทพประกันภัย","อาคเนย์ประกันภัย","ไทยประกันภัย"], ans:1, exp:"บริษัทจัดทำประกันภัยกลุ่ม กรุ๊ป พีเอ เฟิสต์ ในเครือกรุงเทพประกันภัย" },
  { q:"นโยบายใดเกี่ยวข้องกับการรับมือกับความเปลี่ยนแปลงและรักษาความต่อเนื่องทางธุรกิจ?", opts:["การส่งมอบความเป็นเลิศ","การจัดการความเสี่ยงแบบบูรณาการ","ความยืดหยุ่นขององค์กรและความต่อเนื่องทางธุรกิจ","ขับเคลื่อนการพัฒนาอย่างต่อเนื่อง"], ans:2, exp:"นโยบายข้อ 6 'ความยืดหยุ่นขององค์กรและความต่อเนื่องทางธุรกิจ' ครอบคลุมเรื่องนี้" },
  { q:"พนักงานสามารถสมัครกองทุนสำรองเลี้ยงชีพได้เมื่อใด?", opts:["ทำงานครบ 6 เดือน","ผ่านทดลองงาน","ทำงานครบ 1 ปี","ทำงานครบ 2 ปี"], ans:1, exp:"พนักงานที่ผ่านทดลองงานแล้วสามารถสมัครกองทุนได้ทันที" }
];

const KEYS = ['ก','ข','ค','ง'];
let deck = [], cur = 0, score = 0, answered = false;

function shuffle(a) { return a.slice().sort(() => Math.random() - 0.5); }

function startQuiz() {
  deck = shuffle(QUESTIONS);
  cur = 0; score = 0; answered = false;
  document.getElementById('intro-screen').style.display = 'none';
  document.getElementById('result-screen').style.display = 'none';
  document.getElementById('quiz-screen').style.display = 'block';
  document.getElementById('live-score').textContent = '0';
  renderQ();
}

function renderQ() {
  answered = false;
  const q = deck[cur];
  const total = deck.length;
  document.getElementById('prog').style.width = ((cur / total) * 100) + '%';
  document.getElementById('q-badge').textContent = 'ข้อที่ ' + (cur + 1) + ' / ' + total;
  document.getElementById('q-text').textContent = q.q;

  const opts = document.getElementById('options');
  opts.innerHTML = '';
  q.opts.forEach((o, i) => {
    const btn = document.createElement('button');
    btn.className = 'opt';
    btn.innerHTML = '<span class="opt-key">' + KEYS[i] + '</span><span>' + o + '</span>';
    btn.onclick = () => pick(i);
    opts.appendChild(btn);
  });

  const fb = document.getElementById('feedback');
  fb.className = 'feedback';
  document.getElementById('next-btn').className = 'next-btn';
}

function pick(idx) {
  if (answered) return;
  answered = true;
  const q = deck[cur];
  const btns = document.querySelectorAll('.opt');
  btns.forEach((b, i) => {
    b.disabled = true;
    if (i === q.ans) b.classList.add('correct');
    else if (i === idx) b.classList.add('wrong');
  });

  const fb = document.getElementById('feedback');
  if (idx === q.ans) {
    score++;
    document.getElementById('live-score').textContent = score;
    fb.className = 'feedback correct show';
    document.getElementById('fb-icon').textContent = '✓';
    document.getElementById('fb-text').textContent = 'ถูกต้อง! ' + q.exp;
  } else {
    fb.className = 'feedback wrong show';
    document.getElementById('fb-icon').textContent = '✗';
    document.getElementById('fb-text').textContent = 'ไม่ถูกต้อง ' + q.exp;
  }
  document.getElementById('next-btn').className = 'next-btn show';
}

function nextQuestion() {
  cur++;
  if (cur >= deck.length) showResult();
  else renderQ();
}

function showResult() {
  document.getElementById('quiz-screen').style.display = 'none';
  document.getElementById('result-screen').style.display = 'block';
  document.getElementById('prog').style.width = '100%';

  const pct = Math.round((score / 20) * 100);
  document.getElementById('res-score').textContent = score;
  document.getElementById('stat-correct').textContent = score;
  document.getElementById('stat-wrong').textContent = 20 - score;
  document.getElementById('stat-pct').textContent = pct + '%';

  // donut animation
  const circ = 2 * Math.PI * 58;
  const arc = document.getElementById('donut-arc');
  const gradeInfo = pct >= 90
    ? { grade: 'ยอดเยี่ยม!', msg: 'คุณเข้าใจนโยบายบริษัทอย่างดีเยี่ยม', cls: 'grade-A', color: '#0ea472' }
    : pct >= 70
    ? { grade: 'ดีมาก', msg: 'คุณมีความรู้ในระดับที่ดี', cls: 'grade-B', color: '#0284c7' }
    : pct >= 50
    ? { grade: 'ผ่าน', msg: 'ควรทบทวนนโยบายบางส่วนเพิ่มเติม', cls: 'grade-C', color: '#f59e0b' }
    : { grade: 'ต้องพัฒนาเพิ่มเติม', msg: 'โปรดศึกษานโยบายบริษัทอีกครั้ง', cls: 'grade-D', color: '#ef4444' };

  arc.setAttribute('stroke', gradeInfo.color);
  setTimeout(() => {
    arc.style.transition = 'stroke-dashoffset 1s cubic-bezier(.4,0,.2,1)';
    arc.setAttribute('stroke-dashoffset', circ - (circ * pct / 100));
  }, 100);

  document.getElementById('res-grade').textContent = gradeInfo.grade;
  document.getElementById('res-grade').className = 'result-grade ' + gradeInfo.cls;
  document.getElementById('res-msg').textContent = gradeInfo.msg;

  generateQR('qr-canvas', 180);
  renderURLText();
}

function generateQR(canvasId, size) {
  const url = window.location.href.split('?')[0];
  if (typeof QRCode !== 'undefined') {
    QRCode.toCanvas(document.getElementById(canvasId), url, { width: size, margin: 2 }, () => {});
  }
}

function renderURLText() {
  const url = window.location.href.split('?')[0];
  const el = document.getElementById('qr-url-text');
  if (el) el.textContent = url;
  const mel = document.getElementById('modal-url-text');
  if (mel) mel.textContent = url;
}

function openQRModal() {
  document.getElementById('qr-modal').classList.add('open');
  generateQR('qr-modal-canvas', 200);
  renderURLText();
}

function closeQRModal(e, force) {
  if (force || e.target === document.getElementById('qr-modal'))
    document.getElementById('qr-modal').classList.remove('open');
}

function copyLink(isModal) {
  const url = window.location.href.split('?')[0];
  navigator.clipboard.writeText(url).then(() => {
    const id = isModal ? 'modal-copy-txt' : 'copy-txt';
    const el = document.getElementById(id);
    el.textContent = 'คัดลอกแล้ว!';
    setTimeout(() => { el.textContent = 'คัดลอกลิงก์'; }, 2000);
  });
}
</script>
</body>
</html>
