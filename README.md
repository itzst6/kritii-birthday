# kritii-birthday
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Kriti ❤️</title>
<style>
body{
margin:0;
font-family:'Segoe UI',sans-serif;
background:linear-gradient(135deg,#ff9a9e,#fad0c4);
height:100vh;
display:flex;
align-items:center;
justify-content:center;
overflow:hidden;
}

.box{
width:220px;
height:220px;
background:#ff6b81;
border-radius:15px;
position:relative;
cursor:pointer;
box-shadow:0 10px 25px rgba(0,0,0,0.2);
display:flex;
align-items:center;
justify-content:center;
color:white;
font-size:20px;
font-weight:bold;
}

.ribbon{
position:absolute;
width:100%;
height:30px;
background:#fff;
top:50%;
transform:translateY(-50%);
}

.ribbon:before{
content:"";
position:absolute;
height:100%;
width:30px;
background:#fff;
left:50%;
transform:translateX(-50%);
}

.letter{
position:absolute;
width:80%;
max-width:500px;
background:white;
padding:30px;
border-radius:15px;
box-shadow:0 10px 25px rgba(0,0,0,0.3);
text-align:center;
display:none;
animation:fade 1s ease;
}

.letter h1{
color:#ff4d6d;
}

.butterfly{
position:absolute;
font-size:24px;
animation:fly 6s linear infinite;
}

@keyframes fly{
0%{transform:translateY(100vh) translateX(0);} 
100%{transform:translateY(-100vh) translateX(200px);} 
}

@keyframes fade{
from{opacity:0;transform:scale(0.8);} 
to{opacity:1;transform:scale(1);} 
}
</style>
</head>

<body>

<div class="box" onclick="openGift()">
Open Me 🎁
<div class="ribbon"></div>
</div>

<div class="letter" id="letter">
<h1>Happy Birthday Kriti 🎂❤️</h1>
<p>
My dearest Kriti (my cute Mum),
<br><br>
From the moment you came into my life, everything started feeling more beautiful. Your smile, your voice, your presence — they mean the world to me.
<br><br>
On your special day, I just want you to know how incredibly important you are to me. You are not just my girlfriend, you are my happiness, my comfort, and the most precious person in my life.
<br><br>
I promise to stand by your side, support you, protect you, and love you with all my heart.
<br><br>
Happy Birthday my love. May your life always be filled with happiness, laughter, dreams and endless love.
<br><br>
Forever yours ❤️
</p>
</div>

<script>
function openGift(){
document.querySelector('.box').style.display='none';
document.getElementById('letter').style.display='block';

for(let i=0;i<20;i++){
let b=document.createElement('div');
b.className='butterfly';
b.innerHTML='🦋';
b.style.left=Math.random()*100+'vw';
b.style.animationDuration=(3+Math.random()*5)+'s';
document.body.appendChild(b);
}
}
</script>

</body>
</html>
