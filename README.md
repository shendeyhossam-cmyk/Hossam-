# Hossam-
المتحف 
/* 💓 نبضة حب عند الضغط في أي مكان */
document.addEventListener("click", function(e){
let heart=document.createElement("div");
heart.innerHTML="💖";
heart.style.position="fixed";
heart.style.left=e.clientX+"px";
heart.style.top=e.clientY+"px";
heart.style.fontSize="20px";
heart.style.animation="float 3s linear forwards";
document.body.appendChild(heart);
setTimeout(()=>heart.remove(),3000);

document.body.style.transform="scale(1.01)";
setTimeout(()=>document.body.style.transform="scale(1)",150);
});

/* 💌 رسالة عائمة كل 10 ثواني */
setInterval(function(){
let msg=document.createElement("div");
msg.innerHTML="بحبك يا أميرة ❤️";
msg.style.position="fixed";
msg.style.left=Math.random()*window.innerWidth+"px";
msg.style.top=Math.random()*window.innerHeight+"px";
msg.style.color="gold";
msg.style.fontSize="18px";
msg.style.animation="float 4s linear forwards";
document.body.appendChild(msg);
setTimeout(()=>msg.remove(),4000);
},10000);

/* 🌙 رسالة الساعة 12 */
function checkMidnight(){
let now=new Date();
if(now.getHours()===0 && now.getMinutes()===0){
alert("الساعة بقت 12 ❤️\nكل يوم بيعدي بحبك أكتر يا أميرة 👑");
}
}
setInterval(checkMidnight,60000);
