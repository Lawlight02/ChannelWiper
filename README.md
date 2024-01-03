# Channel Wiper
## About
- This code will delete your last 100 messages from the channel you are in
## How to use?
- Copy this snippet and paste into your console (to open use CTRL + SHIFT + I). If it doesn't open, do it in browser or figure it out
```js
!function(){let e=document.querySelector(".selected__3b4cb a")?document.querySelector(".selected__3b4cb a").href.split("/")[5]:document.querySelector(".selected_d94cf9 a").href.split("/")[5],r=(webpackChunkdiscord_app.push([[""],{},e=>{for(let r in m=[],e.c)m.push(e.c[r])}]),m).find(e=>e?.exports?.default?.getToken!==void 0).exports.default.getToken();fetch("https://discord.com/api/v9/channels/"+e+"/messages?limit=100",{headers:{accept:"*/*","accept-language":"en-US,en;q=0.9,en;q=0.8",authorization:r},referrer:"https://discord.com/",referrerPolicy:"strict-origin-when-cross-origin",body:null,method:"GET",mode:"cors",credentials:"include"}).then(t=>{t.json().then(t=>{for(let c in t=t.filter(e=>e.author.id==document.querySelector(".container_ca50b9 .avatarStack__6604a img").src.split("/")[4]))setTimeout(()=>{fetch("https://discord.com/api/v9/channels/"+e+"/messages/"+t[c].id,{headers:{accept:"*/*","accept-language":"en-US,en;q=0.9,en;q=0.8",authorization:r},referrer:"https://discord.com/",referrerPolicy:"strict-origin-when-cross-origin",body:null,method:"DELETE",mode:"cors",credentials:"include"})},2e3*c+1e3*Math.random())})})}();
```
