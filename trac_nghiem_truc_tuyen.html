<!doctype html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Bài kiểm tra trực tuyến — 40 câu</title>
  <style>
    :root{--bg:#f4f7fb;--card:#fff;--accent:#0f62fe;--muted:#6b7280;--danger:#dc2626;--glass:rgba(255,255,255,0.6)}
    *{box-sizing:border-box}
    body{font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;margin:0;background:linear-gradient(180deg,#eef2ff 0%,var(--bg) 100%);color:#0f172a}
    .wrap{max-width:1100px;margin:28px auto;padding:20px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700}
    h1{margin:0;font-size:20px}
    .intro{margin-top:18px;padding:18px;border-radius:12px;background:var(--card);box-shadow:0 6px 18px rgba(12,28,63,0.06)}
    .start-grid{display:grid;grid-template-columns:1fr 360px;gap:20px}
    .field{display:flex;flex-direction:column;margin-bottom:12px}
    label{font-size:13px;color:var(--muted);margin-bottom:6px}
    input[type=text]{padding:10px 12px;border:1px solid #e6e9ef;border-radius:8px;font-size:14px}
    button.btn{background:var(--accent);color:#fff;padding:10px 14px;border-radius:10px;border:0;font-weight:600;cursor:pointer}
    button.ghost{background:transparent;border:1px solid #dbeafe;color:var(--accent)}
    .exam{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:18px}
    .panel{background:var(--card);border-radius:12px;padding:16px;box-shadow:0 8px 30px rgba(12,28,63,0.06)}
    .question{padding:14px;border-radius:10px;border:1px solid #eef2ff;margin-bottom:12px}
    .q-title{font-weight:600}
    .options{display:flex;flex-direction:column;margin-top:10px;gap:8px}
    .option{display:flex;align-items:center;gap:10px;padding:10px;border-radius:8px;border:1px solid #eef2ff;cursor:pointer}
    .option input{accent-color:var(--accent)}
    .sidebar .meta{display:flex;justify-content:space-between;align-items:center}
    .timer{font-size:20px;font-weight:700;color:var(--accent)}
    .nav-grid{display:grid;grid-template-columns:repeat(5,1fr);gap:8px;margin-top:12px}
    .nav-grid button{padding:8px;border-radius:8px;border:1px solid #e6eefc;background:transparent;cursor:pointer}
    .nav-grid button.answered{background:#ecfdf5;border-color:#bbf7d0}
    #ket-qua{margin-top:12px;padding:12px;border-radius:10px;background:linear-gradient(90deg,#f0fdf4,#ffffff);border:1px solid #d1fae5}
    footer{margin-top:16px;font-size:13px;color:var(--muted)}
    @media(max-width:920px){.start-grid{grid-template-columns:1fr}.exam{grid-template-columns:1fr}.sidebar{order:2}}
  </style>
</head>
<body>
<div class="wrap">
  <div class="brand">
    <div class="logo">IT</div>
    <div>
      <h1>Bài kiểm tra trực tuyến — 40 câu</h1>
      <div style="color:var(--muted);font-size:13px;margin-top:6px">Thời gian: <strong>40 phút</strong> · Có chống gian lận và lưu kết quả Google Sheet</div>
    </div>
  </div>

  <div class="intro panel">
    <div id="startScreen">
      <div class="start-grid">
        <div>
          <p>Nhập <strong>Họ tên</strong> và <strong>Lớp</strong> để làm bài. Kết quả sẽ được tự động gửi lên Google Sheet khi nộp bài hoặc khi thoát màn hình làm bài.</p>
          <div class="field"><label>Họ và tên</label><input id="studentName" type="text" placeholder="Nguyễn Văn A" /></div>
          <div class="field"><label>Lớp</label><input id="studentClass" type="text" placeholder="11A1" /></div>
          <button id="startBtn" class="btn">Bắt đầu làm bài</button>
        </div>
        <div style="width:100%;height:160px;border-radius:12px;overflow:hidden;background-image:url('https://images.unsplash.com/photo-1581091012184-7d7a972a6458?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80');background-size:cover;background-position:center;box-shadow:inset 0 0 0 2000px rgba(2,6,23,0.18)"></div>
      </div>
    </div>

    <div id="examArea" style="display:none">
      <div class="exam">
        <div>
          <div id="questionsContainer"></div>
          <div style="display:flex;gap:8px;justify-content:flex-end;margin-top:8px">
            <button id="submitBtn" class="btn">Nộp bài</button>
          </div>
        </div>
        <aside class="sidebar panel">
          <div class="meta">
            <div>
              <div style="font-size:13px;color:var(--muted)">Học sinh</div>
              <div id="displayName" style="font-weight:700;font-size:16px">-</div>
              <div id="displayClass" style="color:var(--muted);font-size:13px">-</div>
            </div>
            <div>
              <div style="font-size:13px;color:var(--muted);text-align:right">Thời gian</div>
              <div id="timer" class="timer">40:00</div>
            </div>
          </div>
          <div class="nav-grid" id="navGrid"></div>
          <div id="ket-qua">Kết quả: <strong id="resultText">Chưa nộp</strong></div>
        </aside>
      </div>
    </div>
  </div>
  <footer>Phiên bản có gửi kết quả Google Sheet — cần cấu hình script Google Apps Script (API endpoint).</footer>
</div>

<script>
const GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/YOUR_DEPLOYMENT_ID/exec"; // thay link Apps Script sau khi triển khai
const TOTAL_QUESTIONS = 40;
const DURATION = 40*60;
let state={answers:{},name:'',class:'',timeLeft:DURATION,timer:null,submitted:false};
const startBtn=document.getElementById('startBtn');
const startScreen=document.getElementById('startScreen');
const examArea=document.getElementById('examArea');
const questionsContainer=document.getElementById('questionsContainer');
const displayName=document.getElementById('displayName');
const displayClass=document.getElementById('displayClass');
const timerEl=document.getElementById('timer');
const resultText=document.getElementById('resultText');
const submitBtn=document.getElementById('submitBtn');
const navGrid=document.getElementById('navGrid');

const questions=Array.from({length:TOTAL_QUESTIONS},(_,i)=>({id:i+1,q:`Câu ${i+1}: Ví dụ câu hỏi ${i+1}.`,options:{A:'Đáp án A',B:'Đáp án B',C:'Đáp án C',D:'Đáp án D'},answer:'A'}));

startBtn.onclick=()=>{
 const n=document.getElementById('studentName').value.trim();
 const c=document.getElementById('studentClass').value.trim();
 if(!n||!c)return alert('Nhập đủ họ tên và lớp.');
 state.name=n;state.class=c;
 displayName.textContent=n;displayClass.textContent=c;
 startScreen.style.display='none';examArea.style.display='block';
 renderQuestions();renderNav();startTimer();setupAntiCheat();
};

function renderQuestions(){questionsContainer.innerHTML='';questions.forEach(q=>{let d=document.createElement('div');d.className='question';d.innerHTML=`<div class='q-title'>${q.q}</div>`+Object.entries(q.options).map(([k,v])=>`<label class='option'><input type='radio' name='q${q.id}' value='${k}'/> ${k}. ${v}</label>`).join('');questionsContainer.appendChild(d);d.querySelectorAll('input').forEach(inp=>inp.onchange=e=>{state.answers[q.id]=e.target.value;updateNav();});});}
function renderNav(){navGrid.innerHTML='';for(let i=1;i<=TOTAL_QUESTIONS;i++){let b=document.createElement('button');b.textContent=i;b.onclick=()=>document.getElementById(`q-${i}`)?.scrollIntoView({behavior:'smooth'});navGrid.appendChild(b);}updateNav();}
function updateNav(){navGrid.querySelectorAll('button').forEach((b,i)=>{b.classList.toggle('answered',!!state.answers[i+1]);});}

function startTimer(){updateTimer();state.timer=setInterval(()=>{state.timeLeft--;updateTimer();if(state.timeLeft<=0){clearInterval(state.timer);submitExam('Hết thời gian');}},1000);}
function updateTimer(){let m=Math.floor(state.timeLeft/60).toString().padStart(2,'0');let s=(state.timeLeft%60).toString().padStart(2,'0');timerEl.textContent=`${m}:${s}`;}

function submitExam(reason){if(state.submitted)return;state.submitted=true;clearInterval(state.timer);let correct=0;questions.forEach(q=>{if(state.answers[q.id]===q.answer)correct++;});let score=(correct/TOTAL_QUESTIONS*10).toFixed(1);resultText.textContent=`${score}/10 (${correct}/${TOTAL_QUESTIONS} đúng)`;sendToSheet({name:state.name,class:state.class,correct,score,reason,time:new Date().toISOString()});alert('Bài đã nộp!');}

submitBtn.onclick=()=>{if(confirm('Nộp bài ngay?'))submitExam('Tự nguyện');};

function sendToSheet(data){fetch(GOOGLE_SCRIPT_URL,{method:'POST',mode:'no-cors',headers:{'Content-Type':'application/json'},body:JSON.stringify(data)}).catch(e=>console.error(e));}

function setupAntiCheat(){document.addEventListener('visibilitychange',()=>{if(document.hidden){submitExam('Thoát màn hình');}});window.addEventListener('blur',()=>{submitExam('Rời cửa sổ');});window.addEventListener('beforeunload',e=>{if(!state.submitted){submitExam('Đóng tab');}});}
</script>
</body>
</html>
