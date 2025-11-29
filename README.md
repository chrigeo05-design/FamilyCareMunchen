:root{
  --bg: #fff8f2;
  --warm: #df6b58;
  --accent: #a74b3f;
  --text: #3b2b2a;
  --muted: #7a6b68;
  --card: #fff;
  --radius: 12px;
  --maxw: 980px;
  --gap: 20px;
}
*{box-sizing:border-box}
body{font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; background:var(--bg); color:var(--text); margin:0; line-height:1.45}
.container{max-width:var(--maxw); margin:30px auto; padding:24px;}
.header{display:flex; align-items:center; gap:16px}
.logo{height:72px; width:72px; border-radius:14px; overflow:hidden; flex:0 0 72px; background:#fff}
.brand{display:flex; flex-direction:column}
.brand h1{margin:0; font-size:20px; color:var(--accent)}
.brand p{margin:0; color:var(--muted); font-size:14px}

.nav{margin-top:18px; display:flex; gap:12px; flex-wrap:wrap}
.nav a{background:transparent; padding:8px 12px; border-radius:999px; text-decoration:none; color:var(--accent); font-weight:600; font-size:14px}

.hero{display:grid; grid-template-columns:1fr 360px; gap:24px; align-items:center; margin-top:24px}
.hero .card{background:var(--card); padding:24px; border-radius:var(--radius); box-shadow:0 6px 18px rgba(0,0,0,0.04)}
.hero h2{margin:0 0 12px 0; color:var(--accent); font-size:28px}
.hero p{margin:0 0 18px 0; color:var(--muted)}

.service-grid{display:grid; grid-template-columns:repeat(3,1fr); gap:16px; margin-top:24px}
.service{background:var(--card); padding:18px; border-radius:12px; text-align:center}
.service h3{margin:8px 0; color:var(--accent)}

.pricing{display:flex; gap:12px; margin-top:18px; align-items:stretch}
.price{flex:1; background:linear-gradient(180deg, #fff, #fff); padding:18px; border-radius:12px; border:1px solid rgba(167,75,63,0.08)}

footer{margin-top:32px; padding:18px; text-align:center; color:var(--muted)}

.cta{display:flex; gap:12px; align-items:center}
.btn{background:var(--warm); color:white; padding:10px 14px; border-radius:10px; text-decoration:none; font-weight:700}
.btn.secondary{background:transparent; border:2px solid var(--warm); color:var(--warm)}

.card-list{display:grid; gap:12px}
.note{font-size:13px; color:var(--muted)}

/* responsive */
@media (max-width:900px){
  .hero{grid-template-columns:1fr; padding-bottom:8px}
  .service-grid{grid-template-columns:repeat(2,1fr)}
}
@media (max-width:520px){
  .service-grid{grid-template-columns:1fr}
  .nav{justify-content:center}
  .header{flex-direction:column; align-items:flex-start}
}
