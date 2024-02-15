# Channel Wiper
## About
- This code will delete all your messages from the channel you are in
## How to use?
- Copy this snippet and paste into your console (to open use CTRL + SHIFT + I). If it doesn't open, do it in browser or figure it out
```js
(async()=>{let e=document.querySelector(".selected__3b4cb a")?document.querySelector(".selected__3b4cb a").href.split("/")[5]:document.querySelector(".selected_d94cf9 a").href.split("/")[5],r=(webpackChunkdiscord_app.push([[""],{},e=>{for(let r in m=[],e.c)m.push(e.c[r])}]),m).find(e=>e?.exports?.default?.getToken!==void 0).exports.default.getToken(),t=[],c=null;for(;;){let o=await fetch(`https://discord.com/api/v9/channels/${e}/messages?limit=100${c?`&before=${c}`:""}`,{headers:{accept:"*/*","accept-language":"en-US,en;q=0.9,en;q=0.8",authorization:r},referrer:"https://discord.com/",referrerPolicy:"strict-origin-when-cross-origin",body:null,method:"GET",mode:"cors",credentials:"include"}),i=await o.json();if(0===i.length)break;t=t.concat(i),c=i[i.length-1].id}for(let a in t=t.filter(e=>e.author.id==document.querySelector(".container_ca50b9 .avatarStack__6604a img").src.split("/")[4]))setTimeout(()=>{fetch("https://discord.com/api/v9/channels/"+e+"/messages/"+t[a].id,{headers:{accept:"*/*","accept-language":"en-US,en;q=0.9,en;q=0.8",authorization:r},referrer:"https://discord.com/",referrerPolicy:"strict-origin-when-cross-origin",body:null,method:"DELETE",mode:"cors",credentials:"include"})},2e3*a+1e3*Math.random())})();
```
## Disclaimer
- This is prohibited by Discord, using it may get you banned. Use at your own risk
