<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Scam Shield: is this email safe?</title>
<style>
:root{--bg:#f8f7ff;--card:#fff;--ink:#1e2140;--muted:#626783;--line:#e4e2f5;--accent:#a9aefc;--ai:#14172e;--glow:rgba(169,174,252,.28);--mg:rgba(120,220,180,.16);--low:#2fae7f;--med:#e59a2e;--high:#e8647a;--mark:rgba(255,214,102,.5);--mint:#dff7ec;--peach:#ffefdc;--lilac:#ece9ff;--sky:#e1f1ff;--rose:#ffe5ea;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#12141f;--card:#1b1e2c;--ink:#eef0fa;--muted:#a1a7c0;--line:#2d3145;--accent:#a9aefc;--ai:#14172e;--glow:rgba(169,174,252,.16);--mg:rgba(63,185,138,.1);--low:#5fd6a5;--med:#ffbf5e;--high:#ff8fa0;--mark:rgba(255,214,102,.3);--mint:rgba(95,214,165,.16);--peach:rgba(255,191,94,.16);--lilac:rgba(169,174,252,.18);--sky:rgba(120,190,255,.16);--rose:rgba(255,143,160,.16)}}
:root[data-theme="dark"]{--bg:#12141f;--card:#1b1e2c;--ink:#eef0fa;--muted:#a1a7c0;--line:#2d3145;--accent:#a9aefc;--ai:#14172e;--glow:rgba(169,174,252,.16);--mg:rgba(63,185,138,.1);--low:#5fd6a5;--med:#ffbf5e;--high:#ff8fa0;--mark:rgba(255,214,102,.3);--mint:rgba(95,214,165,.16);--peach:rgba(255,191,94,.16);--lilac:rgba(169,174,252,.18);--sky:rgba(120,190,255,.16);--rose:rgba(255,143,160,.16)}
*{box-sizing:border-box}
body{margin:0;min-height:100vh;color:var(--ink);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;line-height:1.5;background:radial-gradient(600px circle at 90% -5%,var(--glow),transparent 60%),radial-gradient(500px circle at -5% 35%,var(--mg),transparent 60%),var(--bg)}
main{max-width:1040px;margin:0 auto;padding:28px 18px 56px}
header{display:flex;gap:14px;align-items:center;margin-bottom:22px}
header svg{width:48px;height:48px;flex:none;color:var(--ink);background:var(--lilac);border-radius:14px;padding:9px}
h1{margin:0;font-size:28px;letter-spacing:-.02em}
.sub{margin:2px 0 0;color:var(--muted)}
.grow{flex:1}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;align-items:start}
.side{position:sticky;top:20px}
@media (max-width:820px){.grid{grid-template-columns:1fr}.side{position:static}}
.card{background:var(--card);border:1px solid var(--line);border-radius:16px;padding:22px;box-shadow:0 8px 30px rgba(20,23,31,.06)}
label{display:flex;justify-content:space-between;font-weight:600;margin:0 0 6px}
label small{font-weight:400;color:var(--muted)}
input,textarea{width:100%;margin-bottom:18px;padding:12px 14px;font:inherit;color:inherit;background:transparent;border:1px solid var(--line);border-radius:10px;transition:border-color .2s,box-shadow .2s}
textarea{height:190px;resize:vertical}
input:focus,textarea:focus{outline:none;border-color:var(--accent);box-shadow:0 0 0 3px var(--glow)}
.row{display:flex;flex-wrap:wrap;gap:10px;align-items:center}
button{font:inherit;cursor:pointer;border-radius:10px;transition:transform .12s,border-color .2s}
button:active{transform:scale(.97)}
button:focus-visible{outline:2px solid var(--accent);outline-offset:2px}
.go{background:var(--accent);color:var(--ai);border:0;font-weight:700;padding:12px 26px}
.chip{background:transparent;color:var(--ink);border:1px solid var(--line);padding:7px 13px;font-size:14px}
.chip:hover{border-color:var(--accent)}
h2{font-size:13px;color:var(--muted);margin:18px 0 8px;font-weight:600;text-transform:uppercase;letter-spacing:.05em}
#hist{display:flex;flex-wrap:wrap;gap:8px}
#hist .chip{max-width:100%;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.empty{text-align:center;color:var(--muted);padding:40px 10px}
.empty svg{width:64px;height:64px;color:var(--line);margin-bottom:8px}
#res{--c:var(--low);border-top:4px solid var(--c)}
#res[data-risk="Medium"]{--c:var(--med)}
#res[data-risk="High"]{--c:var(--high)}
.gauge{position:relative;width:220px;margin:0 auto}
.gauge svg{display:block;width:100%}
.track,.arc{fill:none;stroke-width:14;stroke-linecap:round}
.track{stroke:var(--line)}
.arc{stroke:var(--c);stroke-dasharray:0 252;transition:stroke-dasharray .9s cubic-bezier(.2,.8,.2,1),stroke .4s}
.gnum{position:absolute;left:0;right:0;bottom:2px;text-align:center;line-height:1.1}
.gnum b{display:block;font-size:36px}
.gnum b em{font-style:normal}
.gnum b small{font-size:16px;color:var(--muted);font-weight:500}
li.s0{border-left-color:var(--high)}
.gnum span{font-weight:700;color:var(--c);font-size:15px}
.verdict{text-align:center;margin:8px 0 14px;font-size:17px;font-weight:600}
.stats{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-bottom:14px}
.stat{background:var(--bg);border-radius:12px;padding:10px;text-align:center}
.stat b{display:block;font-size:22px}
.stat span{font-size:12px;color:var(--muted)}
.tabs{display:flex;gap:6px;border-bottom:1px solid var(--line);margin-bottom:12px}
.tab{background:none;border:0;border-bottom:2px solid transparent;border-radius:0;padding:8px 10px;color:var(--muted);font-weight:600}
.tab[aria-selected="true"]{color:var(--ink);border-bottom-color:var(--c)}
ul{list-style:none;margin:0;padding:0;display:grid;gap:8px}
li{display:flex;gap:10px;padding:10px 12px;border-radius:10px;background:var(--bg);border-left:4px solid var(--line);animation:in .4s ease both}
li.s3{border-left-color:var(--high)}li.s2{border-left-color:var(--med)}li.s1{border-left-color:var(--muted)}li.ok{border-left-color:var(--low)}
li em{font-style:normal;font-weight:700;font-size:13px;min-width:28px}
@keyframes in{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}
.preview{white-space:pre-wrap;word-break:break-word;font-size:14px;max-height:220px;overflow:auto}
mark{background:var(--mark);color:inherit;border-radius:3px;padding:0 2px}
.note{color:var(--muted);font-size:12px;margin:14px 0 0}
#toast{position:fixed;left:50%;bottom:calc(24px + env(safe-area-inset-bottom,0px));transform:translate(-50%,20px);background:var(--ink);color:var(--bg);padding:10px 18px;border-radius:999px;opacity:0;pointer-events:none;transition:.3s}
#toast.on{opacity:1;transform:translate(-50%,0)}
.pills{display:flex;flex-wrap:wrap;gap:8px;margin:0 0 18px}
.pill{background:var(--lilac);color:var(--ink);border:1px solid transparent;padding:7px 12px;font-size:14px}
.pill[aria-pressed="true"]{background:var(--peach);border-color:var(--med)}
.chip.rose{background:var(--rose)}.chip.mint{background:var(--mint)}
.badge{background:var(--sky);color:var(--ink);padding:6px 12px;border-radius:999px;font-size:13px;font-weight:600}
.stat:nth-child(1){background:var(--mint)}.stat:nth-child(2){background:var(--peach)}.stat:nth-child(3){background:var(--sky)}.stat:nth-child(4){background:var(--rose)}
.tipcard{margin-top:20px;display:flex;gap:14px;align-items:center;flex-wrap:wrap;background:var(--sky)}
.tipcard p{margin:0;flex:1;min-width:200px}
.tipemoji{font-size:26px}
[hidden]{display:none!important}
@media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style>
</head>
<body>
<main>
<header>
  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M12 3l7 3v5c0 4.5-3 8-7 10-4-2-7-5.5-7-10V6l7-3z"/><path d="M9 12l2 2 4-4"/></svg>
  <div><h1>Scam Shield</h1><p class="sub">Paste a suspicious email and see how risky it looks.</p></div>
  <span class="grow"></span>
  <span class="badge" id="badge">Checks: 0</span>
  <button class="chip" id="theme" aria-label="Switch light or dark theme">Theme</button>
</header>

<div class="grid">
<section class="card">
  <label for="sender">Sender email address</label>
  <input id="sender" type="text" placeholder="someone@example.com" autocomplete="off">
  <label for="message">Email message <small id="count">0 characters</small></label>
  <textarea id="message" placeholder="Paste the email text here"></textarea>
  <h2 style="margin-top:0">Anything else feel off?</h2>
  <div class="pills" role="group" aria-label="Extra warning signs">
    <button class="pill" aria-pressed="false" data-t="It came with an unexpected attachment">📎 Unexpected attachment</button>
    <button class="pill" aria-pressed="false" data-t="I don't know the sender">🙈 Unknown sender</button>
    <button class="pill" aria-pressed="false" data-t="It pressures me to act fast">⏰ Feels rushed</button>
    <button class="pill" aria-pressed="false" data-t="It offers something too good to be true">🎁 Too good to be true</button>
  </div>
  <div class="row">
    <button class="go" id="go">Check email</button>
    <button class="chip" id="paste">📋 Paste</button>
    <button class="chip rose" id="ex1">🎣 Scam example</button>
    <button class="chip mint" id="ex2">☕ Normal example</button>
    <span class="grow"></span>
    <button class="chip" id="clear">Clear</button>
  </div>
  <div id="histbox" hidden><h2>Recent checks</h2><div id="hist"></div></div>
</section>

<section class="card side" aria-live="polite">
  <div class="empty" id="empty">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M12 3l7 3v5c0 4.5-3 8-7 10-4-2-7-5.5-7-10V6l7-3z"/></svg>
    <p>Your result will appear here.<br>Try an example, or tick any warning signs you noticed.</p>
  </div>
  <div id="res" hidden>
    <div class="gauge">
      <svg viewBox="0 0 200 110" aria-hidden="true"><path class="track" d="M20 100 A80 80 0 0 1 180 100"/><path class="arc" id="arc" d="M20 100 A80 80 0 0 1 180 100"/></svg>
      <div class="gnum"><b><em id="score">0</em><small>/10</small></b><span id="risk">Low</span></div>
    </div>
    <p class="verdict" id="verdict"></p>
    <p class="note" style="text-align:center;margin:0 0 12px">Scale: 0–2 Low · 3–5 Medium · 6–10 High</p>
    <div class="stats">
      <div class="stat"><b id="sSender">0</b><span>Sender</span></div>
      <div class="stat"><b id="sWords">0</b><span>Wording</span></div>
      <div class="stat"><b id="sLinks">0</b><span>Links</span></div>
      <div class="stat"><b id="sYou">0</b><span>Your flags</span></div>
    </div>
    <div class="tabs" role="tablist">
      <button class="tab" role="tab" data-p="p1" aria-selected="true">Reasons</button>
      <button class="tab" role="tab" data-p="p2" aria-selected="false">Highlighted</button>
      <button class="tab" role="tab" data-p="p3" aria-selected="false">What to do</button>
    </div>
    <div class="pane" id="p1"><ul id="reasons"></ul></div>
    <div class="pane preview" id="p2" hidden></div>
    <div class="pane" id="p3" hidden><ul id="tips"></ul></div>
    <div class="row" style="margin-top:14px"><button class="chip" id="copy">Copy report</button></div>
    <p class="note">Runs in your browser; nothing is sent anywhere. A rule-based check, not a guarantee.</p>
  </div>
</section>
</div>
<section class="card tipcard"><span class="tipemoji">💡</span><p id="tip"></p><button class="chip" id="tipbtn">Another tip</button></section>
</main>
<div id="toast" role="status"></div>

<script>
const FREE=["gmail.com","yahoo.com","outlook.com","hotmail.com","aol.com","icloud.com","proton.me"];
const BAD=[".xyz",".top",".click",".work",".zip",".loan",".icu",".tk",".gq",".ml",".cf",".ga"];
const SHORT=["bit.ly","tinyurl.com","t.co","goo.gl","ow.ly","is.gd","cutt.ly","rb.gy"];
const BRANDS={paypal:"paypal.com",amazon:"amazon.com",microsoft:"microsoft.com",apple:"apple.com",google:"google.com",netflix:"netflix.com",facebook:"facebook.com",dhl:"dhl.com",fedex:"fedex.com",hdfc:"hdfcbank.com",icici:"icicibank.com",sbi:"sbi.co.in"};
const URGENT=["urgent","immediately","act now","action required","within 24 hours","within 48 hours","final notice","last warning","account will be closed","account suspended","suspended","deactivated","locked","expires today","verify now","as soon as possible","asap","respond now","limited time","security alert","unusual activity","unusual sign-in","suspicious activity"];
const CREDS=["password","otp","one-time code","verification code","pin number","upi pin","card number","cvv","social security","login details","confirm your identity","verify your account","verify your identity","confirm your account","update your payment","update your billing","update your details","account number","aadhaar","pan card","kyc","sign in to","log in to"];
const MONEY=["gift card","wire transfer","bitcoin","crypto","western union","send money","processing fee","bank details","advance fee","guaranteed returns","double your","upi id","paytm"];
const PRIZE=["you have won","you won","lottery","claim your prize","congratulations","inheritance","winner","you have been selected","free gift"];
const GREET=["dear customer","dear user","dear sir/madam","dear valued","dear account holder"];
const THREAT=["legal action","arrest","warrant","police","court","penalty","will be blocked","will be terminated","will be deleted","failure to"];
const ATTACH=["see attached","open the attachment","attached invoice","enable macros","enable content","download the attachment",".exe",".zip",".scr","invoice attached","open attached"];
const BIZ=["your bank","security team","support team","customer care","customer support","account department","helpdesk","help desk","it department"];
const CLICK=["click here","click the link","click below","tap the link","follow the link","open the link"];
const VERDICT={Low:"😊 Looks fine, but stay careful.",Medium:"🤔 Be careful with this one.",High:"🚨 Likely a scam. Don't click or reply."};
const TIPS={
  Low:["Never share passwords or codes by email, even when it looks fine.","If something feels off, contact the sender using a number you already trust."],
  Medium:["Don't click links. Type the website address yourself instead.","Confirm with the sender another way before replying.","Look closely at the sender's domain spelling."],
  High:["Don't click links, reply, or open attachments.","Report it as phishing or spam, then delete it.","If you already clicked or replied, change your password and contact your bank."]};
const $=id=>document.getElementById(id);
const root=h=>{const p=h.toLowerCase().replace(/^\.|\.$/g,"").split(".");return p.length>=2?p.slice(-2).join("."):h.toLowerCase()};

function check(senderRaw,message,extras){
  let score=0;const items=[],terms=[];
  const flag=(c,p,r,t)=>{score+=p;items.push({c,p,r});if(t)terms.push(t)};
  const text=message.toLowerCase(),sender=senderRaw.trim().toLowerCase();
  const find=l=>l.find(w=>text.includes(w));
  let domain="",w;
  if(!/^[^@\s]+@[^@\s]+\.[^@\s]+$/.test(sender)) flag("s",3,"The sender address is not a valid email address");
  else{
    domain=sender.split("@")[1];
    if(BAD.some(e=>domain.endsWith(e))) flag("s",2,`The sender's domain (${domain}) ends in something often used for spam`);
    if((domain.match(/\d/g)||[]).length>=3) flag("s",1,"The sender's domain contains many numbers");
    if((domain.match(/-/g)||[]).length>=2) flag("s",1,"The sender's domain has several hyphens, common in fake domains");
  }
  const cleaned=domain.replace(/0/g,"o").replace(/1/g,"l").replace(/3/g,"e").replace(/5/g,"s");
  for(const [b,real] of Object.entries(BRANDS)){
    const isReal=domain===real||domain.endsWith("."+real),n=b[0].toUpperCase()+b.slice(1);
    if(domain&&cleaned.includes(b)&&!isReal){flag("s",3,`The sender's domain imitates ${n} but is not ${real}`);break}
    if(domain&&new RegExp("\\b"+b+"\\b").test(text)&&!isReal){
      const f=FREE.includes(domain);
      flag("s",f?3:2,f?`The email talks about ${n} but was sent from a free address (${domain})`:`The email mentions ${n} but was not sent from ${real}`,b);break}
  }
  const u=find(URGENT),c=find(CREDS),m=find(MONEY),pz=find(PRIZE),th=find(THREAT),at=find(ATTACH),bz=find(BIZ),ck=find(CLICK);
  if(u) flag("w",2,`Uses pressure or urgent language ("${u}")`,u);
  if(c) flag("w",3,`Asks for private information ("${c}")`,c);
  if(m) flag("w",3,`Mentions a risky way of sending money ("${m}")`,m);
  if(pz) flag("w",2,"Talks about winning a prize or receiving unexpected money",pz);
  if(th) flag("w",2,`Threatens consequences ("${th}")`,th);
  if(at) flag("w",2,`Pushes you to open an attachment ("${at}")`,at);
  if(ck) flag("w",1,`Tells you to click a link ("${ck}")`,ck);
  if(bz&&FREE.includes(domain)) flag("s",2,"Sounds official but was sent from a free email address");
  if(w=find(GREET)) flag("w",1,"Uses a generic greeting instead of your name",w);
  if((message.match(/!/g)||[]).length>=4) flag("w",1,"Uses a lot of exclamation marks");
  const L=(message.match(/[A-Za-z]/g)||[]).length,U=(message.match(/[A-Z]/g)||[]).length;
  if(L>40&&U/L>.4) flag("w",1,"Has a lot of text in ALL CAPS");
  const links=message.match(/(?:https?:\/\/|www\.)[^\s<>"')]+/gi)||[],hosts=[];
  for(const link of links){
    let host="";
    try{host=new URL(/^http/i.test(link)?link:"http://"+link).hostname.toLowerCase()}catch(e){continue}
    hosts.push(host);
    if(/^\d{1,3}(\.\d{1,3}){3}$/.test(host)) flag("l",3,"A link uses a raw IP address instead of a website name",link);
    else if(SHORT.includes(host)) flag("l",2,`A link is shortened (${host}), so you can't see where it goes`,link);
    else if(BAD.some(e=>host.endsWith(e))) flag("l",2,`A link goes to ${host}, which ends in something often used for spam`,link);
    if(/^http:\/\//i.test(link)) flag("l",1,"A link is not secure (it starts with http, not https)",link);
  }
  if(hosts.length&&domain&&!hosts.some(h=>root(h)===root(domain))) flag("l",1,"The links go to a different website than the sender's domain");
  if(links.length>=4) flag("l",1,"Contains many links");
  if(c&&links.length) flag("w",2,"Asks for private information and also includes a link");
  if(u&&(c||m)) flag("w",2,"Combines pressure with a request for private information or money");
  if(items.some(i=>/imitates/.test(i.r))&&links.length) flag("l",2,"Imitates a known company and pushes you to a link");
  extras.forEach(t=>flag("y",1,"You noted: "+t));
  const sum=c=>items.filter(i=>i.c===c).reduce((a,i)=>a+i.p,0);
  const crit=items.some(i=>/imitates|raw IP/.test(i.r))||!!m||!!(c&&(links.length||u))||/enable macros|\.exe|\.scr/.test(text);
  if(crit&&score<7) items.push({c:"w",p:0,r:"Contains a serious danger sign, so this is rated High"});
  const s10=Math.min(10,crit?Math.max(score,7):score);
  return{score:s10,items,terms,nLinks:links.length,sS:sum("s"),sW:sum("w"),sY:sum("y"),risk:s10>=6?"High":s10>=3?"Medium":"Low"};
}

function highlight(el,message,terms){
  el.textContent="";
  const list=[...new Set(terms.filter(Boolean))].sort((a,b)=>b.length-a.length);
  if(!list.length){el.textContent=message;return}
  const re=new RegExp(list.map(t=>t.replace(/[.*+?^${}()|[\]\\]/g,"\\$&")).join("|"),"gi");
  let last=0,m;
  while((m=re.exec(message))){
    el.append(message.slice(last,m.index));
    const mk=document.createElement("mark");mk.textContent=m[0];el.append(mk);
    last=m.index+m[0].length;
  }
  el.append(message.slice(last));
}

function fillList(ul,rows){
  ul.textContent="";
  rows.forEach((r,i)=>{
    const li=document.createElement("li");li.className=r.cls;li.style.animationDelay=(i*70)+"ms";
    const b=document.createElement("em");b.textContent=r.tag;
    const t=document.createElement("span");t.textContent=r.text;
    li.append(b,t);ul.append(li);
  });
}

function toast(msg){const t=$("toast");t.textContent=msg;t.classList.add("on");clearTimeout(t._h);t._h=setTimeout(()=>t.classList.remove("on"),2000)}

let live=false,timer,last=null,history=[],checks=0;
function run(save){
  const sender=$("sender").value,message=$("message").value;
  if(!sender.trim()||!message.trim()){toast("Enter a sender and a message first");return}
  const extras=[...document.querySelectorAll(".pill[aria-pressed=true]")].map(p=>p.dataset.t);
  const r=check(sender,message,extras);last={r,sender};
  $("empty").hidden=true;$("res").hidden=false;$("res").dataset.risk=r.risk;
  $("risk").textContent=r.risk;$("score").textContent=r.score;$("verdict").textContent=VERDICT[r.risk];
  $("sSender").textContent=r.sS;$("sWords").textContent=r.sW;$("sLinks").textContent=r.nLinks;$("sYou").textContent=r.sY;
  fillList($("reasons"),r.items.length?r.items.map(i=>({cls:"s"+Math.min(i.p,3),tag:"+"+i.p,text:i.r})):[{cls:"ok",tag:"OK",text:"No warning signs found in the sender or the message"}]);
  fillList($("tips"),TIPS[r.risk].map(t=>({cls:"ok",tag:"→",text:t})));
  highlight($("p2"),message,r.terms);
  const arc=$("arc");arc.style.strokeDasharray="0 252";
  requestAnimationFrame(()=>requestAnimationFrame(()=>{arc.style.strokeDasharray=(r.score/10*251.3)+" 252"}));
  live=true;
  if(save){
    checks++;$("badge").textContent="Checks: "+checks;
    history=[{sender,message,risk:r.risk},...history.filter(h=>h.sender!==sender||h.message!==message)].slice(0,5);
    const box=$("hist");box.textContent="";$("histbox").hidden=false;
    history.forEach(h=>{const b=document.createElement("button");b.className="chip";b.textContent=h.risk+" · "+h.sender;b.onclick=()=>{$("sender").value=h.sender;$("message").value=h.message;count();run(false)};box.append(b)});
    if(window.innerWidth<=820)$("res").scrollIntoView({behavior:"smooth",block:"start"});
  }
}
function count(){$("count").textContent=$("message").value.length+" characters"}
function fill(s,m){$("sender").value=s;$("message").value=m;count();run(true)}

const FACTS=["Real companies rarely ask for your password by email.","Hover over a link before clicking. Does the address match the sender?","Urgent deadlines are a favorite scammer trick. Slow down.","A tiny typo in a domain, like paypa1, is a classic giveaway.","When in doubt, open the official app or type the website yourself.","Prizes you never entered for are almost never real."];
let ti=Math.floor(Math.random()*FACTS.length);
const showTip=()=>{$("tip").textContent=FACTS[ti%FACTS.length]};
$("tipbtn").onclick=()=>{ti++;showTip()};showTip();
document.querySelectorAll(".pill").forEach(p=>p.onclick=()=>{p.setAttribute("aria-pressed",p.getAttribute("aria-pressed")!=="true");if(live)run(false)});
$("paste").onclick=async()=>{try{$("message").value=await navigator.clipboard.readText();count();toast("Pasted")}catch(e){toast("Allow clipboard access, or paste with Ctrl+V")}};
$("go").onclick=()=>run(true);
$("ex1").onclick=()=>fill("support@paypa1-security.xyz","URGENT! Dear customer, your PayPal account will be closed. Verify your password now at http://bit.ly/abc123");
$("ex2").onclick=()=>fill("anna@company.com","Hi team, lunch is at 1pm on Friday. Menu is here: https://company.com/menu");
$("clear").onclick=()=>{$("sender").value="";$("message").value="";count();$("res").hidden=true;$("empty").hidden=false;live=false;document.querySelectorAll(".pill").forEach(p=>p.setAttribute("aria-pressed","false"));$("sender").focus()};
$("theme").onclick=()=>{const el=document.documentElement,dark=(el.dataset.theme||(matchMedia("(prefers-color-scheme:dark)").matches?"dark":"light"))==="dark";el.dataset.theme=dark?"light":"dark"};
$("copy").onclick=async()=>{
  if(!last)return;
  const t=`Scam Shield: ${last.r.risk} risk (score ${last.r.score}/10)\nSender: ${last.sender}\n`+(last.r.items.length?last.r.items.map(i=>"- "+i.r).join("\n"):"- No warning signs found");
  try{await navigator.clipboard.writeText(t);toast("Report copied")}catch(e){toast("Couldn't copy on this browser")}
};
document.querySelectorAll(".tab").forEach(b=>b.onclick=()=>{
  document.querySelectorAll(".tab").forEach(x=>x.setAttribute("aria-selected",x===b));
  document.querySelectorAll(".pane").forEach(p=>p.hidden=p.id!==b.dataset.p);
});
["sender","message"].forEach(id=>$(id).addEventListener("input",()=>{count();if(!live)return;clearTimeout(timer);timer=setTimeout(()=>run(false),300)}));
</script>
</body>
</html>
