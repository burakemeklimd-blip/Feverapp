<!doctype html>
<html lang="tr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>PediFever • Decision Support (MVP)</title>

  <!-- Premium-ish system font stack -->
  <style>
    :root{
      --bg: #0b1220;
      --panel: rgba(255,255,255,.06);
      --panel2: rgba(255,255,255,.08);
      --stroke: rgba(255,255,255,.12);
      --text: rgba(255,255,255,.92);
      --muted: rgba(255,255,255,.68);
      --muted2: rgba(255,255,255,.55);
      --good: #34d399;
      --warn: #fbbf24;
      --bad:  #fb7185;
      --chip: rgba(255,255,255,.09);
      --shadow: 0 18px 60px rgba(0,0,0,.45);
      --shadow2: 0 10px 28px rgba(0,0,0,.35);
      --radius: 18px;
      --radius2: 14px;
      --font: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial;
    }
    *{ box-sizing:border-box; }
    html,body{ height:100%; }
    body{
      margin:0;
      font-family: var(--font);
      color: var(--text);
      background:
        radial-gradient(1200px 600px at 20% 10%, rgba(59,130,246,.25), transparent 55%),
        radial-gradient(900px 540px at 85% 25%, rgba(236,72,153,.18), transparent 55%),
        radial-gradient(700px 520px at 35% 90%, rgba(34,197,94,.16), transparent 60%),
        linear-gradient(180deg, #070b14, #0b1220 35%, #060a12);
    }

    .wrap{ max-width: 1100px; margin:0 auto; padding: 26px 16px 64px; }
    .topbar{
      display:flex; align-items:flex-start; justify-content:space-between; gap:16px; flex-wrap:wrap;
      margin-bottom: 14px;
    }
    .brand{
      display:flex; align-items:center; gap:12px;
    }
    .logo{
      width:44px; height:44px; border-radius: 14px;
      background:
        radial-gradient(18px 18px at 30% 30%, rgba(255,255,255,.85), rgba(255,255,255,.25)),
        linear-gradient(135deg, rgba(59,130,246,.95), rgba(236,72,153,.85));
      box-shadow: var(--shadow2);
      position: relative;
      overflow:hidden;
    }
    .logo:after{
      content:"";
      position:absolute; inset:-12px;
      background: radial-gradient(circle at 30% 30%, rgba(255,255,255,.35), transparent 45%);
      transform: rotate(12deg);
    }
    h1{ margin:0; font-size: 20px; letter-spacing: .2px; }
    .sub{ margin-top:4px; color: var(--muted); font-size: 13px; line-height: 1.35; max-width: 720px; }

    .pill{
      display:inline-flex; align-items:center; gap:8px;
      padding: 8px 12px; border-radius: 999px;
      border: 1px solid var(--stroke);
      background: rgba(255,255,255,.05);
      color: var(--muted);
      font-size:12px; font-weight: 700;
      backdrop-filter: blur(8px);
    }
    .pill strong{ color: var(--text); font-weight: 800; }

    .panel{
      border: 1px solid var(--stroke);
      background: linear-gradient(180deg, var(--panel), rgba(255,255,255,.03));
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow:hidden;
    }
    .panelHeader{
      padding: 14px 16px;
      border-bottom: 1px solid rgba(255,255,255,.08);
      display:flex; align-items:center; justify-content:space-between; gap:12px; flex-wrap:wrap;
    }
    .panelHeader h2{
      margin:0; font-size: 14px; letter-spacing: .2px;
      color: rgba(255,255,255,.88);
      display:flex; align-items:center; gap:10px;
    }
    .dot{ width:8px; height:8px; border-radius:999px; background: rgba(255,255,255,.35); }
    .panelBody{ padding: 16px; }

    .grid{
      display:grid; grid-template-columns: 1fr; gap: 14px;
    }
    @media(min-width: 980px){
      .grid{ grid-template-columns: 1.05fr .95fr; gap: 16px; }
    }

    label{ display:block; font-size: 12px; font-weight: 800; color: rgba(255,255,255,.78); margin-bottom: 7px; }
    .field{
      width:100%;
      padding: 11px 12px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.05);
      color: var(--text);
      outline: none;
      font-size: 14px;
    }
    .field:focus{
      border-color: rgba(59,130,246,.6);
      box-shadow: 0 0 0 4px rgba(59,130,246,.15);
    }
    .row2{ display:grid; grid-template-columns: 1fr 1fr; gap: 12px; }
    @media(max-width: 520px){ .row2{ grid-template-columns: 1fr; } }

    .seg{
      display:flex; align-items:center; gap:6px;
      padding: 6px;
      border-radius: 999px;
      border:1px solid rgba(255,255,255,.12);
      background: rgba(255,255,255,.05);
      backdrop-filter: blur(10px);
    }
    .seg button{
      border:0; background: transparent;
      color: var(--muted);
      font-weight: 900;
      padding: 8px 12px;
      border-radius: 999px;
      cursor:pointer;
      font-size:12px;
    }
    .seg button.active{
      background: rgba(255,255,255,.14);
      color: rgba(255,255,255,.92);
      box-shadow: 0 10px 18px rgba(0,0,0,.25);
    }

    .checklist{ display:grid; gap: 10px; margin-top: 6px; }
    .check{
      display:flex; gap: 10px; align-items:flex-start;
      padding: 10px 10px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.10);
      background: rgba(255,255,255,.04);
    }
    .check input{ margin-top: 3px; }
    .check span{ color: rgba(255,255,255,.78); font-size: 13px; line-height: 1.25; }

    .actions{ display:flex; gap:10px; flex-wrap:wrap; margin-top: 4px; }
    .btn{
      display:inline-flex; align-items:center; justify-content:center; gap:10px;
      padding: 11px 14px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.05);
      color: rgba(255,255,255,.88);
      cursor:pointer;
      font-weight: 900;
      font-size: 13px;
    }
    .btn:hover{ background: rgba(255,255,255,.08); }
    .btn.primary{
      border-color: rgba(59,130,246,.55);
      background: linear-gradient(135deg, rgba(59,130,246,.85), rgba(99,102,241,.65));
      box-shadow: 0 18px 35px rgba(59,130,246,.22);
    }
    .btn.primary:hover{
      filter: brightness(1.03);
    }

    .note{
      padding: 12px 12px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.12);
      background: rgba(255,255,255,.05);
      color: var(--muted);
      font-size: 12px;
      line-height: 1.35;
    }
    .error{
      padding: 12px 12px;
      border-radius: 14px;
      border: 1px solid rgba(251,113,133,.45);
      background: rgba(251,113,133,.10);
      color: rgba(255,255,255,.92);
      font-size: 12px;
      line-height: 1.35;
    }

    .resultBadge{
      display:inline-flex; align-items:center; gap:10px;
      padding: 10px 12px;
      border-radius: 999px;
      border: 1px solid rgba(255,255,255,.12);
      background: rgba(255,255,255,.05);
      font-weight: 1000;
      font-size: 12px;
      letter-spacing: .2px;
      backdrop-filter: blur(10px);
    }
    .resultBadge .b{ width:10px; height:10px; border-radius:999px; }
    .resultBadge.red{ border-color: rgba(251,113,133,.45); }
    .resultBadge.red .b{ background: var(--bad); }
    .resultBadge.amber{ border-color: rgba(251,191,36,.45); }
    .resultBadge.amber .b{ background: var(--warn); }
    .resultBadge.green{ border-color: rgba(52,211,153,.45); }
    .resultBadge.green .b{ background: var(--good); }

    .advice{
      margin-top: 12px;
      border-radius: var(--radius2);
      border: 1px solid rgba(255,255,255,.10);
      background: rgba(255,255,255,.03);
      padding: 12px 14px;
    }
    .advice ul{ margin: 8px 0 0 18px; color: rgba(255,255,255,.80); font-size: 13px; line-height: 1.35; }
    .advice li{ margin: 6px 0; }

    .sectionTitle{
      margin-top: 14px;
      font-size: 13px;
      font-weight: 1000;
      color: rgba(255,255,255,.90);
      letter-spacing: .2px;
    }
    .kpis{ display:grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 10px; }
    @media(max-width:520px){ .kpis{ grid-template-columns: 1fr; } }
    .kpi{
      border: 1px solid rgba(255,255,255,.10);
      background: rgba(255,255,255,.04);
      border-radius: 16px;
      padding: 12px;
    }
    .kpi .t{ font-size: 12px; color: var(--muted2); font-weight: 800; }
    .kpi .v{ margin-top: 6px; font-size: 20px; font-weight: 1100; letter-spacing: .2px; }
    .tiny{ font-size: 12px; color: var(--muted2); margin-top: 10px; }

    .footer{
      margin-top: 14px;
      color: rgba(255,255,255,.55);
      font-size: 12px;
    }
    a{ color: rgba(147,197,253,.95); text-decoration: none; }
    a:hover{ text-decoration: underline; }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="topbar">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <div>
          <h1 id="title">PediFever • Ateş Karar Destek</h1>
          <div class="sub" id="subtitle">Bu araç bilgilendirme amaçlıdır; muayene ve hekim değerlendirmesi yerine geçmez.</div>
          <div style="margin-top:10px; display:flex; gap:10px; flex-wrap:wrap;">
            <div class="pill"><strong>0–12</strong> yaş</div>
            <div class="pill">TR / EN</div>
            <div class="pill">No data storage</div>
          </div>
        </div>
      </div>

      <div class="panel" style="max-width: 360px;">
        <div class="panelHeader">
          <h2><span class="dot"></span><span id="prefsTitle">Ayarlar</span></h2>
          <div class="seg" role="tablist" aria-label="Language">
            <button id="btnTR" class="active" type="button">TR</button>
            <button id="btnEN" type="button">EN</button>
          </div>
        </div>
        <div class="panelBody">
          <div class="check" style="margin:0;">
            <input type="checkbox" id="accept">
            <span id="disclaimerCheck">Okudum, anladım. Bu aracın genel bilgilendirme amaçlı olduğunu kabul ediyorum.</span>
          </div>
          <div class="tiny" id="disclaimerTiny">
            Not: Bu araç tanı koymaz; “genel bilgilendirme / karar destek” niteliğindedir.
          </div>
        </div>
      </div>
    </div>

    <div class="grid">
      <!-- INPUTS -->
      <section class="panel">
        <div class="panelHeader">
          <h2><span class="dot"></span><span id="inputsTitle">Girdiler</span></h2>
          <div class="pill" id="statusPill">Ready</div>
        </div>

        <div class="panelBody" style="display:grid; gap: 14px;">
          <div>
            <label id="ageLabel">Yaş grubu</label>
            <select id="ageBand" class="field">
              <option value="0_3m">0–3 ay</option>
              <option value="3_36m" selected>3–36 ay</option>
              <option value="3plus">3 yaş+</option>
            </select>
          </div>

          <div class="row2">
            <div>
              <label id="wLabel">Kilo (kg)</label>
              <input id="weight" class="field" type="number" step="0.1" value="10" inputmode="decimal">
            </div>
            <div>
              <label id="tLabel">Ateş (°C)</label>
              <input id="temp" class="field" type="number" step="0.1" value="38.5" inputmode="decimal">
            </div>
          </div>

          <div>
            <label id="dLabel">Ateş süresi</label>
            <select id="duration" class="field">
              <option value="lt24">&lt;24 saat</option>
              <option value="24_72">24–72 saat</option>
              <option value="gt72">&gt;72 saat</option>
            </select>
          </div>

          <div>
            <div class="sectionTitle" id="symptomsTitle">Eşlik eden bulgular</div>
            <div class="checklist" id="symptomList"></div>
          </div>

          <div id="err" class="error" style="display:none;"></div>

          <div class="actions">
            <button class="btn primary" id="calcBtn" type="button">Hesapla</button>
            <button class="btn" id="resetBtn" type="button">Sıfırla</button>
          </div>

          <div class="note" id="hint">
            Girdileri doldurup “Hesapla”ya basın.
          </div>
        </div>
      </section>

      <!-- OUTPUT -->
      <section class="panel">
        <div class="panelHeader">
          <h2><span class="dot"></span><span id="outTitle">Sonuç</span></h2>
          <div id="badge" class="resultBadge green" style="display:none;">
            <span class="b"></span><span id="badgeText">YEŞİL — Evde izlem uygun olabilir</span>
          </div>
        </div>

        <div class="panelBody">
          <div id="result" style="display:none;">
            <div class="advice">
              <div class="sectionTitle" id="adviceTitle">Öneriler</div>
              <ul id="advice"></ul>
            </div>

            <div class="sectionTitle" id="doseTitle" style="margin-top:14px;">Doz hesaplayıcı (genel)</div>
            <div class="tiny" id="doseNote">
              Aşağıdaki hesaplama bilgilendirme amaçlıdır. Kullandığınız ilacın prospektüsünü ve hekim önerisini esas alın.
            </div>

            <div style="display:grid; gap:12px; margin-top:12px;">
              <!-- Paracetamol -->
              <div class="kpi" style="padding:14px;">
                <div style="display:flex; justify-content:space-between; gap:10px; flex-wrap:wrap;">
                  <div style="font-weight:1100;" id="paraTitle">Parasetamol</div>
                  <div class="tiny" id="paraInterval">Aralık: 4–6 saatte bir (günlük maksimumu aşmayın)</div>
                </div>
                <div style="margin-top:10px;">
                  <label id="chooseSusp1">Süspansiyon seç</label>
                  <select id="paraSusp" class="field">
                    <option value="120">120 mg / 5 mL</option>
                    <option value="160">160 mg / 5 mL</option>
                  </select>
                </div>
                <div class="kpis">
                  <div class="kpi">
                    <div class="t" id="paraPerDose">Tek doz (15 mg/kg)</div>
                    <div class="v"><span id="paraMg">0</span> <span id="mgLbl1">mg</span></div>
                  </div>
                  <div class="kpi">
                    <div class="t" id="paraPerDose2">Tek doz</div>
                    <div class="v"><span id="paraMl">0</span> <span id="mlLbl1">mL</span></div>
                  </div>
                </div>
              </div>

              <!-- Ibuprofen -->
              <div class="kpi" style="padding:14px;">
                <div style="display:flex; justify-content:space-between; gap:10px; flex-wrap:wrap;">
                  <div style="font-weight:1100;" id="ibuTitle">İbuprofen</div>
                  <div class="tiny" id="ibuInterval">Aralık: 6–8 saatte bir (dehidratasyonda/şüphede kaçının)</div>
                </div>
                <div id="ibuWarn" class="error" style="display:none; margin-top:10px;"></div>
                <div style="margin-top:10px;">
                  <label id="chooseSusp2">Süspansiyon seç</label>
                  <select id="ibuSusp" class="field">
                    <option value="100">100 mg / 5 mL</option>
                    <option value="200">200 mg / 5 mL</option>
                  </select>
                </div>
                <div class="kpis">
                  <div class="kpi">
                    <div class="t" id="ibuPerDose">Tek doz (10 mg/kg)</div>
                    <div class="v"><span id="ibuMg">0</span> <span id="mgLbl2">mg</span></div>
                  </div>
                  <div class="kpi">
                    <div class="t" id="ibuPerDose2">Tek doz</div>
                    <div class="v"><span id="ibuMl">0</span> <span id="mlLbl2">mL</span></div>
                  </div>
                </div>
              </div>

              <div class="footer" id="noData">Bu MVP veri saklamaz. Kullanıcı girdileri tarayıcıda işlenir.</div>
            </div>
          </div>

          <div class="footer" id="footerNote" style="margin-top:14px;">
            Not: Kural seti konservatif hazırlanmıştır. Klinik yaklaşımınıza göre özelleştirebiliriz.
          </div>
        </div>
      </section>
    </div>
  </div>

