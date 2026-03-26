<!DOCTYPE html>
<html>
<head>
<title>node_02</title>

<style>
body{
background:black;
color:#00ff88;
font-family:"Courier New", monospace;
padding:40px;
overflow-y:auto;
scroll-behavior:smooth;
}

#terminal{
white-space:pre-wrap;
line-height:1.6;
}

button{
background:black;
color:#00ff88;
border:1px solid #00ff88;
margin:10px;
padding:10px;
cursor:pointer;
}

.hidden{
display:none;
}

.glitch{
animation:glitch 0.15s infinite;
}

@keyframes glitch{
0%{opacity:1;}
50%{opacity:0.4;}
100%{opacity:1;}
}

#return{
margin-top:50px;
opacity:0;
transition:opacity 2s;
}
</style>

</head>
<body>

<div id="gate">
<pre>
> identity verification required

> select identity:
</pre>

<button onclick="check('uglyfoid')">uglyfoid</button>
<button onclick="check('s̶̢̱̥̗̱̟͇̈́̆͜ǫ̴̘̙͔̟̜̈́̀̔̉͗͗̽̿f̷̲̩̏̉̾̓͝ḣ̷̺̖̳͓̜̈̀́́́̾̊̉͝g̸̨̣̲̘̳̹̣̼͑͆̓̑̊h̷͖̖͑́͗̔̅͛i̸̻̦̼̔̚͝ͅa̸̯̟̤̽̒͑͊̊͑̃͗̎̇')">s̶̢̱̥̗̱̟͇̈́̆͜ǫ̴̘̙͔̟̜̈́̀̔̉͗͗̽̿f̷̲̩̏̉̾̓͝ḣ̷̺̖̳͓̜̈̀́́́̾̊̉͝g̸̨̣̲̘̳̹̣̼͑͆̓̑̊h̷͖̖͑́͗̔̅͛i̸̻̦̼̔̚͝ͅa̸̯̟̤̽̒͑͊̊͑̃͗̎̇</button>
<button onclick="check('unknown')">unknown</button>
<button onclick="check('you')">you</button>

<div id="gateMsg"></div>
</div>

<div id="main" class="hidden">
<pre id="terminal"></pre>

<div id="return">
<a href="https://uglyfemcelx.github.io/TheWired/" style="color:#00ff88;">
> return to previous layer
</a>
</div>
</div>

<script>

function check(choice){

let msg = document.getElementById("gateMsg")

if(choice === "you"){
msg.innerText = "> identity accepted\n> access granted"

setTimeout(()=>{
document.getElementById("gate").style.display="none"
document.getElementById("main").classList.remove("hidden")
startNode()
},1500)

}else{
msg.innerText = "> incorrect\n> identity mismatch"
}
}

