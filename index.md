---
layout: default
title: Ananya Roy
---

<section class="hero-bg">
  <div class="hero">
    <img src="assets/profile.png" alt="Ananya Roy" />
    <div>
      <h1>Ananya Roy</h1>
      <p>Product Manager · 0→1 Builder · Customer-first systems</p>

      <div class="cta">
        <a href="assets/Ananya_Roy_PM_Resume.pdf" download>Download Resume</a>
        <a href="https://www.linkedin.com/in/your-link" target="_blank">LinkedIn</a>
        <a href="mailto:your@email.com">Email</a>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <h2>Selected Work</h2>

  <div class="work-stack">

    <!-- WORK CARD 1 -->
    <div class="work-card">
      <div class="work-left">
        <h3>Phone Support for DevRev</h3>
        <p>
          “We love the product — but where’s the phone line?”
        </p>
        <button onclick="openSlides(this)">View Overview</button>
        <a class="details" href="work/phone-support.html">Read case study →</a>
      </div>

      <div class="slides">
        <div class="slide active">Problem<br><small>No voice channel blocked deals</small></div>
        <div class="slide">Insight<br><small>India SMBs rely on phone-first support</small></div>
        <div class="slide">Decision<br><small>Buy vs Build → Amazon Connect</small></div>
        <div class="slide">Execution<br><small>Native voice + AI automation</small></div>
        <div class="slide">Impact<br><small>Deals unblocked + demo wow</small></div>
      </div>
    </div>

    <!-- WORK CARD 2 -->
    <div class="work-card">
      <div class="work-left">
        <h3>Abuse Detection Systems</h3>
        <p>Designing India-first trust & safety heuristics</p>
        <a class="details" href="#">Read case study →</a>
      </div>
    </div>

    <!-- HIDDEN WORK -->
    <div class="work-card hidden">
      <div class="work-left">
        <h3>Family Hub – Neobank</h3>
        <p>Designing multi-member financial controls</p>
      </div>
    </div>

    <div class="work-card hidden">
      <div class="work-left">
        <h3>AI Support Agents</h3>
        <p>Task automation & agent productivity</p>
      </div>
    </div>

  </div>

  <button id="toggleWork" onclick="toggleWork()">Show more work</button>
</section>

<script>
  function toggleWork() {
    document.querySelectorAll('.work-card.hidden').forEach(el => {
      el.classList.toggle('hidden');
    });

    const btn = document.getElementById('toggleWork');
    btn.innerText =
      btn.innerText === 'Show more work'
        ? 'Show less'
        : 'Show more work';
  }

  function openSlides(button) {
    const slides = button.closest('.work-card').querySelector('.slides');
    slides.classList.toggle('open');
  }
</script>
