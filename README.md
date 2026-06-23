<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Online Coaching Intake — Ziad Elfeky</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;1,400&family=DM+Serif+Display:ital@0;1&display=swap');
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0;}
:root{
  --ink:#111111;--mid:#555555;--soft:#999999;--rule:#e2dfd9;
  --bg:#f6f4f0;--white:#ffffff;--gold:#b8966a;--gold-dark:#9a7c52;
  --gold-faint:#faf6f0;--red:#c0392b;--red-bg:#fdf0f0;--red-border:#f5c6c6;
  --green:#2d6a4f;--green-bg:#f0faf5;
}
body{font-family:'DM Sans',sans-serif;background:var(--bg);color:var(--ink);line-height:1.6;min-height:100vh;}
input,select,textarea,button{font-family:'DM Sans',sans-serif;touch-action:manipulation;}
::-webkit-scrollbar{width:5px;}
::-webkit-scrollbar-thumb{background:var(--rule);border-radius:3px;}
.hdr{background:var(--ink);color:#fff;padding:36px 24px 30px;}
.hdr-eye{font-size:11px;font-weight:600;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);}
.hdr h1{font-family:'DM Serif Display',serif;font-size:clamp(26px,5vw,40px);font-weight:400;line-height:1.1;margin-top:6px;}
.hdr-sub{font-size:13px;color:rgba(255,255,255,.35);font-style:italic;margin-top:5px;}
.hdr-desc{font-size:13px;color:rgba(255,255,255,.42);margin-top:14px;max-width:520px;line-height:1.7;border-top:1px solid rgba(255,255,255,.08);padding-top:14px;}
.nav{background:var(--white);border-bottom:1px solid var(--rule);padding:0 24px;}
.nav-inner{max-width:740px;margin:0 auto;display:flex;}
.nav-btn{background:none;border:none;border-bottom:2px solid transparent;cursor:pointer;padding:13px 0;margin-right:28px;font-size:13px;font-weight:500;color:var(--soft);transition:all .14s;-webkit-tap-highlight-color:transparent;}
.nav-btn.active{color:var(--ink);border-bottom-color:var(--gold);}
.wrap{max-width:740px;margin:0 auto;padding:44px 20px 80px;}
.sec{margin-bottom:48px;}
.sec-hdr{display:flex;align-items:baseline;gap:12px;border-bottom:1px solid var(--rule);padding-bottom:11px;margin-bottom:22px;}
.sec-num{font-size:11px;font-weight:700;letter-spacing:.14em;color:var(--gold);text-transform:uppercase;}
.sec-title{font-family:'DM Serif Display',serif;font-size:20px;font-weight:400;}
.field{display:flex;flex-direction:column;gap:6px;margin-bottom:20px;}
.row{display:grid;grid-template-columns:1fr 1fr;gap:16px;}
.lbl{font-size:13px;font-weight:600;color:var(--ink);}
.hint{font-weight:400;color:var(--soft);font-size:12px;margin-left:5px;}
.req{color:var(--gold);margin-left:2px;}
.err-msg{font-size:11px;color:var(--red);margin-top:2px;min-height:14px;}
input[type=text],input[type=number],input[type=date],input[type=password],select,textarea{width:100%;background:var(--white);border:1px solid var(--rule);border-radius:7px;padding:11px 14px;font-size:14px;color:var(--ink);outline:none;transition:border-color .15s;-webkit-appearance:none;}
input:focus,select:focus,textarea:focus{border-color:var(--gold);}
input.err,select.err,textarea.err{border-color:var(--red);}
textarea{resize:vertical;min-height:88px;}
select{background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='7' viewBox='0 0 12 7'%3E%3Cpath d='M1 1l5 5 5-5' stroke='%23999' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");background-repeat:no-repeat;background-position:right 13px center;background-color:var(--white);padding-right:34px;}
.pills{display:flex;flex-wrap:wrap;gap:8px;margin-top:2px;}
.pill{display:inline-flex;align-items:center;gap:7px;background:var(--white);border:1px solid var(--rule);border-radius:20px;padding:7px 15px;font-size:13px;cursor:pointer;transition:all .13s;-webkit-tap-highlight-color:transparent;user-select:none;}
.pill.on{background:var(--gold-faint);border-color:var(--gold);color:var(--gold-dark);font-weight:600;}
.pill-dot{width:8px;height:8px;border-radius:50%;background:var(--rule);flex-shrink:0;transition:background .13s;}
.pill.on .pill-dot{background:var(--gold);}
.scale{display:flex;gap:7px;flex-wrap:wrap;}
.scale-btn{width:40px;height:40px;border-radius:7px;border:1px solid var(--rule);background:var(--white);font-size:13px;font-weight:500;cursor:pointer;transition:all .13s;-webkit-tap-highlight-color:transparent;}
.scale-btn.on{background:var(--ink);color:#fff;border-color:var(--ink);}
.scale-labels{display:flex;justify-content:space-between;font-size:11px;color:var(--soft);margin-top:5px;}
.note{background:var(--gold-faint);border-left:3px solid var(--gold);border-radius:0 7px 7px 0;padding:13px 16px;font-size:13px;color:var(--mid);line-height:1.7;margin-bottom:16px;}
.note strong{color:var(--ink);}
.photo-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin:14px 0;}
.photo-card{border:1.5px dashed var(--rule);border-radius:9px;background:var(--white);padding:18px 10px;display:flex;flex-direction:column;align-items:center;gap:8px;text-align:center;}
.photo-icon{width:36px;height:36px;border-radius:50%;background:var(--gold-faint);display:flex;align-items:center;justify-content:center;}
.photo-lbl{font-size:12px;font-weight:700;color:var(--ink);}
.photo-note{font-size:11px;color:var(--soft);line-height:1.4;}
.cloth-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin:12px 0 18px;}
.cloth-card{background:var(--white);border:1px solid var(--rule);border-radius:8px;padding:13px 15px;}
.cloth-tag{font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--gold);margin-bottom:5px;}
.cloth-card p{font-size:12.5px;color:var(--mid);line-height:1.6;}
.submit-wrap{display:flex;flex-direction:column;align-items:center;gap:12px;margin-top:10px;}
.btn-primary{background:var(--ink);color:#fff;border:none;border-radius:8px;padding:15px 52px;font-size:14px;font-weight:600;letter-spacing:.05em;cursor:pointer;-webkit-tap-highlight-color:transparent;}
.btn-primary:disabled{background:var(--soft);}
.submit-note{font-size:12px;color:var(--soft);}
.err-banner{font-size:13px;color:var(--red);background:var(--red-bg);border:1px solid var(--red-border);border-radius:7px;padding:10px 16px;text-align:center;width:100%;}
.success-wrap{max-width:500px;margin:60px auto;padding:0 24px;text-align:center;display:flex;flex-direction:column;align-items:center;gap:22px;}
.success-icon{width:64px;height:64px;border-radius:50%;background:var(--green-bg);border:2px solid var(--green);display:flex;align-items:center;justify-content:center;}
.success-title{font-family:'DM Serif Display',serif;font-size:28px;font-weight:400;}
.success-body{font-size:14px;color:var(--mid);line-height:1.7;}
.next-steps{background:var(--gold-faint);border:1px solid var(--rule);border-radius:10px;padding:18px 20px;width:100%;text-align:left;}
.next-tag{font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--gold);margin-bottom:10px;}
.next-item{display:flex;gap:10px;align-items:flex-start;font-size:13px;color:var(--mid);margin-bottom:8px;}
.next-num{color:var(--gold);font-weight:700;flex-shrink:0;}
.pin-wrap{max-width:360px;margin:60px auto;padding:0 24px;display:flex;flex-direction:column;gap:18px;align-items:center;}
.pin-title{font-family:'DM Serif Display',serif;font-size:24px;text-align:center;}
.pin-sub{font-size:13px;color:var(--mid);text-align:center;}
.dash-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px;flex-wrap:wrap;gap:12px;}
.dash-title{font-family:'DM Serif Display',serif;font-size:24px;}
.dash-count{font-size:13px;color:var(--soft);margin-top:3px;}
.btn-sm{background:none;border:1px solid var(--rule);border-radius:6px;padding:8px 14px;font-size:12px;color:var(--mid);cursor:pointer;-webkit-tap-highlight-color:transparent;}
.btn-danger{border-color:var(--red-border);color:var(--red);}
.empty-state{text-align:center;padding:60px 0;color:var(--soft);font-size:14px;}
.loading{text-align:center;padding:40px;color:var(--soft);font-size:14px;}
.client-card{background:var(--white);border:1px solid var(--rule);border-radius:10px;padding:16px 20px;cursor:pointer;display:flex;align-items:center;gap:15px;margin-bottom:10px;-webkit-tap-highlight-color:transparent;}
.avatar{width:40px;height:40px;border-radius:50%;background:var(--gold-faint);border:1px solid var(--rule);display:flex;align-items:center;justify-content:center;flex-shrink:0;font-size:16px;font-weight:700;color:var(--gold);}
.client-name{font-weight:600;font-size:14px;}
.client-meta{font-size:12px;color:var(--soft);margin-top:2px;}
.client-date{font-size:11px;color:var(--soft);flex-shrink:0;text-align:right;}
.back-row{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px;flex-wrap:wrap;gap:10px;}
.detail-name{font-family:'DM Serif Display',serif;font-size:26px;margin-bottom:4px;}
.detail-meta{font-size:12px;color:var(--soft);margin-bottom:24px;}
.detail-sec-title{font-size:11px;font-weight:700;letter-spacing:.14em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;margin-top:28px;}
.detail-row{display:flex;gap:12px;padding:9px 0;border-bottom:1px solid var(--rule);flex-wrap:wrap;}
.detail-key{font-size:12px;font-weight:600;color:var(--soft);min-width:160px;flex-shrink:0;}
.detail-val{font-size:13px;color:var(--ink);flex:1;}
.footer{background:var(--ink);color:rgba(255,255,255,.28);text-align:center;padding:18px;font-size:12px;letter-spacing:.04em;}
.footer span{color:var(--gold);font-weight:500;}
@media(max-width:580px){
  .row{grid-template-columns:1fr;}
  .photo-grid{grid-template-columns:1fr 1fr;}
  .cloth-grid{grid-template-columns:1fr;}
  .scale-btn{width:34px;height:34px;font-size:12px;}
}
</style>
</head>
<body>

