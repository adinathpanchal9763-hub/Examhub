<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>JEE PYQ Download | Free Study Material</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
    margin:0;
    font-family: Arial, sans-serif;
    background:#f5f7fa;
}
header{
    background:#0d6efd;
    color:white;
    padding:15px;
    text-align:center;
}
.container{
    max-width:900px;
    margin:auto;
    padding:15px;
}
.subject{
    background:white;
    margin-bottom:20px;
    padding:15px;
    border-radius:10px;
    box-shadow:0 2px 5px rgba(0,0,0,0.1);
}
.subject h2{
    margin-top:0;
}
.year{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:8px 0;
    border-bottom:1px solid #ddd;
}
.year:last-child{border-bottom:none;}
.download-btn{
    background:#0d6efd;
    color:white;
    border:none;
    padding:6px 12px;
    border-radius:5px;
    cursor:pointer;
}
.download-btn:hover{
    background:#084298;
}

/* Ad Modal */
.modal{
    display:none;
    position:fixed;
    top:0;left:0;
    width:100%;height:100%;
    background:rgba(0,0,0,0.6);
    z-index:1000;
}
.modal-content{
    background:white;
    width:300px;
    margin:20% auto;
    padding:15px;
    text-align:center;
    border-radius:10px;
}
.ad-box{
    height:100px;
    background:#eee;
    display:flex;
    align-items:center;
    justify-content:center;
    margin:10px 0;
    font-weight:bold;
}
#finalDownload{
    background:#198754;
    color:white;
    border:none;
    padding:8px 14px;
    border-radius:5px;
    cursor:not-allowed;
}
footer{
    text-align:center;
    font-size:14px;
    color:#555;
    padding:10px;
}
</style>
</head>

<body>

<header>
<h1>JEE Previous Year Question Papers</h1>
<p>Free Downloads • Physics • Chemistry • Maths</p>
</header>

<div class="container">

<!-- PHYSICS -->
<div class="subject">
<h2>Physics</h2>
<div class="year"><span>2024</span><button class="download-btn" onclick="showAd('downloads/jee/physics/2024.pdf')">Download</button></div>
<div class="year"><span>2023</span><button class="download-btn" onclick="showAd('downloads/jee/physics/2023.pdf')">Download</button></div>
<div class="year"><span>2022</span><button class="download-btn" onclick="showAd('downloads/jee/physics/2022.pdf')">Download</button></div>
<div class="year"><span>2021</span><button class="download-btn" onclick="showAd('downloads/jee/physics/2021.pdf')">Download</button></div>
<div class="year"><span>2020</span><button class="download-btn" onclick="showAd('downloads/jee/physics/2020.pdf')">Download</button></div>
</div>

<!-- CHEMISTRY -->
<div class="subject">
<h2>Chemistry</h2>
<div class="year"><span>2024</span><button class="download-btn" onclick="showAd('downloads/jee/chemistry/2024.pdf')">Download</button></div>
<div class="year"><span>2023</span><button class="download-btn" onclick="showAd('downloads/jee/chemistry/2023.pdf')">Download</button></div>
<div class="year"><span>2022</span><button class="download-btn" onclick="showAd('downloads/jee/chemistry/2022.pdf')">Download</button></div>
<div class="year"><span>2021</span><button class="download-btn" onclick="showAd('downloads/jee/chemistry/2021.pdf')">Download</button></div>
<div class="year"><span>2020</span><button class="download-btn" onclick="showAd('downloads/jee/chemistry/2020.pdf')">Download</button></div>
</div>

<!-- MATHS -->
<div class="subject">
<h2>Mathematics</h2>
<div class="year"><span>2024</span><button class="download-btn" onclick="showAd('downloads/jee/maths/2024.pdf')">Download</button></div>
<div class="year"><span>2023</span><button class="download-btn" onclick="showAd('downloads/jee/maths/2023.pdf')">Download</button></div>
<div class="year"><span>2022</span><button class="download-btn" onclick="showAd('downloads/jee/maths/2022.pdf')">Download</button></div>
<div class="year"><span>2021</span><button class="download-btn" onclick="showAd('downloads/jee/maths/2021.pdf')">Download</button></div>
<div class="year"><span>2020</span><button class="download-btn" onclick="showAd('downloads/jee/maths/2020.pdf')">Download</button></div>
</div>

</div>

<!-- AD MODAL -->
<div class="modal" id="adModal">
<div class="modal-content">
<h3>Advertisement</h3>

<div class="ad-box">
YOUR AD HERE
</div>

<p id="timerText">Please wait 5 seconds...</p>
<button id="finalDownload" disabled>Download</button>
</div>
</div>

<footer>
© 2025 JEE PYQ | Educational Purpose Only
</footer>

<script>
let fileLink="";
let timer;

function showAd(link){
    fileLink=link;
    document.getElementById("adModal").style.display="block";
    let time=5;
    document.getElementById("timerText").innerText="Please wait "+time+" seconds...";
    const btn=document.getElementById("finalDownload");
    btn.disabled=true;
    btn.style.cursor="not-allowed";

    timer=setInterval(()=>{
        time--;
        document.getElementById("timerText").innerText="Please wait "+time+" seconds...";
        if(time<=0){
            clearInterval(timer);
            document.getElementById("timerText").innerText="You can download now";
            btn.disabled=false;
            btn.style.cursor="pointer";
            btn.onclick=()=>{ window.location.href=fileLink; }
        }
    },1000);
}
</script>

</body>
</html>
