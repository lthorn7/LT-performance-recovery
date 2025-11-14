# LT-performance-recovery
index.html.
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>LT PERFORMANCE RECOVERY — Bookings</title>
  <meta name="description" content="Nutrition & Sports Massage bookings — LT Performance Recovery" />
  <style>
    /* ========== Basic Reset & Typography ========== */
    :root{
      --bg:#f7fbfa;
      --card:#ffffff;
      --accent:#2e8f8a; /* calm teal */
      --accent-2:#1b6b66;
      --muted:#6b7280;
      --glass: rgba(255,255,255,0.6);
      --shadow: 0 6px 20px rgba(23,23,23,0.08);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background: linear-gradient(180deg,var(--bg), #eef7f6 60%);
      color:#0f172a;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding-bottom:80px;
    }
    a{color:var(--accent); text-decoration:none}
    h1,h2,h3{margin:0 0 8px 0; line-height:1.05}
    p{margin:0 0 12px 0; color:var(--muted)}
    .container{max-width:1100px;margin:36px auto;padding:0 20px}

    /* ========== Header ========== */
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      margin-bottom:22px;
    }
    .brand{
      display:flex;align-items:center;gap:14px;
    }
    .logo{
      width:58px;height:58px;border-radius:10px;
      background:linear-gradient(135deg,var(--accent),var(--accent-2));
      box-shadow: 0 6px 20px rgba(14,60,58,0.18);
      display:flex;align-items:center;justify-content:center;
      color:white;font-weight:700;font-size:18px;
    }
    nav{display:flex;gap:18px;align-items:center}
    .nav-link{font-weight:600;color:var(--accent-2)}
    .cta{
      background:var(--accent-2);color:white;padding:10px 14px;border-radius:10px;font-weight:700;
      box-shadow: var(--shadow);
    }

    /* ========== Grid ========== */
    .grid{
      display:grid;
      grid-template-columns: 1fr 420px;
      gap:30px;
      align-items:start;
    }

    /* ========== Left Card ========== */
    .card{
      background:var(--card);padding:22px;border-radius:14px;box-shadow:var(--shadow);
    }
    .hero{
      display:flex;gap:18px;align-items:center;margin-bottom:18px;
    }
    .hero .title{
      font-size:22px;font-weight:800;
    }
    .pill{display:inline-block;padding:6px 10px;border-radius:999px;background:linear-gradient(90deg, rgba(46,143,138,0.12), rgba(27,107,102,0.06));font-weight:700;color:var(--accent-2);font-size:12px}

    /* ========== Services List ========== */
    .services{display:flex;flex-direction:column;gap:12px;margin-top:10px}
    .service{
      border-radius:10px;padding:12px;background:linear-gradient(180deg, rgba(46,143,138,0.035), rgba(27,107,102,0.02));
      display:flex;justify-content:space-between;align-items:center;
    }
    .service .meta{color:var(--muted);font-size:13px}
    .price{font-weight:800;color:var(--accent-2)}

    /* ========== Booking Column ========== */
    .booking { position:relative; }
    .booking h3{margin-bottom:8px}
    form .row{display:flex;gap:10px;align-items:center;margin-bottom:10px}
    .row.col{flex-direction:column;align-items:stretch}
    label{font-size:13px;color:var(--muted);margin-bottom:6px;display:block}
    input[type="text"], input[type="email"], input[type="date"], select {
      width:100%;padding:10px;border-radius:8px;border:1px solid #e6eef0;background:white;
      font-size:15px;
    }
    .timeslots{display:flex;flex-wrap:wrap;gap:8px}
    .slot{padding:8px 10px;border-radius:10px;border:1px solid #dff2ef;background:transparent;cursor:pointer}
    .slot.selected{background:var(--accent);color:white;border-color:transparent}
    .btn{
      display:inline-block;padding:10px 14px;border-radius:10px;font-weight:800;border:none;background:var(--accent);
      color:white;cursor:pointer;
    }
    .btn.ghost{background:transparent;border:1px solid #cfeeea;color:var(--accent-2)}
    .muted-small{font-size:13px;color:var(--muted)}

    /* ========== Confirmation ========== */
    .confirm{
      padding:14px;border-radius:10px;background:linear-gradient(180deg, #f2fffe, #ffffff);border:1px solid #e6f6f5;
    }

    /* ========== Responsive ========== */
    @media (max-width:980px){
      .grid{grid-template-columns:1fr; }
      header{flex-direction:column;align-items:flex-start;gap:12px}
    }

    footer{margin-top:24px;text-align:center;color:var(--muted);font-size:13px}
    small.note{color:var(--muted); display:block;margin-top:8px}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">LT</div>
        <div>
          <div style="font-weight:900;font-size:16px">LT PERFORMANCE RECOVERY</div>
          <div class="muted-small">Nutrition · Sports Massage · Recovery</div>
        </div>
      </div>
      <nav>
        <a class="nav-link" href="#services">Services</a>
        <a class="nav-link" href="#booking">Book</a>
        <a class="cta" href="#booking">Book Now</a>
      </nav>
    </header>

    <main class="grid">
      <section>
        <div class="card hero">
          <div>
            <div class="pill">Experienced Therapist</div>
            <div class="title">Recover faster. Perform better.</div>
            <p>Holistic nutrition consultations combined with targeted sports massage to speed recovery, reduce injury risk and optimise performance.</p>
            <small class="muted-small">Open Mon–Sat · Flexible appointment lengths</small>
          </div>
        </div>

        <div id="services" class="card" style="margin-top:18px">
          <h2>Services</h2>
          <p class="muted-small">Choose a service and book a time below.</p>

          <div class="services" id="servicesList">
            <!-- Services populated by JS -->
          </div>

          <div style="margin-top:18px">
            <h3>Location</h3>
            <p class="muted-small">LT Performance Studio — 12 Recovery Lane, Cityville</p>
          </div>
        </div>

        <div class="card" style="margin-top:18px">
          <h2>About</h2>
          <p>We combine evidence-informed nutrition plans with hands-on sports massage to reduce pain, restore function and help athletes return stronger. Appointments are one-on-one and tailored to each client.</p>
        </div>

      </section>

      <aside class="booking">
        <div id="bookingCard" class="card">
          <h3 id="bookingTitle">Book an appointment</h3>
          <p class="muted-small">Choose service, date and an available time slot. You’ll receive a downloadable calendar invite.</p>

          <form id="bookingForm" autocomplete="off">
            <div class="row col">
              <label for="service">Service</label>
              <select id="service" required>
                <!-- options populated by JS -->
              </select>
            </div>

            <div class="row">
              <div style="flex:1">
                <label for="date">Date</label>
                <input id="date" type="date" required>
              </div>
              <div style="width:140px">
                <label for="duration">Duration</label>
                <select id="duration">
                  <!-- durations adjust based on service -->
                </select>
              </div>
            </div>

            <div class="row col">
              <label>Available times</label>
              <div id="times" class="timeslots">
                <!-- slots generated by JS -->
              </div>
              <div id="noSlots" style="display:none;color:#9aa6a3;margin-top:8px">No available slots for this date — try another day.</div>
            </div>

            <div class="row col" style="margin-top:6px">
              <label for="name">Full name</label>
              <input id="name" type="text" required placeholder="Your name">
            </div>
            <div class="row">
              <div style="flex:1">
                <label for="email">Email</label>
                <input id="email" type="email" required placeholder="you@email.com">
              </div>
              <div style="width:150px">
                <label for="phone">Phone</label>
                <input id="phone" type="text" placeholder="+44 7..." >
              </div>
            </div>

            <div class="row" style="margin-top:10px;justify-content:space-between;align-items:center;">
              <div>
                <label for="payment">Payment</label>
                <select id="payment">
                  <option value="pay_on_site">Pay on site</option>
                  <option value="invoice">Invoice (card link)</option>
                  <option value="placeholder">Card (placeholder)</option>
                </select>
                <small class="muted-small"> — integration placeholder</small>
              </div>
              <div>
                <button id="bookBtn" class="btn" type="submit">Confirm booking</button>
              </div>
            </div>

            <small class="muted-small">By booking you agree to our <a href="#">terms</a>.</small>
          </form>
        </div>

        <div id="confirmation" class="card" style="margin-top:14px;display:none">
          <!-- Confirmation area -->
        </div>

        <footer>
          <small class="muted-small">Questions? Email <a id="contactEmail" href="mailto:hello@ltperformance.com">hello@ltperformance.com</a></small>
          <small style="display:block;margin-top:6px;color:var(--muted)">© LT PERFORMANCE RECOVERY</small>
        </footer>
      </aside>
    </main>
  </div>

  <script>
    /* ===========================
       CONFIG — edit these values
       =========================== */
    const CONFIG = {
      businessName: "LT PERFORMANCE RECOVERY",
      contactEmail: "hello@ltperformance.com",
      // Business hours (24h) Mon-Sat (0=Sun..6=Sat). Simple weekly pattern.
      hours: {
        // open and close times for booking (hour:minute)
        open: "09:00",
        close: "18:00",
      },
      // Services: id, title, durationMin, priceGBP
      services: [
        { id: "sports_massage", title: "Sports Massage", duration: 60, price: 55 },
        { id: "sports_massage_90", title: "Sports Massage (90 min)", duration: 90, price: 80 },
        { id: "nutrition_consult", title: "Nutrition Consultation (Initial)", duration: 60, price: 65 },
        { id: "nutrition_follow", title: "Nutrition Follow-up", duration: 30, price: 35 }
      ],
      minSlotStep: 15, // minutes
      // buffer minutes between bookings (preparation)
      bufferMinutes: 10,
      // admin email for notifications (placeholder)
      adminEmail: "hello@ltperformance.com",
      // LocalStorage key to store bookings (simple demo)
      storageKey: "ltpr-bookings-v1"
    };

    /* ===========================
       Helper utils
       =========================== */
    function $(sel){return document.querySelector(sel)}
    function $all(sel){return Array.from(document.querySelectorAll(sel))}
    function pad(n){return n<10? "0"+n : ""+n}

    function timeToMinutes(t){
      const [h,m] = t.split(":").map(Number); return h*60 + m;
    }
    function minutesToTime(mins){
      const hh = Math.floor(mins/60); const mm = mins%60; return pad(hh)+":"+pad(mm);
    }

    /* ========== Populate Services UI ========== */
    const servicesList = $("#servicesList");
    const serviceSelect = $("#service");
    const durationSelect = $("#duration");
    const contactEmail = $("#contactEmail");
    contactEmail.href = "mailto:" + CONFIG.contactEmail;
    contactEmail.textContent = CONFIG.contactEmail;

    CONFIG.services.forEach(s=>{
      // list item
      const div = document.createElement("div"); div.className = "service";
      div.innerHTML = `
        <div>
          <div style="font-weight:800">${s.title}</div>
          <div class="meta">${s.duration} min · <span class="muted-small">Price</span> <span class="price">£${s.price}</span></div>
        </div>
        <div style="display:flex;flex-direction:column;gap:8px;align-items:flex-end">
          <div class="pill">${s.duration}m</div>
          <div class="muted-small">£${s.price}</div>
        </div>
      `;
      servicesList.appendChild(div);

      // select option
      const opt = document.createElement("option");
      opt.value = s.id;
      opt.textContent = `${s.title} — ${s.duration} min — £${s.price}`;
      serviceSelect.appendChild(opt);
    });

    // populate durations from selected service (some services include their own duration options)
    function populateDurationForSelected(){
      const sel = serviceSelect.value;
      const svc = CONFIG.services.find(x=>x.id===sel);
      durationSelect.innerHTML = "";
      const opt = document.createElement("option");
      opt.value = svc.duration;
      opt.textContent = svc.duration + " minutes";
      durationSelect.appendChild(opt);
    }

    serviceSelect.addEventListener("change", ()=>{
      populateDurationForSelected();
      generateTimeslots();
    });

    /* ========== Date input: limit range (today -> +60 days) ========== */
    const dateInput = $("#date");
    const today = new Date();
    const maxDays = 60;
    const isoToday = today.toISOString().slice(0,10);
    const isoMax = new Date(today.getTime() + maxDays*24*60*60*1000).toISOString().slice(0,10);
    dateInput.min = isoToday;
    dateInput.max = isoMax;
    dateInput.value = isoToday;

    /* ========== Bookings storage (simple) ========== */
    function loadBookings(){
      try{
        return JSON.parse(localStorage.getItem(CONFIG.storageKey) || "[]");
      }catch(e){ return []; }
    }
    function saveBooking(b){
      const all = loadBookings();
      all.push(b);
      localStorage.setItem(CONFIG.storageKey, JSON.stringify(all));
    }

    /* ========== Timeslot generation ========== */
    const timesContainer = $("#times");
    const noSlots = $("#noSlots");

    function generateTimeslots(){
      timesContainer.innerHTML = "";
      noSlots.style.display = "none";

      const dateVal = dateInput.value;
      if(!dateVal) return;
      const selectedService = serviceSelect.value;
      const svc = CONFIG.services.find(x=>x.id===selectedService);
      const duration = Number(durationSelect.value || svc.duration);

      // Business hours
      const openM = timeToMinutes(CONFIG.hours.open);
      const closeM = timeToMinutes(CONFIG.hours.close);

      // Create candidate start times at minSlotStep intervals
      const step = CONFIG.minSlotStep;
      const slots = [];
      for(let t=openM; t + duration <= closeM; t += step){
        slots.push({startMin:t, endMin:t+duration});
      }

      // Remove past times if date is today
      const chosenDate = new Date(dateVal + "T00:00:00");
      const isToday = (new Date()).toISOString().slice(0,10) === dateVal;
      const nowMins = (()=>{ const d = new Date(); return d.getHours()*60 + d.getMinutes(); })();

      const existing = loadBookings().filter(b=> b.date === dateVal);

      const available = slots.filter(slot=>{
        // not in the past today
        if(isToday && slot.startMin <= nowMins + 25) return false; // 25-minute minimum lead time
        // check collision with existing bookings + buffer
        const collision = existing.some(b=>{
          const bookedStart = timeToMinutes(b.time);
          const bookedEnd = bookedStart + b.duration;
          const slotStart = slot.startMin - CONFIG.bufferMinutes;
          const slotEnd = slot.endMin + CONFIG.bufferMinutes;
          // overlap check
          return Math.max(slotStart, bookedStart) < Math.min(slotEnd, bookedEnd);
        });
        return !collision;
      });

      if(available.length === 0){
        noSlots.style.display = "block";
        return;
      }

      available.forEach(slot=>{
        const btn = document.createElement("button");
        btn.type = "button";
        btn.className = "slot";
        const tlabel = minutesToTime(slot.startMin);
        btn.textContent = tlabel;
        btn.dataset.time = tlabel;
        btn.addEventListener("click", ()=>{
          $all(".slot").forEach(s=>s.classList.remove("selected"));
          btn.classList.add("selected");
        });
        timesContainer.appendChild(btn);
      });
    }

    /* ========== Booking submit handling ========== */
    function resetFormToDefaults(){
      serviceSelect.selectedIndex = 0;
      populateDurationForSelected();
      dateInput.value = isoToday;
      timesContainer.innerHTML = "";
      noSlots.style.display = "none";
      $("#name").value = "";
      $("#email").value = "";
      $("#phone").value = "";
    }

    document.getElementById("bookingForm").addEventListener("submit", function(ev){
      ev.preventDefault();
      // gather
      const svcId = serviceSelect.value;
      const svc = CONFIG.services.find(x=>x.id===svcId);
      const duration = Number(durationSelect.value || svc.duration);
      const date = dateInput.value;
      const name = $("#name").value.trim();
      const email = $("#email").value.trim();
      const phone = $("#phone").value.trim();
      const payment = $("#payment").value;
      const selectedSlot = document.querySelector(".slot.selected");
      if(!selectedSlot){ alert("Please pick an available time slot."); return; }
      const time = selectedSlot.dataset.time;

      // Build booking
      const booking = {
        id: "bk_" + Date.now(),
        serviceId: svcId,
        serviceTitle: svc.title,
        duration,
        date,
        time,
        name,
        email,
        phone,
        payment,
        createdAt: new Date().toISOString()
      };

      saveBooking(booking);
      showConfirmation(booking);
      // regenerate timeslots to block the chosen one
      generateTimeslots();
    });

    /* ========== Confirmation UI & ICS generation ========== */
    function showConfirmation(b){
      const conf = $("#confirmation");
      conf.style.display = "block";
      conf.innerHTML = "";
      const card = document.createElement("div");
      card.className = "confirm";

      const startParts = b.time.split(":").map(Number);
      const dateParts = b.date.split("-").map(Number);
      const startDate = new Date(dateParts[0], dateParts[1]-1, dateParts[2], startParts[0], startParts[1]);
      const endDate = new Date(startDate.getTime() + b.duration*60*1000);

      const humanStart = startDate.toLocaleString([], {dateStyle:"medium", timeStyle:"short"});
      const humanEnd = endDate.toLocaleTimeString([], {timeStyle:"short"});

      card.innerHTML = `
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div>
            <div style="font-weight:900">${b.serviceTitle}</div>
            <div class="muted-small">${humanStart} — ${humanEnd}</div>
            <div style="margin-top:10px;font-weight:700">Client: ${escapeHtml(b.name)}</div>
            <div class="muted-small">${escapeHtml(b.email)} ${b.phone? "· "+escapeHtml(b.phone) : ""}</div>
            <div style="margin-top:12px">Price: <strong>£${getPriceForService(b.serviceId)}</strong></div>
            <div class="muted-small" style="margin-top:8px">Payment: ${escapeHtml(b.payment)}</div>
          </div>
          <div style="text-align:right">
            <button id="downloadIcs" class="btn ghost">Download .ics</button>
            <div style="height:10px"></div>
            <button id="emailConfirm" class="btn">Email me</button>
          </div>
        </div>
        <small class="muted-small" style="display:block;margin-top:10px">A confirmation is stored in your browser. This demo doesn't send emails — use the 'Email me' button to prepare an email or integrate a backend to send automatic notifications.</small>
      `;
      conf.appendChild(card);

      // download ics handler
      $("#downloadIcs").addEventListener("click", ()=>{
        const ics = createICS({
          start: startDate,
          end: endDate,
          title: b.serviceTitle + " — LT Performance Recovery",
          description: `Appointment for ${b.name}. Contact: ${b.email}${b.phone? " · "+b.phone : ""}`,
          location: "LT Performance Studio — 12 Recovery Lane, Cityville",
          uid: b.id
        });
        downloadData(ics, `${b.serviceTitle.replace(/\s+/g,"_")}_${b.date}_${b.time}.ics`, 'text/calendar;charset=utf-8');
      });

      $("#emailConfirm").addEventListener("click", ()=>{
        const subj = encodeURIComponent(`Booking confirmation — ${b.serviceTitle} on ${b.date} at ${b.time}`);
        const body = encodeURIComponent(`Hi ${b.name},

This is your booking confirmation.

Service: ${b.serviceTitle}
Date: ${b.date} at ${b.time}
Duration: ${b.duration} minutes
Price: £${getPriceForService(b.serviceId)}

Location:
LT Performance Studio
12 Recovery Lane, Cityville

If you need to change or cancel, reply to this email: ${CONFIG.adminEmail}

Thanks,
LT Performance Recovery
`);
        window.location.href = `mailto:${b.email}?subject=${subj}&body=${body}`;
      });

      // scroll into view
      conf.scrollIntoView({behavior:"smooth"});
    }

    function getPriceForService(id){
      const s = CONFIG.services.find(x=>x.id===id);
      return s ? s.price : "—";
    }

    function escapeHtml(s){
      return (s || "").replace(/[&<>"']/g, function(m){ return {'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[m] });
    }

    function createICS({start, end, title, description, location, uid}){
      function fmtDate(d){
        // YYYYMMDDTHHMMSSZ (UTC)
        const z = new Date(d.getTime() - d.getTimezoneOffset()*60000).toISOString().replace(/[-:]/g,'').split('.')[0] + "Z";
        return z;
      }
      const lines = [
        "BEGIN:VCALENDAR",
        "VERSION:2.0",
        "PRODID:-//LT PERFORMANCE RECOVERY//EN",
        "CALSCALE:GREGORIAN",
        "METHOD:REQUEST",
        "BEGIN:VEVENT",
        `UID:${uid}`,
        `DTSTAMP:${fmtDate(new Date())}`,
        `DTSTART:${fmtDate(start)}`,
        `DTEND:${fmtDate(end)}`,
        `SUMMARY:${title}`,
        `DESCRIPTION:${(description || "").replace(/\n/g,'\\n')}`,
        `LOCATION:${location || ""}`,
        "END:VEVENT",
        "END:VCALENDAR"
      ];
      return lines.join("\\r\\n");
    }

    function downloadData(data, filename, mime){
      const blob = new Blob([data], {type: mime});
      const url = URL.createObjectURL(blob);
      const a = document.createElement("a");
      a.href = url; a.download = filename;
      document.body.appendChild(a);
      a.click();
      a.remove();
      URL.revokeObjectURL(url);
    }

    /* ========== Initialize page ========== */
    (function init(){
      // inject service select options done above
      populateDurationForSelected();
      // default: pick today and generate slots
      generateTimeslots();
      // regenerate when date or duration changes
      dateInput.addEventListener("change", generateTimeslots);
      durationSelect.addEventListener("change", generateTimeslots);

      // initial date list includes today — for demonstration we pre-load a sample booking
      // ADMIN: uncomment the following to seed a sample booking for testing:
      /*
      saveBooking({
        id: "seed1",
        serviceId: CONFIG.services[0].id,
        serviceTitle: CONFIG.services[0].title,
        duration: CONFIG.services[0].duration,
        date: isoToday,
        time: "11:00",
        name: "Test User",
        email: "test@example.com",
        phone: "",
        payment: "pay_on_site",
        createdAt: new Date().toISOString()
      });
      generateTimeslots();
      */
    })();

    /* ========== Small convenience: show today's available slots on load ========== */
    window.addEventListener("load", ()=>{
      generateTimeslots();
    });

    /* ===========================
       Notes / Next steps for real deployment
       - Replace localStorage persistence with a secure backend (Node/Express, Firebase, Supabase, etc.)
       - Add server-side availability checks to avoid race conditions
       - Integrate Stripe Checkout / PayPal for online payments (server-side)
       - Send real email/SMS confirmations: use SendGrid/Twilio/SES from your backend
       - Consider using a calendar API (Google Calendar) for two-way syncing
       =========================== */
  </script>
</body>
</html>