<div class="hdr" id="hdr">
  <div class="hdr-eye">Online Coaching · Ziad Elfeky</div>
  <h1 id="hdr-title">Client Intake Form</h1>
  <div class="hdr-sub">Fix the root cause. Build the body. Perform for life.</div>
  <div class="hdr-desc" id="hdr-desc">Fill this out fully and honestly. The more accurate your answers, the more precise your program will be.</div>
</div>

<div class="nav">
  <div class="nav-inner">
    <button class="nav-btn active" id="nav-form" onclick="showView('form')">Intake Form</button>
    <button class="nav-btn" id="nav-dash" onclick="showView('dashboard')">Coach Dashboard</button>
  </div>
</div>

<!-- FORM -->
<div id="view-form">
<div class="wrap">

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">01</span><span class="sec-title">Basic Info</span></div>
    <div class="row">
      <div class="field">
        <label class="lbl">Full Name <span class="req">*</span></label>
        <input type="text" id="f-name" placeholder="Your full name">
        <span class="err-msg" id="e-name"></span>
      </div>
      <div class="field">
        <label class="lbl">Date of Birth</label>
        <input type="date" id="f-dob">
      </div>
    </div>
    <div class="row">
      <div class="field">
        <label class="lbl">Gender <span class="req">*</span></label>
        <select id="f-gender" onchange="handleGender()">
          <option value="">Select</option>
          <option>Male</option>
          <option>Female</option>
          <option>Prefer not to say</option>
        </select>
        <span class="err-msg" id="e-gender"></span>
      </div>
      <div class="field">
        <label class="lbl">Occupation <span class="hint">— affects energy</span></label>
        <input type="text" id="f-occupation" placeholder="e.g. Student, engineer…">
      </div>
    </div>
    <div class="field">
      <label class="lbl">Country / City</label>
      <input type="text" id="f-location" placeholder="e.g. Cairo, Egypt">
    </div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">02</span><span class="sec-title">Current Measurements</span></div>
    <div class="row">
      <div class="field">
        <label class="lbl">Height <span class="hint">— cm</span></label>
        <input type="number" id="f-height" placeholder="e.g. 178">
      </div>
      <div class="field">
        <label class="lbl">Weight <span class="hint">— kg</span></label>
        <input type="number" id="f-weight" placeholder="e.g. 82">
      </div>
    </div>
    <div class="field">
      <label class="lbl">Waist <span class="hint">— cm, at navel (optional)</span></label>
      <input type="number" id="f-waist" placeholder="e.g. 88">
    </div>
    <div class="note">Measure first thing in the morning before eating. Stand relaxed, tape at navel — don't suck in.</div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">03</span><span class="sec-title">Training Background</span></div>
    <div class="field">
      <label class="lbl">Total training experience <span class="req">*</span></label>
      <div class="pills" id="p-exp"></div>
      <span class="err-msg" id="e-exp"></span>
    </div>
    <div class="field">
      <label class="lbl">Length of break <span class="req">*</span></label>
      <div class="pills" id="p-break"></div>
      <span class="err-msg" id="e-break"></span>
    </div>
    <div class="field">
      <label class="lbl">Activity during break</label>
      <textarea id="f-break-activity" placeholder="e.g. Mostly sedentary, some walking…"></textarea>
    </div>
    <div class="field">
      <label class="lbl">Training type before break <span class="hint">— select all that apply</span></label>
      <div class="pills" id="p-train-type"></div>
    </div>
    <div class="field">
      <label class="lbl">Equipment available now <span class="req">*</span></label>
      <div class="pills" id="p-equipment"></div>
      <span class="err-msg" id="e-equipment"></span>
    </div>
    <div class="row">
      <div class="field">
        <label class="lbl">Days per week <span class="req">*</span></label>
        <select id="f-days">
          <option value="">Select</option>
          <option>2 days</option><option>3 days</option><option>4 days</option>
          <option>5 days</option><option>6 days</option>
        </select>
        <span class="err-msg" id="e-days"></span>
      </div>
      <div class="field">
        <label class="lbl">Session duration <span class="req">*</span></label>
        <select id="f-duration">
          <option value="">Select</option>
          <option>30–40 min</option><option>45–60 min</option>
          <option>60–75 min</option><option>75–90 min</option>
        </select>
        <span class="err-msg" id="e-duration"></span>
      </div>
    </div>
    <div class="field">
      <label class="lbl">Preferred training time</label>
      <div class="pills" id="p-train-time"></div>
    </div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">04</span><span class="sec-title">Goals & Priorities</span></div>
    <div class="field">
      <label class="lbl">Primary goal <span class="req">*</span></label>
      <div class="pills" id="p-goal"></div>
      <span class="err-msg" id="e-goal"></span>
    </div>
    <div class="field">
      <label class="lbl">Describe your physique goal</label>
      <textarea id="f-physique-goal" placeholder="e.g. Lose 6–8 kg of fat, maintain muscle…"></textarea>
    </div>
    <div class="field">
      <label class="lbl">Timeline</label>
      <div class="pills" id="p-timeline"></div>
    </div>
    <div class="field">
      <label class="lbl">Specific areas to work on</label>
      <input type="text" id="f-focus" placeholder="e.g. Lower back, posture, core…">
    </div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">05</span><span class="sec-title">Health & Medical</span></div>
    <div class="field">
      <label class="lbl">Pain, injuries, or conditions <span class="req">*</span></label>
      <textarea id="f-pain" placeholder="e.g. Lower back pain, knee surgery 2022 — or write 'None'"></textarea>
      <span class="err-msg" id="e-pain"></span>
    </div>
    <div class="field">
      <label class="lbl">Movements to avoid</label>
      <input type="text" id="f-avoid" placeholder="e.g. No running, no overhead pressing…">
    </div>
    <div class="field">
      <label class="lbl">On medication affecting training?</label>
      <div class="pills" id="p-meds"></div>
    </div>
    <div class="field" id="f-cycle-wrap" style="display:none">
      <label class="lbl">Menstrual cycle status</label>
      <select id="f-cycle">
        <option value="">Select</option>
        <option>Regular</option><option>Irregular</option>
        <option>On hormonal contraception</option>
        <option>PCOS or hormonal condition</option>
        <option>Prefer not to say</option>
      </select>
    </div>
    <div class="field">
      <label class="lbl">Additional health context</label>
      <textarea id="f-health-notes" placeholder="Medication details, conditions, anything relevant…"></textarea>
    </div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">06</span><span class="sec-title">Lifestyle & Recovery</span></div>
    <div class="field">
      <label class="lbl">Average sleep per night</label>
      <div class="pills" id="p-sleep"></div>
    </div>
    <div class="field">
      <label class="lbl">Daily stress level</label>
      <div class="scale" id="scale-stress"></div>
      <div class="scale-labels"><span>Completely calm</span><span>Extremely stressed</span></div>
    </div>
    <div class="field">
      <label class="lbl">Current approach to food</label>
      <div class="pills" id="p-nutrition"></div>
    </div>
    <div class="row">
      <div class="field">
        <label class="lbl">Daily water intake</label>
        <select id="f-water">
          <option value="">Select</option>
          <option>Less than 1L</option><option>1–1.5L</option>
          <option>1.5–2L</option><option>2L+</option>
        </select>
      </div>
      <div class="field">
        <label class="lbl">Daily steps</label>
        <select id="f-steps">
          <option value="">Select</option>
          <option>Less than 3,000</option><option>3,000–6,000</option>
          <option>6,000–10,000</option><option>10,000+</option>
          <option>I don't track</option>
        </select>
      </div>
    </div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">07</span><span class="sec-title">Progress Photos</span></div>
    <div class="note">
      <strong>Send photos to WhatsApp after submitting.</strong> First thing in the morning, before eating. Same spot and light every time. Stand relaxed, arms slightly away from sides. No posing.<br><br>
      <strong>Males:</strong> Shorts only, no shirt. &nbsp;&nbsp;<strong>Females:</strong> Sports bra + shorts, or fitted top + leggings.
    </div>
    <div class="cloth-grid">
      <div class="cloth-card"><div class="cloth-tag">Males</div><p>Shorts only, no shirt. Shows chest, arms, abdomen, legs clearly.</p></div>
      <div class="cloth-card"><div class="cloth-tag">Females</div><p>Sports bra + shorts, or fitted top + leggings. No baggy clothing.</p></div>
    </div>
    <div class="photo-grid">
      <div class="photo-card">
        <div class="photo-icon"><svg width="18" height="18" fill="none" stroke="#b8966a" stroke-width="1.5" viewBox="0 0 24 24"><circle cx="12" cy="8" r="4"/><path d="M12 14c-5 0-8 2-8 4v2h16v-2c0-2-3-4-8-4z"/></svg></div>
        <div class="photo-lbl">Front</div><div class="photo-note">Facing camera, arms slightly out</div>
      </div>
      <div class="photo-card">
        <div class="photo-icon"><svg width="18" height="18" fill="none" stroke="#b8966a" stroke-width="1.5" viewBox="0 0 24 24"><circle cx="12" cy="8" r="4"/><path d="M12 14c-5 0-8 2-8 4v2h16v-2c0-2-3-4-8-4z"/></svg></div>
        <div class="photo-lbl">Back</div><div class="photo-note">Facing away, relaxed</div>
      </div>
      <div class="photo-card">
        <div class="photo-icon"><svg width="18" height="18" fill="none" stroke="#b8966a" stroke-width="1.5" viewBox="0 0 24 24"><circle cx="12" cy="8" r="4"/><path d="M12 14c-5 0-8 2-8 4v2h16v-2c0-2-3-4-8-4z"/></svg></div>
        <div class="photo-lbl">Side — Right</div><div class="photo-note">Profile, arms down</div>
      </div>
    </div>
    <div class="field" style="margin-top:16px">
      <label class="lbl">How do you feel about your current physique?</label>
      <textarea id="f-physique-self" placeholder="e.g. Lost muscle during the break, belly more prominent…"></textarea>
    </div>
  </div>

  <div class="sec">
    <div class="sec-hdr"><span class="sec-num">08</span><span class="sec-title">Coaching Preferences</span></div>
    <div class="field">
      <label class="lbl">Online coaching experience</label>
      <div class="pills" id="p-prev-coach"></div>
    </div>
    <div class="field">
      <label class="lbl">What worked / didn't in the past?</label>
      <textarea id="f-what-worked" placeholder="e.g. I respond well to explanations. I struggle with strict meal plans…"></textarea>
    </div>
    <div class="field">
      <label class="lbl">Preferred check-in method</label>
      <div class="pills" id="p-checkin"></div>
    </div>
    <div class="field">
      <label class="lbl">Anything else before we start?</label>
      <textarea id="f-other" placeholder="Upcoming travel, concerns, expectations…"></textarea>
    </div>
  </div>

  <div class="submit-wrap">
    <div id="submit-err" class="err-banner" style="display:none">Please fill in all required fields.</div>
    <button class="btn-primary" id="submit-btn" onclick="handleSubmit()">Submit Intake Form</button>
    <span class="submit-note">Then send your 3 progress photos via WhatsApp</span>
  </div>