<script>
  const COPY = {
    tr: {
      title: "PediFever • Ateş Karar Destek",
      subtitle: "Bu araç bilgilendirme amaçlıdır; muayene ve hekim değerlendirmesi yerine geçmez.",
      prefsTitle: "Ayarlar",
      disclaimerCheck: "Okudum, anladım. Bu aracın genel bilgilendirme amaçlı olduğunu kabul ediyorum.",
      disclaimerTiny: "Not: Bu araç tanı koymaz; “genel bilgilendirme / karar destek” niteliğindedir.",
      inputsTitle: "Girdiler",
      outTitle: "Sonuç",
      hint: "Girdileri doldurup “Hesapla”ya basın.",
      ageLabel: "Yaş grubu",
      wLabel: "Kilo (kg)",
      tLabel: "Ateş (°C)",
      dLabel: "Ateş süresi",
      symptomsTitle: "Eşlik eden bulgular",
      calcBtn: "Hesapla",
      resetBtn: "Sıfırla",
      adviceTitle: "Öneriler",
      doseTitle: "Doz hesaplayıcı (genel)",
      doseNote: "Aşağıdaki hesaplama bilgilendirme amaçlıdır. Kullandığınız ilacın prospektüsünü ve hekim önerisini esas alın.",
      chooseSusp: "Süspansiyon seç",
      paraTitle: "Parasetamol",
      ibuTitle: "İbuprofen",
      paraInterval: "Aralık: 4–6 saatte bir (günlük maksimumu aşmayın)",
      ibuInterval: "Aralık: 6–8 saatte bir (dehidratasyonda/şüphede kaçının)",
      paraPerDose: "Tek doz (15 mg/kg)",
      ibuPerDose: "Tek doz (10 mg/kg)",
      perDose2: "Tek doz",
      mg: "mg",
      ml: "mL",
      noData: "Bu MVP veri saklamaz. Kullanıcı girdileri tarayıcıda işlenir.",
      footerNote: "Not: Kural seti konservatif hazırlanmıştır. Klinik yaklaşımınıza göre özelleştirebiliriz.",
      ibuWarn: "6 aydan küçüklerde ibuprofen kullanımı için hekime danışın.",
      validation: {
        needDisclaimer: "Devam etmek için onayı işaretleyin.",
        weight: "Kilo 2–80 kg aralığında olmalı.",
        temp: "Ateş 34–43 °C aralığında olmalı."
      },
      triage: {
        red: "KIRMIZI — Acil değerlendirme önerilir",
        amber: "SARI — Aynı gün hekim değerlendirmesi düşünülür",
        green: "YEŞİL — Evde izlem uygun olabilir"
      },
      advice: {
        red: [
          "Acil servise başvuru / acil hekim değerlendirmesi önerilir.",
          "Bilinç değişikliği, solunum sıkıntısı, morarma, peteşi/purpura gibi bulgular acildir."
        ],
        amber: [
          "Aynı gün çocuk hekimi değerlendirmesi uygun olur.",
          "Genel durum bozulursa veya yeni kırmızı bayrak gelişirse acile başvurun."
        ],
        green: [
          "Genel durum iyi ise evde izlem yapılabilir.",
          "Bol sıvı, hafif giydirme, ortam ısısını ılımlı tutma önerilir.",
          "Ateş tek başına değil, çocuğun genel durumu önemlidir."
        ]
      },
      ageBands: { "0_3m":"0–3 ay", "3_36m":"3–36 ay", "3plus":"3 yaş+" },
      durations: { "lt24":"<24 saat", "24_72":"24–72 saat", "gt72":">72 saat" },
      symptomLabels: {
        poorGeneral: "Genel durum kötü / uyandırmak zor",
        respDistress: "Solunum sıkıntısı",
        cyanosis: "Morarma",
        petechiae: "Peteşi/purpura benzeri döküntü",
        neckStiffness: "Ense sertliği / şiddetli baş ağrısı / fotofobi",
        cannotDrink: "Sıvı alamama / inatçı kusma",
        dehydration: "Belirgin susuzluk bulguları (az idrar, ağız kuruluğu vb.)",
        immunocompromised: "İmmünsüpresyon / ciddi kronik hastalık"
      }
    },
    en: {
      title: "PediFever • Fever Decision Support",
      subtitle: "This tool is for general information only; it does not replace clinical evaluation or a physician’s assessment.",
      prefsTitle: "Preferences",
      disclaimerCheck: "I understand and agree this tool provides general information only.",
      disclaimerTiny: "Note: This tool does not provide a diagnosis; it is decision support / general information.",
      inputsTitle: "Inputs",
      outTitle: "Result",
      hint: "Fill in the inputs and click “Calculate”.",
      ageLabel: "Age group",
      wLabel: "Weight (kg)",
      tLabel: "Temperature (°C)",
      dLabel: "Fever duration",
      symptomsTitle: "Associated features",
      calcBtn: "Calculate",
      resetBtn: "Reset",
      adviceTitle: "Guidance",
      doseTitle: "Dose calculator (general)",
      doseNote: "The calculation below is for general information only. Follow product labeling and your clinician’s advice.",
      chooseSusp: "Choose suspension",
      paraTitle: "Paracetamol (Acetaminophen)",
      ibuTitle: "Ibuprofen",
      paraInterval: "Interval: every 4–6 hours (do not exceed daily maximum)",
      ibuInterval: "Interval: every 6–8 hours (avoid if dehydrated / unsure)",
      paraPerDose: "Per dose (15 mg/kg)",
      ibuPerDose: "Per dose (10 mg/kg)",
      perDose2: "Per dose",
      mg: "mg",
      ml: "mL",
      noData: "This MVP stores no data. Inputs are processed in the browser.",
      footerNote: "Note: Ruleset is intentionally conservative. We can tailor it to your protocol.",
      ibuWarn: "For infants under 6 months, consult a clinician before ibuprofen.",
      validation: {
        needDisclaimer: "Please accept the disclaimer to continue.",
        weight: "Weight must be between 2–80 kg.",
        temp: "Temperature must be between 34–43 °C."
      },
      triage: {
        red: "RED — Urgent evaluation recommended",
        amber: "AMBER — Same-day clinician review advised",
        green: "GREEN — Home monitoring may be appropriate"
      },
      advice: {
        red: [
          "Seek urgent medical care / emergency evaluation.",
          "Altered mental status, breathing difficulty, cyanosis, petechiae/purpura are red flags."
        ],
        amber: [
          "Same-day pediatric assessment is recommended.",
          "Go to emergency care if red flags develop or condition worsens."
        ],
        green: [
          "If overall condition is good, home monitoring can be reasonable.",
          "Encourage fluids, light clothing, comfortable ambient temperature.",
          "Overall appearance matters more than the number alone."
        ]
      },
      ageBands: { "0_3m":"0–3 months", "3_36m":"3–36 months", "3plus":"3 years+" },
      durations: { "lt24":"<24 hours", "24_72":"24–72 hours", "gt72":">72 hours", },
      symptomLabels: {
        poorGeneral: "Poor general condition / difficult to arouse",
        respDistress: "Breathing difficulty",
        cyanosis: "Bluish discoloration (cyanosis)",
        petechiae: "Petechiae/purpura-like rash",
        neckStiffness: "Neck stiffness / severe headache / photophobia",
        cannotDrink: "Unable to drink / persistent vomiting",
        dehydration: "Signs of dehydration (low urine, dry mouth, etc.)",
        immunocompromised: "Immunocompromised / serious chronic condition"
      }
    }
  };

  const symptomKeys = [
    "poorGeneral","respDistress","cyanosis","petechiae","neckStiffness","cannotDrink","dehydration","immunocompromised"
  ];

  let lang = "tr";

  const $ = (id) => document.getElementById(id);

  function roundTo(val, step){ return Math.round(val/step)*step; }
  function doseToMl(mgDose, mgPer5mL){
    const mgPerMl = mgPer5mL/5;
    return mgDose / mgPerMl;
  }

  // Conservative rule-based triage for MVP
  function computeTriage({ageBand, tempC, duration, symptoms}){
    // RED: any red-flag symptom selected
    if (symptomKeys.some(k => symptoms[k])) return "red";

    // 0–3 months: conservative thresholds
    if (ageBand === "0_3m"){
      if (tempC >= 38.0) return "red";
      if (tempC >= 37.5) return "amber";
    }

    // high fever
    if (tempC >= 40.0) return "amber";

    // duration >72h
    if (duration === "gt72") return "amber";

    // 3–36 months >=39
    if (ageBand === "3_36m" && tempC >= 39.0) return "amber";

    return "green";
  }

  function renderSymptoms(){
    const list = $("symptomList");
    list.innerHTML = "";
    const labels = COPY[lang].symptomLabels;

    symptomKeys.forEach(key => {
      const row = document.createElement("label");
      row.className = "check";
      row.innerHTML = `<input type="checkbox" id="sym_${key}">
                       <span>${labels[key]}</span>`;
      list.appendChild(row);
    });
  }

  function setLang(newLang){
    lang = newLang;
    $("btnTR").classList.toggle("active", lang === "tr");
    $("btnEN").classList.toggle("active", lang === "en");
    document.documentElement.lang = lang;

    const t = COPY[lang];
    $("title").textContent = t.title;
    $("subtitle").textContent = t.subtitle;
    $("prefsTitle").textContent = t.prefsTitle;
    $("disclaimerCheck").textContent = t.disclaimerCheck;
    $("disclaimerTiny").textContent = t.disclaimerTiny;

    $("inputsTitle").textContent = t.inputsTitle;
    $("outTitle").textContent = t.outTitle;
    $("hint").textContent = t.hint;

    $("ageLabel").textContent = t.ageLabel;
    $("wLabel").textContent = t.wLabel;
    $("tLabel").textContent = t.tLabel;
    $("dLabel").textContent = t.dLabel;
    $("symptomsTitle").textContent = t.symptomsTitle;

    $("calcBtn").textContent = t.calcBtn;
    $("resetBtn").textContent = t.resetBtn;

    $("adviceTitle").textContent = t.adviceTitle;
    $("doseTitle").textContent = t.doseTitle;
    $("doseNote").textContent = t.doseNote;

    $("chooseSusp1").textContent = t.chooseSusp;
    $("chooseSusp2").textContent = t.chooseSusp;

    $("paraTitle").textContent = t.paraTitle;
    $("ibuTitle").textContent = t.ibuTitle;

    $("paraInterval").textContent = t.paraInterval;
    $("ibuInterval").textContent = t.ibuInterval;

    $("paraPerDose").textContent = t.paraPerDose;
    $("paraPerDose2").textContent = t.perDose2;
    $("ibuPerDose").textContent = t.ibuPerDose;
    $("ibuPerDose2").textContent = t.perDose2;

    $("mgLbl1").textContent = t.mg;
    $("mgLbl2").textContent = t.mg;
    $("mlLbl1").textContent = t.ml;
    $("mlLbl2").textContent = t.ml;

    $("noData").textContent = t.noData;
    $("footerNote").textContent = t.footerNote;

    // update select option labels
    const ageSel = $("ageBand");
    [...ageSel.options].forEach(opt => opt.textContent = t.ageBands[opt.value]);

    const durSel = $("duration");
    [...durSel.options].forEach(opt => opt.textContent = t.durations[opt.value]);

    // re-render symptom labels in selected language
    const prev = {};
    symptomKeys.forEach(k => prev[k] = $("sym_"+k) ? $("sym_"+k).checked : false);
    renderSymptoms();
    symptomKeys.forEach(k => $("sym_"+k).checked = !!prev[k]);

    // update badge if visible
    if ($("badge").style.display === "inline-flex"){
      // keep current triage text by recalculating
      runCalc(true);
    }
  }

  function getSymptomsState(){
    const s = {};
    symptomKeys.forEach(k => s[k] = $("sym_"+k).checked);
    return s;
  }

  function validate(){
    const t = COPY[lang];
    if (!$("accept").checked) return t.validation.needDisclaimer;

    const w = Number($("weight").value);
    const tc = Number($("temp").value);
    if (!(w >= 2 && w <= 80)) return t.validation.weight;
    if (!(tc >= 34 && tc <= 43)) return t.validation.temp;
    return null;
  }

  function updateDoses(){
    const w = Number($("weight").value);
    const paraSusp = Number($("paraSusp").value);
    const ibuSusp  = Number($("ibuSusp").value);

    const paraMgDose = roundTo(w * 15, 1);
    const paraMl = roundTo(doseToMl(paraMgDose, paraSusp), 0.1);

    const ibuMgDose = roundTo(w * 10, 1);
    const ibuMl = roundTo(doseToMl(ibuMgDose, ibuSusp), 0.1);

    $("paraMg").textContent = paraMgDose.toFixed(1).replace(/\.0$/,"");
    $("paraMl").textContent = paraMl.toFixed(1).replace(/\.0$/,"");
    $("ibuMg").textContent = ibuMgDose.toFixed(1).replace(/\.0$/,"");
    $("ibuMl").textContent = ibuMl.toFixed(1).replace(/\.0$/,"");
  }

  function setBadge(level){
    const t = COPY[lang];
    const badge = $("badge");
    badge.style.display = "inline-flex";
    badge.classList.remove("red","amber","green");
    badge.classList.add(level);
    $("badgeText").textContent = t.triage[level];
  }

  function runCalc(silent=false){
    const err = validate();
    if (err){
      $("err").textContent = err;
      $("err").style.display = "block";
      $("statusPill").innerHTML = "<strong>Error</strong>";
      $("result").style.display = "none";
      $("badge").style.display = "none";
      if (!silent) $("hint").style.display = "block";
      return;
    }

    $("err").style.display = "none";
    $("statusPill").innerHTML = "<strong>OK</strong>";

    const ageBand = $("ageBand").value;
    const tempC = Number($("temp").value);
    const duration = $("duration").value;
    const symptoms = getSymptomsState();

    const level = computeTriage({ageBand, tempC, duration, symptoms});
    setBadge(level);

    const ul = $("advice");
    ul.innerHTML = "";
    COPY[lang].advice[level].forEach(line => {
      const li = document.createElement("li");
      li.textContent = line;
      ul.appendChild(li);
    });

    // ibuprofen warning for under 6 months: we only have 0-3m band in MVP
    const warn = $("ibuWarn");
    if (ageBand === "0_3m"){
      warn.style.display = "block";
      warn.textContent = COPY[lang].ibuWarn;
    } else {
      warn.style.display = "none";
    }

    updateDoses();
    $("result").style.display = "block";
    $("hint").style.display = "none";
  }

  function resetAll(){
    $("accept").checked = false;
    $("ageBand").value = "3_36m";
    $("weight").value = "10";
    $("temp").value = "38.5";
    $("duration").value = "lt24";
    symptomKeys.forEach(k => $("sym_"+k).checked = false);
    $("paraSusp").value = "120";
    $("ibuSusp").value = "100";
    $("err").style.display = "none";
    $("badge").style.display = "none";
    $("result").style.display = "none";
    $("hint").style.display = "block";
    $("statusPill").textContent = "Ready";
  }

  // Events
  $("btnTR").addEventListener("click", () => setLang("tr"));
  $("btnEN").addEventListener("click", () => setLang("en"));

  $("calcBtn").addEventListener("click", () => runCalc(false));
  $("resetBtn").addEventListener("click", resetAll);

  $("paraSusp").addEventListener("change", () => { if ($("result").style.display==="block") updateDoses(); });
  $("ibuSusp").addEventListener("change", () => { if ($("result").style.display==="block") updateDoses(); });
  $("weight").addEventListener("input", () => { if ($("result").style.display==="block") updateDoses(); });

  // Init
  renderSymptoms();
  setLang("tr");
  updateDoses();
</script>
</body>
</html>
