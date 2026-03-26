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
overflow:hidden;
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
margin-top:30px;
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
<button onclick="check('ş̷̧̠̼̩͍͚̰̭̬͗̊͊̿͋̌̌̒͝o̴̢̞͍͎̣̻̞͓̓̈͒̏̕k̸̨͖̠̮̳̭̞̅̈́̋̑̂͆̈̚̕͜f̸̣̠͂́i̸̼̱̰͓̻͙̰̻̜̇̐̽͋̈́̈́̚̚ạ̵͈͍͐̔')">ş̷̧̠̼̩͍͚̰̭̬͗̊͊̿͋̌̌̒͝o̴̢̞͍͎̣̻̞͓̓̈͒̏̕k̸̨͖̠̮̳̭̞̅̈́̋̑̂͆̈̚̕͜f̸̣̠͂́i̸̼̱̰͓̻͙̰̻̜̇̐̽͋̈́̈́̚̚ạ̵͈͍͐̔</button>
<button onclick="check('unknown')">unknown</button>
<button onclick="check('you')">you</button>

<div id="gateMsg"></div>
</div>

<div id="main" class="hidden">
<pre id="terminal"></pre>

<div id="return">
<a href="https://uglyfemcelx.github.io/node_1/" style="color:#00ff88;">
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

// main content
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
"name: sofia",
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

// random glitch replace
function glitchText(){
setInterval(()=>{
if(term.innerHTML.length > 0){
term.classList.add("glitch")
setTimeout(()=>term.classList.remove("glitch"),200)
}
},2000)
}

// returning visitor
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