</div>
</div>

<!-- SUCCESS -->
<div id="view-success" style="display:none">
  <div class="success-wrap">
    <div class="success-icon">
      <svg width="28" height="28" fill="none" stroke="#2d6a4f" stroke-width="2.5" viewBox="0 0 24 24"><path d="M5 13l4 4L19 7" stroke-linecap="round" stroke-linejoin="round"/></svg>
    </div>
    <div class="success-title" id="success-title">You're all set.</div>
    <div class="success-body">Your intake has been received. Send your 3 progress photos via WhatsApp and your program will be ready within 48 hours.</div>
    <div class="next-steps">
      <div class="next-tag">Next steps</div>
      <div class="next-item"><span class="next-num">1.</span>Send front, back & right-side photos via WhatsApp</div>
      <div class="next-item"><span class="next-num">2.</span>Program ready within 48 hours</div>
      <div class="next-item"><span class="next-num">3.</span>Let's go</div>
    </div>
    <button onclick="resetForm()" style="font-size:12px;color:var(--soft);background:none;border:none;cursor:pointer;text-decoration:underline;">Submit another response</button>
  </div>
</div>

<!-- DASHBOARD -->
<div id="view-dashboard" style="display:none">

  <!-- PIN -->
  <div id="dash-pin" style="display:none">
    <div class="pin-wrap">
      <div class="pin-title">Coach Access</div>
      <div class="pin-sub">Enter your PIN to view submitted intakes.</div>
      <div style="width:100%;display:flex;flex-direction:column;gap:10px">
        <input type="password" id="pin-input" placeholder="PIN" style="text-align:center;font-size:22px;letter-spacing:.3em">
        <div id="pin-err" style="font-size:12px;color:var(--red);text-align:center;display:none">Incorrect PIN</div>
        <button class="btn-primary" onclick="checkPin()">Enter</button>
      </div>
      <button onclick="showView('form')" style="font-size:12px;color:var(--soft);background:none;border:none;cursor:pointer">Back to form</button>
    </div>
  </div>

  <!-- LIST -->
  <div id="dash-list" style="display:none">
    <div class="wrap">
      <div class="dash-header">
        <div>
          <div class="dash-title">Client Submissions</div>
          <div class="dash-count" id="dash-count">Loading…</div>
        </div>
        <div style="display:flex;gap:8px;flex-wrap:wrap">
          <button class="btn-sm" onclick="exportCSV()">Export CSV</button>
          <button class="btn-sm" onclick="loadSubmissions()">Refresh</button>
          <button class="btn-sm" onclick="dashLogout()">Lock</button>
        </div>
      </div>
      <div id="clients-list"></div>
    </div>
  </div>

  <!-- DETAIL -->
  <div id="dash-detail" style="display:none">
    <div class="wrap">
      <div class="back-row">
        <button class="btn-sm" onclick="showDashList()">← All clients</button>
        <button class="btn-sm btn-danger" id="detail-delete-btn">Delete record</button>
      </div>
      <div id="detail-content"></div>
    </div>
  </div>

