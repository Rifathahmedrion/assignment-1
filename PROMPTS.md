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

Part 1 — Developer Journey Timeline (HTML)
=============================
Developer Journey Timeline
============================== 

<section class="journey">

    <div class="section-title">
        <span>Developer Journey</span>
        <h2>Your Experience at DevConf2026</h2>
        <p>
            Every attendee follows an exciting journey—from registration to
            becoming part of an inspiring developer community.
        </p>
    </div>
    <div class="journey-grid">
        <div class="journey-card">
            <div class="step">01</div>
            <div class="icon">
                📝
            </div>
            <h3>Register</h3>
            <p>
                Secure your seat online and receive your conference ticket
                instantly.
            </p>
        </div>
        <div class="journey-card">
            <div class="step">02</div>
            <div class="icon">
                🎟️
            </div>
            <h3>Check-In</h3>
            <p>
                Verify your ticket and receive your conference badge and welcome
                kit.
            </p>
        </div>
        <div class="journey-card">
            <div class="step">03</div>
            <div class="icon">
                🎤
            </div>
            <h3>Keynote Sessions</h3>
            <p>
                Learn from world-class speakers sharing modern development
                practices.
            </p>
        </div>
        <div class="journey-card">
            <div class="step">04</div>
            <div class="icon">
                💻
            </div>
            <h3>Hands-on Workshop</h3>
            <p>
                Participate in practical coding sessions and improve your real
                development skills.
            </p>
        </div>
        <div class="journey-card">
            <div class="step">05</div>
            <div class="icon">
                🤝
            </div>
            <h3>Networking</h3>
            <p>
                Connect with developers, recruiters, founders and open-source
                contributors.
            </p>
        </div>
        <div class="journey-card">
            <div class="step">06</div>
            <div class="icon">
                🚀
            </div>
            <h3>Grow Your Career</h3>

Part 2 — Developer Journey Timeline (CSS)
=====================================
    Developer Journey [AI GENERATED]
=======================================
<style>
:root {
    --primary: #002efc;
    --light: #e5e7eb;
    --dark: #111827;
    --white: #ffffff;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.journey {
    width: min(1200px, 92%);
    margin: 100px auto;
}

.section-title {
    text-align: center;
    margin-bottom: 70px;
}

.section-title span {
    display: inline-block;
    background: #002efc10;
    color: var(--primary);
    padding: 10px 22px;
    border-radius: 30px;
    font-weight: 600;
    letter-spacing: 0.5px;
}

.section-title h2 {
    font-size: 44px;
    margin: 22px 0;
}

.section-title p {
    max-width: 700px;
    margin: auto;
    color: #666;
    line-height: 1.8;
}

.journey-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 70px 35px;
    position: relative;
}

.journey-grid::before {
    content: "";
    position: absolute;
    top: 90px;
    left: 15%;
    width: 70%;
    height: 5px;
    background: linear-gradient(to right, #002efc, #8aa4ff, #002efc);
    z-index: -1;
    border-radius: 20px;
}

.journey-card {
    background: white;
    border: 1px solid var(--light);
    border-radius: 22px;
    padding: 45px 30px;
    position: relative;
    transition: 0.45s;
    overflow: hidden;
    cursor: pointer;
}

.journey-card::before {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, rgba(0, 46, 252, 0.08), transparent);
    opacity: 0;
    transition: 0.4s;
}

.journey-card:hover::before {
    opacity: 1;
}

.journey-card:hover {
    transform: translateY(-12px);
    border-color: #002efc;
    box-shadow: 0 18px 40px rgba(0, 46, 252, 0.18);
}

.step {
    position: absolute;
    right: 20px;
    top: 20px;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: #002efc;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 700;
    transition: 0.4s;
}

.journey-card:hover .step {
    transform: rotate(360deg);
}

.icon {
    width: 80px;
    height: 80px;
    background: #002efc12;
    color: #002efc;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 18px;
    font-size: 40px;
    margin-bottom: 28px;
    transition: 0.45s;
}

.journey-card:hover .icon {
    background: #002efc;
    color: white;
    transform: scale(1.08) rotate(-6deg);
}

.journey-card h3 {
    font-size: 24px;
    margin-bottom: 18px;
}

.journey-card p {
    color: #666;
    line-height: 1.8;
}
</style>