<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Program Gym 5 Hari</title>

<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:wght@300;400;500;700&display=swap" rel="stylesheet">

<style>
:root {
  --bg: #eaf6ff;
  --card: #ffffff;
  --accent: #4da6ff;
  --text: #0a2540;
  --muted: #7a9bbd;
}

.light {
  --bg: #ffffff;
  --card: #f5fbff;
  --text: #0a2540;
  --muted: #9bb3c9;
}

body {
  background: linear-gradient(to bottom, #eaf6ff, #ffffff);
  color: var(--text);
  font-family: 'DM Sans', sans-serif;
  padding: 20px;
  transition: 0.3s;
}

h1 {
  font-family: 'Bebas Neue';
  font-size: 60px;
  text-align: center;
}

.tabs {
  display: flex;
  gap: 8px;
  overflow-x: auto;
  margin: 20px 0;
}

.tab {
  padding: 10px;
  background: var(--card);
  border: 1px solid #cfe6ff;
  cursor: pointer;
  border-radius: 6px;
}

.tab.active {
  background: var(--accent);
  color: #fff;
}

.day {
  display: none;
}

.day.active {
  display: block;
}

.exercise {
  background: var(--card);
  margin: 10px 0;
  padding: 15px;
  border-radius: 12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  transition: 0.2s;
  box-shadow: 0 4px 12px rgba(77,166,255,0.15);
}

.exercise:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 20px rgba(77,166,255,0.25);
}

button {
  cursor: pointer;
  border: none;
  background: var(--accent);
  color: #fff;
  padding: 6px 10px;
  border-radius: 6px;
}

.timer {
  font-size: 12px;
  color: var(--muted);
  text-align: center;
}

.progress-bar {
  height: 6px;
  background: #dcefff;
  border-radius: 10px;
  overflow: hidden;
  margin-top: 10px;
}

.progress-fill {
  height: 100%;
  background: var(--accent);
  width: 0%;
}

.toggle {
  position: fixed;
  top: 10px;
  right: 10px;
  padding: 6px 10px;
  background: var(--card);
  border: 1px solid #cfe6ff;
}
</style>
</head>

<body>

<button class="toggle" onclick="toggleMode()">🌗</button>

<h1>GYM PROGRAM</h1>

<div class="tabs">
  <button class="tab active" onclick="showDay(0)">Senin</button>
  <button class="tab" onclick="showDay(1)">Selasa</button>
  <button class="tab" onclick="showDay(2)">Rabu</button>
  <button class="tab" onclick="showDay(3)">Kamis</button>
  <button class="tab" onclick="showDay(4)">Jumat</button>
</div>

<div id="days"></div>

<script>
const data = [
["Bench Press","Incline DB Press","Cable Fly","Pushdown","Overhead Ext"],
["Deadlift","Lat Pulldown","Row","Curl","Hammer Curl"],
["Squat","RDL","Leg Press","Leg Curl","Calf Raise"],
["OHP","Lateral Raise","Face Pull","Shrug","Rear Delt"],
["Pull Up","Dips","Lunges","Weak Point","Core"]
];

const container = document.getElementById("days");

data.forEach((day, i)=>{
  let div = document.createElement("div");
  div.className = "day " + (i===0 ? "active":"");

  let html = `<h2>Hari ${i+1}</h2>
  <div class="progress-bar"><div class="progress-fill" id="progress-${i}"></div></div>`;

  day.forEach((ex,j)=>{
    const id = `d${i}e${j}`;
    html += `
    <div class="exercise">
      <label>
        <input type="checkbox" onchange="save('${id}',${i})" id="${id}">
        ${ex}
      </label>
      <div>
        <button onclick="startTimer(this)">⏱</button>
        <div class="timer">0</div>
      </div>
    </div>`;
  });

  div.innerHTML = html;
  container.appendChild(div);
});

function showDay(i){
  document.querySelectorAll(".day").forEach((d,idx)=>{
    d.classList.toggle("active", idx===i);
  });
  document.querySelectorAll(".tab").forEach((t,idx)=>{
    t.classList.toggle("active", idx===i);
  });
}

function save(id,day){
  localStorage.setItem(id, document.getElementById(id).checked);
  updateProgress(day);
}

function load(){
  data.forEach((day,i)=>{
    day.forEach((_,j)=>{
      const id = `d${i}e${j}`;
      const val = localStorage.getItem(id)==="true";
      document.getElementById(id).checked = val;
    });
    updateProgress(i);
  });
}

function updateProgress(day){
  let total = data[day].length;
  let done = 0;
  for(let j=0;j<total;j++){
    if(document.getElementById(`d${day}e${j}`).checked) done++;
  }
  document.getElementById(`progress-${day}`).style.width = (done/total*100)+"%";
}

function startTimer(btn){
  let t = btn.nextElementSibling;
  let sec = 0;
  clearInterval(btn.interval);
  btn.interval = setInterval(()=>{
    sec++;
    t.textContent = sec+"s";
  },1000);
}

function toggleMode(){
  document.body.classList.toggle("light");
}

load();
</script>

</body>
</html>