</div>

<div class="footer"><span>Ziad Elfeky</span> · Online Coaching</div>

<script>
var SUPABASE_URL = "https://gndbfxwjcumkftbultkt.supabase.co";
var SUPABASE_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImduZGJmeHdqY3Vta2Z0YnVsdGt0Iiwicm9sZSI6ImFub24iLCJpYXQiOjE3ODIwMzc5NTAsImV4cCI6MjA5NzYxMzk1MH0.LLk6yk3kgyH5INPE60hU1tyAaKNCWF6Sdkoywg3kRjo";
var COACH_PIN = "1991";
var TABLE = "intake_submissions";
var pillState = {};
var stressVal = null;
var dashUnlocked = false;
var allSubmissions = [];

function initPills(id, opts, multi) {
  pillState[id] = multi ? [] : '';
  var el = document.getElementById(id);
  if (!el) return;
  el.innerHTML = '';
  opts.forEach(function(opt) {
    var btn = document.createElement('button');
    btn.type = 'button';
    btn.className = 'pill';
    btn.innerHTML = '<span class="pill-dot"></span>' + opt;
    btn.addEventListener('click', function() { togglePill(id, opt, multi, btn); });
    el.appendChild(btn);
  });
}

function togglePill(id, val, multi, btn) {
  if (multi) {
    var arr = pillState[id];
    var idx = arr.indexOf(val);
    if (idx > -1) { arr.splice(idx, 1); btn.classList.remove('on'); }
    else { arr.push(val); btn.classList.add('on'); }
  } else {
    var same = pillState[id] === val;
    pillState[id] = same ? '' : val;
    var el = document.getElementById(id);
    if (el) el.querySelectorAll('.pill').forEach(function(b) { b.classList.remove('on'); });
    if (!same) btn.classList.add('on');
  }
}

