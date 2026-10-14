

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Free 30-Day Challenge Tracker: Track Habits and Goals Online</title>
<meta name="description" content="A free, simple 30-day challenge tracker. Add your own goals, check off each day, and watch your streaks grow. No sign-up, works on phone and desktop.">
<link rel="canonical" href="https://YOUR-DOMAIN.com/">
<meta property="og:type" content="website">
<meta property="og:title" content="Free 30-Day Challenge Tracker">
<meta property="og:description" content="Pick your goals, tick off 30 days, and build streaks. No sign-up needed.">
<meta property="og:url" content="https://YOUR-DOMAIN.com/">
<meta name="twitter:card" content="summary">
<script type="application/ld+json">{"@context":"https://schema.org","@type":"WebApplication","name":"30-Day Challenge Tracker","description":"Free online tracker for 30-day goals and habits with streaks and progress.","applicationCategory":"LifestyleApplication","operatingSystem":"Any","offers":{"@type":"Offer","price":"0","priceCurrency":"USD"}}</script>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@400;600;800&display=swap">
<style>
:root{--bg:#EAF1EE;--surface:#fff;--ink:#12302A;--mute:#5F7A73;--line:#CBDAD5;--accent:#0F766E;--sun:#F2B134;--empty:#E1EBE8;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0E1B18;--surface:#152723;--surface:#152723;--ink:#E3F0EC;--mute:#8FB0A7;--line:#254039;--accent:#2DD4BF;--sun:#F5C158;--empty:#1D332E}}
:root[data-theme="dark"]{--bg:#0E1B18;--surface:#152723;--ink:#E3F0EC;--mute:#8FB0A7;--line:#254039;--accent:#2DD4BF;--sun:#F5C158;--empty:#1D332E}
*,*:before,*:after{box-sizing:inherit}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--ink);font-family:"Bricolage Grotesque",system-ui,-apple-system,"Segoe UI",sans-serif;line-height:1.45}
main{max-width:560px;margin:0 auto;padding:20px 16px 40px}
h1{font-size:15px;font-weight:600;color:var(--mute);margin:0 0 6px}
.hero{display:flex;align-items:baseline;gap:10px;flex-wrap:wrap}
.big{font-size:clamp(64px,22vw,104px);font-weight:800;line-height:.9;letter-spacing:-.04em}
.of{font-size:22px;font-weight:600;color:var(--mute)}
.left{margin:8px 0 14px;font-size:17px}
.bar{height:12px;background:var(--empty);border-radius:6px;overflow:hidden}
.bar i{display:block;height:100%;width:0;background:var(--accent);transition:width .4s}
.stat{display:flex;justify-content:space-between;font-size:13px;color:var(--mute);margin:6px 0 22px}
.goal{background:var(--surface);border:1px solid var(--line);border-radius:14px;padding:14px;margin-bottom:14px}
.gh{display:flex;justify-content:space-between;align-items:center;gap:8px;margin-bottom:10px}
.gh b{font-size:18px}
.gm{font-size:13px;color:var(--mute);white-space:nowrap}
.gm em{font-style:normal;color:var(--ink);font-weight:600}
.grid{display:grid;grid-template-columns:repeat(10,1fr);gap:5px}
.d{aspect-ratio:1;border:0;padding:0;border-radius:6px;background:var(--empty);color:var(--mute);font:600 11px/1 inherit;font-family:inherit;cursor:pointer}
.d.on{background:var(--accent);color:var(--bg)}
.d.today{outline:2px solid var(--sun);outline-offset:1px}
.d.fut{opacity:.4;cursor:default}
.d:focus-visible,button:focus-visible,input:focus-visible{outline:3px solid var(--sun);outline-offset:2px}
.rm{background:none;border:0;color:var(--mute);font:inherit;font-size:12px;cursor:pointer;padding:8px 0 0}
form{display:flex;gap:8px;margin:18px 0}
input{font:inherit;font-size:16px;padding:11px 12px;border-radius:10px;border:1px solid var(--line);background:var(--surface);color:var(--ink);min-width:0}
input[type=text]{flex:1}
.add{font:inherit;font-weight:600;padding:11px 16px;border-radius:10px;border:0;background:var(--accent);color:var(--bg);cursor:pointer}
.set{display:flex;gap:10px;align-items:center;justify-content:space-between;font-size:13px;color:var(--mute);flex-wrap:wrap;margin-top:24px}
.set button{font:inherit;font-size:13px;background:none;border:1px solid var(--line);color:var(--mute);border-radius:8px;padding:6px 10px;cursor:pointer}
.about{margin-top:26px;font-size:15px;color:var(--mute)}.about h2{font-size:16px;color:var(--ink);margin:0 0 6px}
.empty{text-align:center;color:var(--mute);padding:20px 0}
.done{background:var(--sun);color:#1b1500;border-radius:12px;padding:12px 14px;margin-bottom:14px;font-weight:600;display:none}
</style>
</head>
<body>
<main>
  <h1 id="title">Free 30-day challenge tracker</h1>
  <div class="hero"><span class="big" id="day">1</span><span class="of">of 30 days</span></div>
  <div class="left" id="left"></div>
  <div class="bar"><i id="fill"></i></div>
  <div class="stat"><span id="pct">0% of check-ins done</span><span id="best"></span></div>
  <div class="done" id="done">Month complete. Look at everything you did.</div>
  <div id="goals"></div>
  <form id="f">
    <input type="text" id="n" placeholder="Add a goal, e.g. Walk 5 km" maxlength="40" aria-label="New goal">
    <button class="add" type="submit">Add goal</button>
  </form>
  <section class="about">
    <h2>How it works</h2>
    <p>Add the goals you want to build into a habit, like exercise, reading, or learning a skill. Each day, tap the matching square to check it off. Your streaks and progress update automatically, and everything stays saved in your browser. No account needed.</p>
  </section>
  <div class="set">
    <label>Day 1 is <input type="date" id="start"></label>
    <button id="reset" type="button">Start over</button>
  </div>
</main>
<script>
var KEY="month30-v1",N=30,DAY=864e5;
function iso(d){var m=d.getMonth()+1,x=d.getDate();return d.getFullYear()+"-"+(m<10?"0":"")+m+"-"+(x<10?"0":"")+x}
function load(){try{var s=localStorage.getItem(KEY);if(s)return JSON.parse(s)}catch(e){}return null}
function save(){try{localStorage.setItem(KEY,JSON.stringify(S))}catch(e){}}
var S=load()||{start:iso(new Date()),goals:[{id:1,name:"Move my body",days:{}},{id:2,name:"Read 20 pages",days:{}},{id:3,name:"Learn something new",days:{}}]};
var $=function(i){return document.getElementById(i)};
function today(){var a=new Date(S.start+"T00:00:00"),b=new Date(iso(new Date())+"T00:00:00");return Math.round((b-a)/DAY)+1}
function streak(g,t){var c=0,i=Math.min(t,N);if(!g.days[i])i--;for(;i>=1&&g.days[i];i--)c++;return c}
function render(){
  var t=today(),cur=Math.max(1,Math.min(t,N)),el=$("goals");
  $("day").textContent=t<1?"0":cur;
  $("left").textContent=t<1?"Starts in "+(1-t)+" day"+(1-t>1?"s":""):t>N?"The 30 days are over.":(N-t===0?"Last day. Finish strong.":(N-t)+" days left");
  $("done").style.display=t>N?"block":"none";
  var tot=0,poss=Math.max(0,Math.min(t,N))*S.goals.length,best=0;
  el.innerHTML="";
  if(!S.goals.length)el.innerHTML='<div class="empty">No goals yet. Add one below to begin.</div>';
  S.goals.forEach(function(g){
    var n=0;for(var k in g.days)if(g.days[k])n++;tot+=n;
    var st=streak(g,t);if(st>best)best=st;
    var c=document.createElement("div");c.className="goal";
    var h='<div class="gh"><b></b><span class="gm"><em>'+st+'</em> day streak &middot; '+n+'/30</span></div><div class="grid">';
    for(var i=1;i<=N;i++){
      var cls="d"+(g.days[i]?" on":"")+(i===t?" today":"")+(i>t?" fut":"");
      h+='<button class="'+cls+'" data-g="'+g.id+'" data-d="'+i+'" aria-pressed="'+!!g.days[i]+'" aria-label="Day '+i+'">'+i+'</button>';
    }
    h+='</div><button class="rm" data-rm="'+g.id+'">Remove goal</button>';
    c.innerHTML=h;c.querySelector("b").textContent=g.name;el.appendChild(c);
  });
  var p=poss?Math.round(tot/poss*100):0;
  $("fill").style.width=p+"%";
  $("pct").textContent=p+"% of check-ins done";
  $("best").textContent=best?"Best streak: "+best+" days":"";
  $("start").value=S.start;
}
$("goals").addEventListener("click",function(e){
  var b=e.target.closest("button");if(!b)return;
  if(b.dataset.rm){S.goals=S.goals.filter(function(g){return g.id!=b.dataset.rm});save();render();return}
  if(b.dataset.d){var d=+b.dataset.d;if(d>today())return;
    S.goals.forEach(function(g){if(g.id==b.dataset.g){g.days[d]=!g.days[d]}});save();render()}
});
$("f").addEventListener("submit",function(e){e.preventDefault();var v=$("n").value.trim();if(!v)return;
  S.goals.push({id:Date.now(),name:v,days:{}});$("n").value="";save();render()});
$("start").addEventListener("change",function(){if(this.value){S.start=this.value;save();render()}});
$("reset").addEventListener("click",function(){
  if(!confirm("Clear all check-ins and start Day 1 today?"))return;
  S.start=iso(new Date());S.goals.forEach(function(g){g.days={}});save();render()});
render();
</script>
</body>
</html>
