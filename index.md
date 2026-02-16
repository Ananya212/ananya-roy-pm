---
layout: default
title: Ananya Roy
---

<!-- ================= HERO ================= -->

<section class="hero-bg">
  <div class="hero">
    <img src="{{ site.baseurl }}/assets/you.png" alt="Ananya Roy" />

    <div>
      <h1>Ananya Roy</h1>
      <p>
        Product Manager · 0→1 Builder · Customer-first systems
      </p>

      <div class="cta">
        <a href="{{ site.baseurl }}/assets/Ananya_Roy_PM_Resume.pdf" download>
          Download Resume
        </a>
        <a href="https://www.linkedin.com/in/your-link" target="_blank">
          LinkedIn
        </a>
        <a href="mailto:your@email.com">
          Email
        </a>
      </div>
    </div>
  </div>
</section>

<!-- ================= WORK ================= -->

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

        <button onclick="openSlides(this)">
          View overview
        </button>

        <a
          class="details"
          href="{{ site.baseurl }}/work/phone-support.html"
        >
          Read case study →
        </a>
      </div>

      <div class="slides">
        <div class="slide active">
          <strong>Problem</strong><br />
          <small>No voice channel blocked deals</small>
        </div>
        <div class="slide">
          <strong>Insight</strong><br />
          <small>India SMBs are phone-first</small>
        </div>
        <div class="slide">
          <strong>Decision</strong><br />
          <small>Build vs Buy → Amazon Connect</small>
        </div>
        <div class="slide">
          <strong>Execution</strong><br />
          <small>Native voice + AI automation</small>
        </div>
        <div class="slide">
          <strong>Impact</strong><br />
          <small>Deals unblocked + demo wow</small>
        </div>
      </div>
    </div>

    <!-- WORK CARD 2 -->
    <div class="work-card">
      <div class="work-left">
        <h3>Abuse Detection Systems</h3>
        <p>
          India-first trust & safety heuristics for scale
        </p>

        <a
          class="details"
          href="{{ site.baseurl }}/work/abuse-detection.html"
        >
          Read case study →
        </a>
      </div>
    </div>

    <!-- HIDDEN WORK CARD 3 -->
    <div class="work-card hidden">
      <div class="work-left">
        <h3>Family Hub – Neobank</h3>
        <p>
          Multi-member controls for shared finances
        </p>

        <a
          class="details"
          href="{{ site.baseurl }}/work/family-hub.html"
        >
          Read case study →
        </a>
      </div>
    </div>

    <!-- HIDDEN WORK CARD 4 -->
    <div class="work-card hidden">
      <div class="work-left">
        <h3>AI Support Agents</h3>
        <p>
          Agent productivity via workflow automation
        </p>

        <a
          class="details"
          href="{{ site.baseurl }}/ai-agents.html"
        >
          View agents →
        </a>
      </div>
    </div>

  </div>

  <button id="toggleWork" onclick="toggleWork()">
    Show more work
  </button>
</section>

<!-- ================= SCRIPTS ================= -->

<script>
  function toggleWork() {
    document
      .querySelectorAll('.work-card.hidden')
      .forEach(card => {
        card.classList.toggle('hidden');
      });

    const btn = document.getElementById('toggleWork');
    btn.innerText =
      btn.innerText === 'Show more work'
        ? 'Show less'
        : 'Show more work';
  }

  function openSlides(button) {
    const slides =
      button.closest('.work-card').querySelector('.slides');
    slides.classList.toggle('open');
  }
</script>