function getPill(id) { return pillState[id]; }

function initScale() {
  var el = document.getElementById('scale-stress');
  if (!el) return;
  el.innerHTML = '';
  for (var i = 1; i <= 10; i++) {
    (function(n) {
      var btn = document.createElement('button');
      btn.type = 'button';
      btn.className = 'scale-btn';
      btn.textContent = n;
      btn.addEventListener('click', function() {
        stressVal = n;
        document.querySelectorAll('.scale-btn').forEach(function(b) { b.classList.remove('on'); });
        btn.classList.add('on');
      });
      el.appendChild(btn);
    })(i);
  }
}

function initAllPills() {
  initPills('p-exp', ['Less than 1 year','1–2 years','2–4 years','4+ years'], false);
  initPills('p-break', ['Less than 4 weeks','1–2 months','2–4 months','4+ months'], false);
  initPills('p-train-type', ['Strength / Weights','HIIT','Cardio','Yoga / Pilates','Sport','Calisthenics','CrossFit','Other'], true);
  initPills('p-equipment', ['Full gym','Home gym (weights)','Dumbbells only','Resistance bands','Bodyweight only'], true);
  initPills('p-train-time', ['Morning','Midday','Evening','Varies'], false);
  initPills('p-goal', ['Fat loss','Muscle gain','Recomposition','Strength','Fitness & endurance','Return to baseline','Rehab / pain management'], false);
  initPills('p-timeline', ['4–6 weeks','2–3 months','3–6 months','Long-term, no rush'], false);
  initPills('p-meds', ['No','Yes — will add details below','Prefer not to say'], false);
  initPills('p-sleep', ['Less than 5h','5–6h','6–7h','7–8h','8h+'], false);
  initPills('p-nutrition', ['No tracking','Counting calories','Specific diet','Inconsistent / struggling'], false);
  initPills('p-prev-coach', ['First time','Yes, with someone else','Yes, with you before'], false);
  initPills('p-checkin', ['WhatsApp weekly','Video call monthly','App only','Message as needed'], false);
  initScale();
}

