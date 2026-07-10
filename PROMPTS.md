# assignment-1

My PROMPT-
"Act as a Senior Web Developer, I am working on a site named "DevConf2026" and created a full layout of the site and implemented it with HTML and CSS and JavaScript is not required for it. So after creating the site, I feel a missing of a section to make it more interesting. Could you give me the code for creating the Journey Roadmap section?
That must require-

1. Relevance to the site
2. Useful for the reader
3. Not much complex or easy layout
4. Great thinking"

ChatGPT-
That's a great addition for a DevConf website. However, the design you're describing (interactive timeline with elegant hover animations) is quite substantial—it will easily exceed the maximum response length I can generate in a single message.

# Part 1 — Developer Journey Timeline (HTML)

Developer Journey Timeline
==============================

<!--========================================
  Developer Journey Timeline [AI GENERATED]
============================================ -->

<section class="timeline-section">
        <div class="heading">
          <span>Developer Journey</span>
          <h2>Your DevConf2026 Experience</h2>
          <p>
            Follow every step of your conference journey from registration to
            career growth.
          </p>
        </div>

        <div class="timeline">
          <div class="item left">
            <div class="dot"></div>
            <div class="content">
              <div class="badge">Step 01</div>
              <h3>📝 Register</h3>
              <p>Reserve your seat and receive your confirmation ticket.</p>
            </div>
          </div>

          <div class="item right">
            <div class="dot"></div>
            <div class="content">
              <div class="badge">Step 02</div>
              <h3>🎟️ Check-In</h3>
              <p>Collect your badge and welcome kit at the venue.</p>
            </div>
          </div>

          <div class="item left">
            <div class="dot"></div>
            <div class="content">
              <div class="badge">Step 03</div>
              <h3>🎤 Keynote Sessions</h3>
              <p>Learn from industry experts and technology leaders.</p>
            </div>
          </div>

          <div class="item right">
            <div class="dot"></div>
            <div class="content">
              <div class="badge">Step 04</div>
              <h3>💻 Workshops</h3>
              <p>Build practical skills through hands-on coding sessions.</p>
            </div>
          </div>

          <div class="item left">
            <div class="dot"></div>
            <div class="content">
              <div class="badge">Step 05</div>
              <h3>🤝 Networking</h3>
              <p>
                Meet developers, founders and recruiters from leading companies.
              </p>
            </div>
          </div>

          <div class="item right">
            <div class="dot"></div>
            <div class="content">
              <div class="badge">Step 06</div>
              <h3>🚀 Career Growth</h3>
              <p>
                Leave inspired with new knowledge, connections and
                opportunities.
              </p>
            </div>
          </div>
        </div>
</section>

# Part 2 — Developer Journey Timeline (CSS)

    Developer Journey [AI GENERATED]

=======================================

<style>
:root{
 --primary:#002efc;
 --light:#E5E7EB;
 --dark:#111827;
 --text:#6b7280;
}
*{margin:0;padding:0;box-sizing:border-box}

.timeline-section{
 max-width:1100px;
 margin:80px auto;
 padding:20px;
}
.heading{text-align:center;margin-bottom:60px}
.heading span{
 display:inline-block;padding:8px 18px;border-radius:25px;
 background:#002efc12;color:var(--primary);font-weight:bold;
}
.heading h2{font-size:42px;margin:20px 0}
.heading p{max-width:700px;margin:auto;color:var(--text);line-height:1.7}

.timeline{position:relative;padding:20px 0}
.timeline:before{
 content:"";
 position:absolute;
 left:50%;
 top:0;
 transform:translateX(-50%);
 width:4px;
 height:100%;
 background:linear-gradient(#002efc,#7ea0ff,#002efc);
 border-radius:10px;
}
.item{
 position:relative;
 width:50%;
 padding:20px 40px;
}
.item.left{left:0;text-align:right;}
.item.right{left:50%;}
.content{
 background:#fff;
 border:1px solid var(--light);
 border-radius:18px;
 padding:24px;
 position:relative;
 transition:.35s;
}
.content:hover{
 transform:translateY(-8px);
 border-color:var(--primary);
 box-shadow:0 15px 35px rgba(0,46,252,.18);
}
.dot{
 position:absolute;
 top:38px;
 width:22px;height:22px;
 background:var(--primary);
 border:5px solid #fff;
 border-radius:50%;
 box-shadow:0 0 0 5px #dbe4ff;
 z-index:2;
}
.left .dot{right:-11px;}
.right .dot{left:-11px;}
.badge{
 display:inline-block;
 background:#002efc12;
 color:var(--primary);
 padding:6px 12px;
 border-radius:20px;
 font-size:13px;
 font-weight:bold;
 margin-bottom:12px;
}
h3{margin-bottom:10px}
p{line-height:1.7;color:var(--text)}
</style>
=======================================
