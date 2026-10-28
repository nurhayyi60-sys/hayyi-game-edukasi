<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<title>Tarik Tambang 2 Tim - Persamaan Linear</title>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
  body {
    background: linear-gradient(180deg, #87CEEB 0%, #98D8E8 60%, #7CB342 60%, #558B2F 100%);
    min-height: 100vh;
    padding: 15px;
  }
  .container { max-width: 1100px; margin: 0 auto; }
  h1 {
    text-align: center;
    color: #fff;
    text-shadow: 3px 3px 0 #d32f2f;
    font-size: 2.3em;
    margin-bottom: 5px;
  }
  .subtitle {
    text-align: center;
    color: #fff;
    margin-bottom: 15px;
    font-size: 1em;
  }

  /* Arena */
  .arena {
    position: relative;
    height: 260px;
    background: linear-gradient(180deg, transparent 0%, #8D6E63 70%, #5D4037 100%);
    border-radius: 20px;
    overflow: hidden;
    border: 4px solid #3E2723;
    margin-bottom: 15px;
  }
  .ground {
    position: absolute; bottom: 0; width: 100%; height: 30%;
    background: repeating-linear-gradient(45deg, #8D6E63, #8D6E63 20px, #795548 20px, #795548 40px);
  }
  .center-line {
    position: absolute; top: 0; left: 50%; width: 4px; height: 100%;
    background: repeating-linear-gradient(0deg, #fff 0, #fff 10px, transparent 10px, transparent 20px);
    z-index: 2;
  }
  .rope {
    position: absolute; top: 50%; left: 0; right: 0; height: 12px;
    background: repeating-linear-gradient(90deg, #D7CCC8 0, #D7CCC8 15px, #8D6E63 15px, #8D6E63 30px);
    transform: translateY(-50%);
    transition: transform 1s cubic-bezier(0.68, -0.55, 0.27, 1.55);
    z-index: 3;
  }
  .flag {
    position: absolute; top: 50%; left: 50%;
    width: 4px; height: 70px; background: #fff;
    transform: translate(-50%, -50%);
    transition: left 1s cubic-bezier(0.68, -0.55, 0.27, 1.55);
    z-index: 4;
  }
  .flag::after {
    content: ''; position: absolute; top: -5px; left: 4px;
    width: 30px; height: 22px; background: #FF5722;
    clip-path: polygon(0 0, 100% 0, 80% 50%, 100% 100%, 0 100%);
  }
  .team {
    position: absolute; top: 50%; transform: translateY(-50%);
    text-align: center; z-index: 5;
    transition: left 1s cubic-bezier(0.68, -0.55, 0.27, 1.55),
                right 1s cubic-bezier(0.68, -0.55, 0.27, 1.55);
  }
  .team-left { left: 5%; }
  .team-right { right: 5%; }
  .character { font-size: 3.5em; }
  .team.active .character { animation: pullHard 0.4s ease-in-out infinite alternate; }
  .team-right.active .character { animation: pullHardRight 0.4s ease-in-out infinite alternate; }
  @keyframes pullHard { from { transform: translateX(0) rotate(-5deg); } to { transform: translateX(-15px) rotate(5deg); } }
  @keyframes pullHardRight { from { transform: translateX(0) rotate(5deg); } to { transform: translateX(15px) rotate(-5deg); } }
  .team-label {
    background: rgba(0,0,0,0.7); color: #fff;
    padding: 5px 15px; border-radius: 20px;
    font-weight: bold; margin-top: 5px; display: inline-block;
  }
  .team-left .team-label { background: #1976D2; }
  .team-right .team-label { background: #D32F2F; }
  .team.active { filter: drop-shadow(0 0 15px gold); }

  /* Scoreboard */
  .scoreboard {
    display: flex; justify-content: space-around;
    background: rgba(255,255,255,0.95);
    padding: 12px; border-radius: 15px;
    margin-bottom: 15px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
  }
  .score-item { text-align: center; flex: 1; }
  .score-item h3 { color: #555; font-size: 0.85em; }
  .score-item .value { font-size: 1.8em; font-weight: bold; }
  .score-item.siswa .value { color: #1976D2; }
  .score-item.komputer .value { color: #D32F2F; }
  .score-item.turn .value { color: #F57C00; font-size: 1.1em; }

  /* Progress */
  .progress {
    display: flex; justify-content: center; gap: 6px;
    margin-bottom: 15px; flex-wrap: wrap;
  }
  .dot {
    width: 32px; height: 32px; border-radius: 50%;
    background: #ddd; display: flex; align-items: center; justify-content: center;
    font-size: 0.75em; font-weight: bold; color: #fff;
    transition: all 0.3s; border: 3px solid transparent;
  }
  .dot.kiri { background: #64B5F6; }
  .dot.kanan { background: #E57373; }
  .dot.correct { background: #4CAF50 !important; }
  .dot.wrong { background: #F44336 !important; }
  .dot.current { border-color: gold; transform: scale(1.25); box-shadow: 0 0 15px gold; }
  .dot span { font-size: 0.7em; }

  /* Question box */
  .question-box {
    background: #fff; padding: 20px;
    border-radius: 15px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    text-align: center;
    border: 4px solid transparent;
    transition: border-color 0.3s;
  }
  .question-box.turn-kiri { border-color: #1976D2; }
  .question-box.turn-kanan { border-color: #D32F2F; }
  .turn-indicator {
    font-size: 1.3em; font-weight: bold;
    padding: 8px; border-radius: 10px;
    margin-bottom: 10px; color: #fff;
  }
  .turn-indicator.kiri { background: #1976D2; }
  .turn-indicator.kanan { background: #D32F2F; }
  .question-number { color: #555; font-weight: bold; margin: 8px 0; font-size: 0.95em; }
  .question {
    font-size: 1.8em; color: #333; margin: 12px 0;
    font-family: 'Courier New', monospace;
    background: #FFF9C4; padding: 15px;
    border-radius: 10px; border: 3px dashed #FBC02D;
  }
  .answer-area {
    display: flex; justify-content: center; align-items: center;
    gap: 10px; margin: 15px 0; flex-wrap: wrap;
  }
  .answer-area label { font-size: 1.3em; font-weight: bold; }
  input[type="number"] {
    font-size: 1.5em; padding: 10px 15px; width: 120px;
    border: 3px solid #1976D2; border-radius: 10px;
    text-align: center; font-weight: bold;
  }
  button {
    background: #4CAF50; color: #fff; border: none;
    padding: 12px 30px; font-size: 1.2em;
    border-radius: 10px; cursor: pointer; font-weight: bold;
    transition: all 0.3s; box-shadow: 0 4px 0 #2E7D32;
  }
  button:hover { background: #45a049; transform: translateY(-2px); }
  button:active { transform: translateY(2px); box-shadow: 0 2px 0 #2E7D32; }
  button:disabled { background: #999; cursor: not-allowed; box-shadow: none; }

  .feedback {
    margin-top: 12px; padding: 12px;
    border-radius: 10px; font-size: 1.1em; font-weight: bold;
    min-height: 45px;
    display: flex; align-items: center; justify-content: center;
  }
  .feedback.correct { background: #C8E6C9; color: #2E7D32; }
  .feedback.wrong { background: #FFCDD2; color: #C62828; }
  .feedback.info { background: #E3F2FD; color: #1565C0; }

  /* Modal */
  .modal {
    display: none; position: fixed; top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(0,0,0,0.8); z-index: 100;
    justify-content: center; align-items: center;
  }
  .modal.show { display: flex; }
  .modal-content {
    background: #fff; padding: 35px;
    border-radius: 20px; text-align: center;
    max-width: 500px; animation: popIn 0.5s;
  }
  @keyframes popIn { from { transform: scale(0); } to { transform: scale(1); } }
  .modal-content h2 { font-size: 2.2em; margin-bottom: 15px; }
  .modal-content.win-kiri h2 { color: #1976D2; }
  .modal-content.win-kanan h2 { color: #D32F2F; }
  .modal-content.draw h2 { color: #F57C00; }
  .emoji { font-size: 4.5em; margin: 15px 0; }

  .rules {
    background: rgba(255,255,255,0.9);
    padding: 10px 15px; border-radius: 10px;
    margin-bottom: 15px; font-size: 0.9em;
    text-align: center; color: #333;
  }
  .rules b { color: #D32F2F; }
</style>
</head>
<body>
<div class="container">
  <h1>🏆 TARIK TAMBANG 2 TIM 🏆</h1>
  <p class="subtitle">Persamaan Linear | SMK Kelas 10</p>

  <div class="rules">
    🎯 <b>Aturan:</b> Soal muncul bergantian untuk Tim Kiri & Tim Kanan.
    Jawaban benar = tali bergerak ke arah timmu. Jawaban salah = tali bergerak ke arah lawan.
    Setelah 10 soal, tim yang menarik tali paling jauh ke arahnya menang!
  </div>

  <div class="arena">
    <div class="ground"></div>
    <div class="center-line"></div>
    <div class="rope" id="rope"></div>
    <div class="flag" id="flag"></div>
    <div class="team team-left" id="teamLeft">
      <div class="character">🧑‍🎓</div>
      <div class="team-label">TIM KIRI</div>
    </div>
    <div class="team team-right" id="teamRight">
      <div class="character">🤖</div>
      <div class="team-label">TIM KANAN</div>
    </div>
  </div>

  <div class="scoreboard">
    <div class="score-item siswa">
      <h3>🧑‍🎓 Skor Tim Kiri</h3>
      <div class="value" id="scoreKiri">0</div>
    </div>
    <div class="score-item turn">
      <h3>🎯 Giliran</h3>
      <div class="value" id="turnInfo">TIM KIRI</div>
    </div>
    <div class="score-item komputer">
      <h3>🤖 Skor Tim Kanan</h3>
      <div class="value" id="scoreKanan">0</div>
    </div>
  </div>

  <div class="progress" id="progress"></div>

  <div class="question-box" id="questionBox">
    <div class="turn-indicator kiri" id="turnIndicator">🎯 GILIRAN: TIM KIRI</div>
    <div class="question-number" id="qNumber">Soal 1 dari 10</div>
    <div class="question" id="question">2x + 3 = 11</div>
    <div class="answer-area">
      <label>x = </label>
      <input type="number" id="answer" placeholder="?">
      <button onclick="checkAnswer()" id="submitBtn">JAWAB</button>
    </div>
    <div class="feedback info" id="feedback">Masukkan jawabanmu dan tarik tali!</div>
  </div>
</div>

<div class="modal" id="modal">
  <div class="modal-content" id="modalContent">
    <div class="emoji" id="modalEmoji">🏆</div>
    <h2 id="modalTitle">SELAMAT!</h2>
    <p id="modalText" style="font-size:1.15em; margin:15px 0;"></p>
    <button onclick="restartGame()">🔄 MAIN LAGI</button>
  </div>
</div>

<script>
  // 5 pasang soal - topik sama per pasangan, angka berbeda
  // Setiap pasangan: { topic, kiri: {q, answer, hint}, kanan: {q, answer, hint} }
  const questionPairs = [
    {
      topic: "Bentuk ax + b = c",
      kiri:  { q: "2x + 3 = 11",      answer: 4,  hint: "Kurangi 3 dari kedua ruas, lalu bagi 2" },
      kanan: { q: "3x + 5 = 20",      answer: 5,  hint: "Kurangi 5 dari kedua ruas, lalu bagi 3" }
    },
    {
      topic: "Bentuk ax - b = c",
      kiri:  { q: "4x - 5 = 11",      answer: 4,  hint: "Tambah 5 ke kedua ruas, lalu bagi 4" },
      kanan: { q: "5x - 3 = 17",      answer: 4,  hint: "Tambah 3 ke kedua ruas, lalu bagi 5" }
    },
    {
      topic: "Bentuk a(x + b) = c",
      kiri:  { q: "2(x + 3) = 14",    answer: 4,  hint: "Bagi 2 dulu, lalu kurangi 3" },
      kanan: { q: "3(x + 2) = 18",    answer: 4,  hint: "Bagi 3 dulu, lalu kurangi 2" }
    },
    {
      topic: "Bentuk ax + b = cx + d",
      kiri:  { q: "5x + 2 = 3x + 10", answer: 4,  hint: "Kumpulkan x di kiri, angka di kanan" },
      kanan: { q: "6x - 1 = 4x + 7",  answer: 4,  hint: "Kumpulkan x di kiri, angka di kanan" }
    },
    {
      topic: "Bentuk x/a + b = c",
      kiri:  { q: "x/2 + 3 = 7",      answer: 8,  hint: "Kurangi 3, lalu kali 2" },
      kanan: { q: "x/3 + 2 = 6",      answer: 12, hint: "Kurangi 2, lalu kali 3" }
    }
  ];

  // Urutan giliran: Kiri soal 1, Kanan soal 1, Kiri soal 2, Kanan soal 2, ...
  let turns = [];
  for (let i = 0; i < questionPairs.length; i++) {
    turns.push({ pairIndex: i, team: 'kiri' });
    turns.push({ pairIndex: i, team: 'kanan' });
  }

  let currentTurn = 0;
  let scoreKiri = 0;
  let scoreKanan = 0;
  let ropePosition = 0; // negatif = ke kiri, positif = ke kanan

  function initProgress() {
    const p = document.getElementById('progress');
    p.innerHTML = '';
    turns.forEach((t, i) => {
      const d = document.createElement('div');
      d.className = 'dot ' + t.team + (i === 0 ? ' current' : '');
      d.id = 'dot-' + i;
      d.innerHTML = `<span>${i+1}<br>${t.team === 'kiri' ? '🧑' : '🤖'}</span>`;
      p.appendChild(d);
    });
  }

  function loadTurn() {
    if (currentTurn >= turns.length) {
      endGame();
      return;
    }
    const turn = turns[currentTurn];
    const pair = questionPairs[turn.pairIndex];
    const qData = pair[turn.team];

    // Update indikator giliran
    const turnIndicator = document.getElementById('turnIndicator');
    const questionBox = document.getElementById('questionBox');
    const turnInfo = document.getElementById('turnInfo');
    const teamLeft = document.getElementById('teamLeft');
    const teamRight = document.getElementById('teamRight');

    questionBox.classList.remove('turn-kiri', 'turn-kanan');
    turnIndicator.classList.remove('kiri', 'kanan');
    teamLeft.classList.remove('active');
    teamRight.classList.remove('active');

    if (turn.team === 'kiri') {
      turnIndicator.classList.add('kiri');
      turnIndicator.textContent = '🎯 GILIRAN: TIM KIRI (Siswa)';
      questionBox.classList.add('turn-kiri');
      turnInfo.textContent = 'TIM KIRI';
      teamLeft.classList.add('active');
    } else {
      turnIndicator.classList.add('kanan');
      turnIndicator.textContent = '🎯 GILIRAN: TIM KANAN (Komputer)';
      questionBox.classList.add('turn-kanan');
      turnInfo.textContent = 'TIM KANAN';
      teamRight.classList.add('active');
    }

    document.getElementById('qNumber').textContent = 
      `Soal ${currentTurn + 1} dari ${turns.length} • Topik: ${pair.topic}`;
    document.getElementById('question').textContent = qData.q;
    document.getElementById('answer').value = '';
    document.getElementById('answer').focus();
    document.getElementById('feedback').className = 'feedback info';
    document.getElementById('feedback').textContent = 
      turn.team === 'kiri' 
        ? 'Jawab benar → tali ke kiri. Salah → tali ke kanan.'
        : 'Jawab benar → tali ke kanan. Salah → tali ke kiri.';
    document.getElementById('submitBtn').disabled = false;

    document.querySelectorAll('.dot').forEach((d, i) => {
      if (i === currentTurn) d.classList.add('current');
      else d.classList.remove('current');
    });
  }

  function checkAnswer() {
    const input = document.getElementById('answer');
    const userAns = parseFloat(input.value);
    if (isNaN(userAns)) {
      document.getElementById('feedback').className = 'feedback wrong';
      document.getElementById('feedback').textContent = '⚠️ Masukkan angka terlebih dahulu!';
      return;
    }

    const turn = turns[currentTurn];
    const qData = questionPairs[turn.pairIndex][turn.team];
    const correct = userAns === qData.answer;
    const dot = document.getElementById('dot-' + currentTurn);
    dot.classList.remove('current');

    document.getElementById('submitBtn').disabled = true;

    let feedbackHTML = '';
    let ropeMoved = '';

    if (turn.team === 'kiri') {
      if (correct) {
        scoreKiri++;
        ropePosition--;
        dot.classList.add('correct');
        dot.innerHTML = '✓';
        feedbackHTML = `✅ BENAR! Tali bergerak ke TIM KIRI! <br><small>Jawaban: x = ${qData.answer}</small>`;
        ropeMoved = '← ke kiri';
      } else {
        scoreKanan++;
        ropePosition++;
        dot.classList.add('wrong');
        dot.innerHTML = '✗';
        feedbackHTML = `❌ SALAH! Tali bergerak ke TIM KANAN! <br><small>Jawaban benar: x = ${qData.answer}. ${qData.hint}</small>`;
        ropeMoved = '→ ke kanan';
      }
    } else { // kanan
      if (correct) {
        scoreKanan++;
        ropePosition++;
        dot.classList.add('correct');
        dot.innerHTML = '✓';
        feedbackHTML = `✅ BENAR! Tali bergerak ke TIM KANAN! <br><small>Jawaban: x = ${qData.answer}</small>`;
        ropeMoved = '→ ke kanan';
      } else {
        scoreKiri++;
        ropePosition--;
        dot.classList.add('wrong');
        dot.innerHTML = '✗';
        feedbackHTML = `❌ SALAH! Tali bergerak ke TIM KIRI! <br><small>Jawaban benar: x = ${qData.answer}. ${qData.hint}</small>`;
        ropeMoved = '← ke kiri';
      }
    }

    document.getElementById('feedback').className = correct ? 'feedback correct' : 'feedback wrong';
    document.getElementById('feedback').innerHTML = feedbackHTML + `<br><small>🪢 Tali bergeser ${ropeMoved}</small>`;

    document.getElementById('scoreKiri').textContent = scoreKiri;
    document.getElementById('scoreKanan').textContent = scoreKanan;
    updateRope();

    setTimeout(() => {
      currentTurn++;
      loadTurn();
    }, 2800);
  }

  function updateRope() {
    const offset = ropePosition * 5; // %
    document.getElementById('flag').style.left = `calc(50% + ${offset}%)`;
    document.getElementById('teamLeft').style.left = `calc(5% + ${offset * 0.4}%)`;
    document.getElementById('teamRight').style.right = `calc(5% - ${offset * 0.4}%)`;
  }

  function endGame() {
    const modal = document.getElementById('modal');
    const content = document.getElementById('modalContent');
    const emoji = document.getElementById('modalEmoji');
    const title = document.getElementById('modalTitle');
    const text = document.getElementById('modalText');

    if (scoreKiri > scoreKanan) {
      content.className = 'modal-content win-kiri';
      emoji.textContent = '🏆🧑‍🎓';
      title.textContent = 'TIM KIRI MENANG!';
      text.innerHTML = `Selamat! Tim Kiri berhasil mengalahkan Tim Kanan!<br><br>
        Skor Akhir: <b style="color:#1976D2">${scoreKiri}</b> - <b style="color:#D32F2F">${scoreKanan}</b><br>
        Posisi tali: ${ropePosition < 0 ? Math.abs(ropePosition) + ' langkah ke kiri' : ropePosition > 0 ? ropePosition + ' langkah ke kanan' : 'tengah'}<br><br>
        Kamu menguasai Persamaan Linear! 🎉`;
    } else if (scoreKiri < scoreKanan) {
      content.className = 'modal-content win-kanan';
      emoji.textContent = '🤖🏆';
      title.textContent = 'TIM KANAN MENANG!';
      text.innerHTML = `Yah, Tim Kanan berhasil menarik tali!<br><br>
        Skor Akhir: <b style="color:#1976D2">${scoreKiri}</b> - <b style="color:#D32F2F">${scoreKanan}</b><br>
        Posisi tali: ${ropePosition < 0 ? Math.abs(ropePosition) + ' langkah ke kiri' : ropePosition > 0 ? ropePosition + ' langkah ke kanan' : 'tengah'}<br><br>
        Ayo belajar lagi persamaan linear! 💪`;
    } else {
      content.className = 'modal-content draw';
      emoji.textContent = '🤝';
      title.textContent = 'SERI!';
      text.innerHTML = `Kedua tim sama kuatnya!<br><br>
        Skor Akhir: <b>${scoreKiri} - ${scoreKanan}</b><br>
        Posisi tali tetap di tengah!<br><br>
        Coba lagi untuk menentukan pemenang!`;
    }
    modal.classList.add('show');
  }

  function restartGame() {
    currentTurn = 0;
    scoreKiri = 0;
    scoreKanan = 0;
    ropePosition = 0;
    document.getElementById('scoreKiri').textContent = '0';
    document.getElementById('scoreKanan').textContent = '0';
    document.getElementById('modal').classList.remove('show');
    document.getElementById('flag').style.left = '50%';
    document.getElementById('teamLeft').style.left = '5%';
    document.getElementById('teamRight').style.right = '5%';
    initProgress();
    loadTurn();
  }

  document.getElementById('answer').addEventListener('keypress', (e) => {
    if (e.key === 'Enter' && !document.getElementById('submitBtn').disabled) {
      checkAnswer();
    }
  });

  initProgress();
  loadTurn();
</script>
</body>
</html>