function handleGender() {
  var g = document.getElementById('f-gender').value;
  document.getElementById('f-cycle-wrap').style.display = g === 'Female' ? 'flex' : 'none';
}

function showView(v) {
  document.getElementById('view-form').style.display = 'none';
  document.getElementById('view-success').style.display = 'none';
  document.getElementById('view-dashboard').style.display = 'none';
  document.getElementById('nav-form').classList.remove('active');
  document.getElementById('nav-dash').classList.remove('active');
  document.getElementById('view-' + v).style.display = 'block';
  if (v === 'dashboard') {
    document.getElementById('nav-dash').classList.add('active');
    document.getElementById('hdr-title').textContent = 'Coach Dashboard';
    document.getElementById('hdr-desc').style.display = 'none';
    if (!dashUnlocked) {
      document.getElementById('dash-pin').style.display = 'block';
      document.getElementById('dash-list').style.display = 'none';
      document.getElementById('dash-detail').style.display = 'none';
    } else {
      showDashList();
      loadSubmissions();
    }
  } else {
    document.getElementById('nav-form').classList.add('active');
    document.getElementById('hdr-title').textContent = 'Client Intake Form';
    document.getElementById('hdr-desc').style.display = 'block';
  }
}

function checkPin() {
  var val = document.getElementById('pin-input').value;
  if (val === COACH_PIN) {
    dashUnlocked = true;
    document.getElementById('dash-pin').style.display = 'none';
    loadSubmissions();
  } else {
    var err = document.getElementById('pin-err');
    err.style.display = 'block';
    setTimeout(function() { err.style.display = 'none'; }, 2000);
  }
}

function dashLogout() {
  dashUnlocked = false;
  document.getElementById('pin-input').value = '';
  showView('form');
}

function showDashList() {
  document.getElementById('dash-pin').style.display = 'none';
  document.getElementById('dash-list').style.display = 'block';
  document.getElementById('dash-detail').style.display = 'none';
}

function loadSubmissions() {
  showDashList();
  document.getElementById('clients-list').innerHTML = '<div class="loading">Loading…</div>';
  fetch(SUPABASE_URL + '/rest/v1/' + TABLE + '?select=*&order=submitted_at.desc', {
    headers: { 'apikey': SUPABASE_KEY, 'Authorization': 'Bearer ' + SUPABASE_KEY }
  })
  .then(function(res) { return res.json(); })
  .then(function(data) {
    allSubmissions = data;
    renderList();
  })
  .catch(function(e) {
    document.getElementById('clients-list').innerHTML = '<div class="empty-state">Error: ' + e.message + '</div>';
  });
}