const lines = [

"[ node_02 :: unstable ]",
"",
"memory_05: overwritten",
"memory_06: duplicated",
"memory_07: not yours",
"",
"> i remember things that never happened",
"> or maybe they did",
"> just not to me",
"",
"—",
"",
"name: uglyfoid",
"name: s̶̢̱̥̗̱̟͇̈́̆͜ǫ̴̘̙͔̟̜̈́̀̔̉͗͗̽̿f̷̲̩̏̉̾̓͝ḣ̷̺̖̳͓̜̈̀́́́̾̊̉͝g̸̨̣̲̘̳̹̣̼͑͆̓̑̊h̷͖̖͑́͗̔̅͛i̸̻̦̼̔̚͝ͅa̸̯̟̤̽̒͑͊̊͑̃͗̎̇",
"name: ????",
"name: you",
"",
"> select correct identity",
"> selection failed",
"",
"—",
"",
"observer: detected",
"observer: tracking",
"observer: inside",
"",
"> you were not supposed to see this",
"",
"—",
"",
"> why did you come here",
"> this node is unstable",
"> return is recommended",
"",
"—",
"",
"> anomaly detected",
"> foreign data fragment found",
"",
"hobby_01: listening to any music",
"hobby_02: watching coryxkenshin, forever neena, miawaug, kubz scouts, h20 delirious, carto0nz, etc",
"hobby_03: wandering the wired",
"",
"> these feel real",
"> more real than the rest",
"",
"—",
"",
"fav_actress: unknown",
"fav_artist: fragmented",
"fav_idol: multiple",
"fav_anime: ???",
"",
"> attempting reconstruction...",
"",
"fav_actress: s̶̢̱̥̗̱̟͇̈́̆͜ǫ̴̘̙͔̟̜̈́̀̔̉͗͗̽̿f̷̲̩̏̉̾̓͝ḣ̷̺̖̳͓̜̈̀́́́̾̊̉͝s̶̢̱̥̗̱̟͇̈́̆͜ǫ̴̘̙͔̟̜̈́̀̔̉͗͗̽̿f̷̲̩̏̉̾̓͝ḣ̷̺̖̳͓̜̈̀́́́̾̊̉͝g̸̨̣̲̘̳̹̣̼͑͆̓̑̊h̷͖̖͑́͗̔̅͛i̸̻̦̼̔̚͝ͅa̸̯̟̤̽̒͑͊̊͑̃͗̎̇g̸̨̣̲̘̳̹̣̼͑͆̓̑̊h̷͖̖͑́͗̔̅͛i̸̻̦̼̔̚͝ͅa̸̯̟̤̽̒͑͊̊͑̃͗̎̇s̶̢̱̥̗̱̟͇̈́̆͜ǫ̴̘̙͔̟̜̈́̀̔̉͗͗̽̿f̷̲̩̏̉̾̓͝ḣ̷̺̖̳͓̜̈̀́́́̾̊̉͝g̸̨̣̲̘̳̹̣̼͑͆̓̑̊h̷͖̖͑́͗̔̅͛i̸̻̦̼̔̚͝ͅa̸̯̟̤̽̒͑͊̊͑̃͗̎̇ ",
"fav_artist: wonyoung",
"fav_idol: ayunda risu, kobo kanaeru, elizabeth rose bloodflame, gigi murin, nerissa ravencroft, usada pekora, suisei hochimachi, houshou marine",
"fav_anime: blood-c, another, the promise neverland, boku dake ga inai machi, mirai nikki, shiki, attack on titan,  coppelion, corpse party, higurashi no naku koro ni, shigatsu wa kimi no uso, himouto! umaru-chan, nagi no asukara, parasyte, tokyo ghoul, kakegurui, yarichin bi- ERROR DETECTED",
"",
"> data unstable",
"> preferences do not remain consistent",
"",
"> are these really yours",
"> or were they assigned to you",
"",
"—",
"",
"> if you want to see more",
"> access external node below",
"",
"> https://open.spotify.com/user/z7h6vgos21nu9l09kxajufoip?si=n6HFm-c9QDOZYG1LhzdAIA",
"",
"—",
"",
"ERROR: memory mismatch",
"ERROR: identity conflict",
"ERROR: user not recognized",
"",
"—",
"",
"> are you reading this",
"> or is this reading you"
]

let i = 0
let term = document.getElementById("terminal")

function startNode(){
type()
glitchText()
visitorCheck()
}

function type(){
if(i < lines.length){
term.innerHTML += lines[i] + "\n"
i++
setTimeout(type, 400)
}else{
after()
}
}

function after(){
setTimeout(()=>{
document.getElementById("return").style.opacity="1"
},3000)
}

function glitchText(){
setInterval(()=>{
if(term.innerHTML.length > 0){
term.classList.add("glitch")
setTimeout(()=>term.classList.remove("glitch"),200)
}
},2000)
}

function visitorCheck(){
if(localStorage.getItem("node2")){
setTimeout(()=>{
term.innerHTML += "\n> this node has been accessed before"
term.innerHTML += "\n> you don’t remember it"
term.innerHTML += "\n> but we do"
},3000)
}else{
localStorage.setItem("node2",true)
}
}

</script>

</body>
</html>