function renderList() {
  var count = allSubmissions.length;
  document.getElementById('dash-count').textContent = count + ' intake' + (count !== 1 ? 's' : '') + ' received';
  var list = document.getElementById('clients-list');
  if (count === 0) {
    list.innerHTML = '<div class="empty-state">No submissions yet. Share the form with your clients.</div>';
    return;
  }
  var html = '';
  allSubmissions.forEach(function(s, i) {
    var meta = [s.gender, s.location, s.primary_goal].filter(Boolean).join(' · ');
    html += '<div class="client-card" onclick="showDetail(' + i + ')">' +
      '<div class="avatar">' + (s.name || '?').charAt(0).toUpperCase() + '</div>' +
      '<div style="flex:1;min-width:0"><div class="client-name">' + esc(s.name || '—') + '</div>' +
      '<div class="client-meta">' + esc(meta) + '</div></div>' +
      '<div class="client-date">' + fmtDate(s.submitted_at) + '</div>' +
      '<svg width="16" height="16" fill="none" stroke="#999" stroke-width="1.5" viewBox="0 0 24 24"><path d="M9 18l6-6-6-6" stroke-linecap="round" stroke-linejoin="round"/></svg>' +
      '</div>';
  });
  list.innerHTML = html;
}

function showDetail(idx) {
  var s = allSubmissions[idx];
  document.getElementById('dash-list').style.display = 'none';
  document.getElementById('dash-detail').style.display = 'block';
  document.getElementById('detail-delete-btn').onclick = function() {
    if (confirm('Delete ' + s.name + '\'s record? Cannot be undone.')) { deleteRecord(s.id); }
  };
  var rows = [
    ['Name', s.name], ['Date of Birth', s.dob], ['Gender', s.gender],
    ['Occupation', s.occupation], ['Location', s.location],
    ['Height', s.height_cm ? s.height_cm + ' cm' : ''],
    ['Weight', s.weight_kg ? s.weight_kg + ' kg' : ''],
    ['Waist', s.waist_cm ? s.waist_cm + ' cm' : ''],
    ['Experience', s.exp_years], ['Break duration', s.break_duration],
    ['Break activity', s.break_activity], ['Training types', s.training_types],
    ['Equipment', s.equipment], ['Days/week', s.days_per_week],
    ['Session duration', s.session_duration], ['Train time', s.train_time],
    ['Primary goal', s.primary_goal], ['Physique goal', s.physique_goal],
    ['Timeline', s.timeline], ['Specific focus', s.specific_focus],
    ['Pain / injuries', s.pain_injuries], ['Avoid', s.avoid_movements],
    ['Medication', s.medications], ['Menstrual cycle', s.menstrual_cycle],
    ['Health notes', s.health_notes], ['Sleep', s.sleep],
    ['Stress level', s.stress_level ? s.stress_level + '/10' : ''],
    ['Nutrition', s.nutrition], ['Water', s.water], ['Steps', s.steps],
    ['Physique self-assessment', s.physique_self],
    ['Previous coaching', s.prev_coach], ['What worked', s.what_worked],
    ['Check-in preference', s.checkin], ['Other notes', s.other_notes]
  ];
  var html = '<div class="detail-name">' + esc(s.name || '—') + '</div>';
  html += '<div class="detail-meta">' + esc([s.gender, s.location].filter(Boolean).join(' · ')) + ' · Submitted ' + fmtDate(s.submitted_at, true) + '</div>';
  rows.forEach(function(r) {
    if (r[1] && String(r[1]).trim()) {
      html += '<div class="detail-row"><span class="detail-key">' + r[0] + '</span><span class="detail-val">' + esc(String(r[1])) + '</span></div>';
    }
  });
  document.getElementById('detail-content').innerHTML = html;
}

function deleteRecord(id) {
  fetch(SUPABASE_URL + '/rest/v1/' + TABLE + '?id=eq.' + id, {
    method: 'DELETE',
    headers: { 'apikey': SUPABASE_KEY, 'Authorization': 'Bearer ' + SUPABASE_KEY }
  })
  .then(function() { loadSubmissions(); })
  .catch(function(e) { alert('Error: ' + e.message); });
}

function validate() {
  var ok = true;
  var checks = [['f-name','e-name'],['f-gender','e-gender'],['f-days','e-days'],['f-duration','e-duration']];
  checks.forEach(function(c) {
    var el = document.getElementById(c[0]);
    var err = document.getElementById(c[1]);
    if (!el.value.trim()) { el.classList.add('err'); err.textContent = 'Required'; ok = false; }
    else { el.classList.remove('err'); err.textContent = ''; }
  });
  var pillChecks = [['p-exp','e-exp'],['p-break','e-break'],['p-equipment','e-equipment'],['p-goal','e-goal']];
  pillChecks.forEach(function(c) {
    var v = getPill(c[0]);
    var err = document.getElementById(c[1]);
    var empty = Array.isArray(v) ? v.length === 0 : !v;
    if (empty) { err.textContent = 'Required'; ok = false; }
    else { err.textContent = ''; }
  });
  var pain = document.getElementById('f-pain');
  var painErr = document.getElementById('e-pain');
  if (!pain.value.trim()) { pain.classList.add('err'); painErr.textContent = 'Required — write "None" if no issues'; ok = false; }
  else { pain.classList.remove('err'); painErr.textContent = ''; }
  return ok;
}

function collectData() {
  return {
    name: document.getElementById('f-name').value.trim(),
    dob: document.getElementById('f-dob').value,
    gender: document.getElementById('f-gender').value,
    occupation: document.getElementById('f-occupation').value.trim(),
    location: document.getElementById('f-location').value.trim(),
    height_cm: document.getElementById('f-height').value || null,
    weight_kg: document.getElementById('f-weight').value || null,
    waist_cm: document.getElementById('f-waist').value || null,
    exp_years: getPill('p-exp'),
    break_duration: getPill('p-break'),
    break_activity: document.getElementById('f-break-activity').value.trim(),
    training_types: getPill('p-train-type').join(', '),
    equipment: getPill('p-equipment').join(', '),
    days_per_week: document.getElementById('f-days').value,
    session_duration: document.getElementById('f-duration').value,
    train_time: getPill('p-train-time'),
    primary_goal: getPill('p-goal'),
    physique_goal: document.getElementById('f-physique-goal').value.trim(),
    timeline: getPill('p-timeline'),
    specific_focus: document.getElementById('f-focus').value.trim(),
    pain_injuries: document.getElementById('f-pain').value.trim(),
    avoid_movements: document.getElementById('f-avoid').value.trim(),
    medications: getPill('p-meds'),
    menstrual_cycle: document.getElementById('f-cycle').value,
    health_notes: document.getElementById('f-health-notes').value.trim(),
    sleep: getPill('p-sleep'),
    stress_level: stressVal,
    nutrition: getPill('p-nutrition'),
    water: document.getElementById('f-water').value,
    steps: document.getElementById('f-steps').value,
    physique_self: document.getElementById('f-physique-self').value.trim(),
    prev_coach: getPill('p-prev-coach'),
    what_worked: document.getElementById('f-what-worked').value.trim(),
    checkin: getPill('p-checkin'),
    other_notes: document.getElementById('f-other').value.trim(),
    submitted_at: new Date().toISOString()
  };
}

function handleSubmit() {
  if (!validate()) {
    document.getElementById('submit-err').style.display = 'block';
    return;
  }
  document.getElementById('submit-err').style.display = 'none';
  var btn = document.getElementById('submit-btn');
  btn.disabled = true;
  btn.textContent = 'Submitting…';
  var data = collectData();
  fetch(SUPABASE_URL + '/rest/v1/' + TABLE, {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json',
      'apikey': SUPABASE_KEY,
      'Authorization': 'Bearer ' + SUPABASE_KEY,
      'Prefer': 'return=minimal'
    },
    body: JSON.stringify(data)
  })
  .then(function(res) {
    if (!res.ok) { return res.text().then(function(t) { throw new Error(t); }); }
    var first = data.name ? data.name.split(' ')[0] : '';
    document.getElementById('success-title').textContent = first ? "You're all set, " + first + "." : "You're all set.";
    document.getElementById('view-form').style.display = 'none';
    document.getElementById('view-success').style.display = 'block';
  })
  .catch(function(e) {
    btn.disabled = false;
    btn.textContent = 'Submit Intake Form';
    alert('Something went wrong. Please try again.\n\n' + e.message);
  });
}

function resetForm() {
  document.querySelectorAll('input[type=text],input[type=number],input[type=date],textarea').forEach(function(el) { el.value = ''; });
  document.querySelectorAll('select').forEach(function(el) { el.selectedIndex = 0; });
  document.getElementById('submit-btn').disabled = false;
  document.getElementById('submit-btn').textContent = 'Submit Intake Form';
  document.getElementById('f-cycle-wrap').style.display = 'none';
  stressVal = null;
  initAllPills();
  document.getElementById('view-success').style.display = 'none';
  document.getElementById('view-form').style.display = 'block';
  window.scrollTo(0, 0);
}

function exportCSV() {
  if (!allSubmissions.length) { alert('No data to export.'); return; }
  var keys = Object.keys(allSubmissions[0]);
  var rows = [keys.join(',')];
  allSubmissions.forEach(function(s) {
    rows.push(keys.map(function(k) { return '"' + String(s[k] || '').replace(/"/g, '""') + '"'; }).join(','));
  });
  var blob = new Blob([rows.join('\n')], { type: 'text/csv' });
  var a = document.createElement('a');
  a.href = URL.createObjectURL(blob);
  a.download = 'ziad_intakes_' + new Date().toISOString().slice(0, 10) + '.csv';
  a.click();
}

function fmtDate(iso, long) {
  if (!iso) return '';
  var d = new Date(iso);
  if (long) return d.toLocaleDateString('en-GB', { day: 'numeric', month: 'short', year: 'numeric', hour: '2-digit', minute: '2-digit' });
  return d.toLocaleDateString('en-GB', { day: 'numeric', month: 'short', year: 'numeric' });
}

function esc(s) {
  return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');
}

window.addEventListener('DOMContentLoaded', function() {
  initAllPills();
});
</script>
</body>
</html>
