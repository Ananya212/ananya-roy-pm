---
layout: default
title: Ananya Roy
---

<!-- ================= HERO ================= -->

<section class="hero-bg">
  <div class="hero">
    <img src="{{ site.baseurl }}/assets/images/you.png" alt="Ananya Roy" />

    <div>
      <h1>Ananya Roy</h1>
      <p>Product Manager · 0→1 Builder · Customer-first systems</p>

      <div class="cta">
        <a href="{{ site.baseurl }}/assets/Ananya_Roy_PM_Resume.pdf" download>
          Download Resume
        </a>
        <a href="https://www.linkedin.com/in/your-link" target="_blank">
          LinkedIn
        </a>
        <a href="mailto:your@email.com">Email</a>
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
        <p>“We love the product — but where’s the phone line?”</p>

        <button onclick="openSlides(this)">View overview</button>

        <a
          class="details"
          href="{{ site.baseurl }}/work/phone-support.html"
        >
          Read case study →
        </a>
      </div>

      <div class="slides">
        <div class="slide"><strong>Problem</strong><br>Voice missing</div>
        <div class="slide"><strong>Insight</strong><br>India = phone-first</div>
        <div class="slide"><strong>Decision</strong><br>Buy vs Build</div>
        <div class="slide"><strong>Execution</strong><br>Amazon Connect</div>
        <div class="slide"><strong>Impact</strong><br>Deals unblocked</div>
      </div>
    </div>

    <!-- WORK CARD 2 -->
    <div class="work-card">
      <div class="work-left">
        <h3>Abuse Detection Systems</h3>
        <p>India-first trust & safety heuristics</p>

        <a
          class="details"
          href="{{ site.baseurl }}/work/abuse-detection.html"
        >
          Read case study →
        </a>
      </div>
    </div>

    <!-- HIDDEN WORK -->
    <div class="work-card hidden">
      <div class="work-left">
        <h3>Family Hub – Neobank</h3>
        <p>Multi-member financial controls</p>

        <a
          class="details"
          href="{{ site.baseurl }}/work/family-hub.html"
        >
          Read case study →
        </a>
      </div>
    </div>

    <div class="work-card hidden">
      <div class="work-left">
        <h3>AI Support Agents</h3>
        <p>Agent productivity automation</p>

        <a
          class="details"
          href="{{ site.baseurl }}/ai-agents.html"
        >
          View agents →
        </a>
      </div>
    </div>

  </div>

  <button id="toggleWork" onclick="toggleWork()">Show more work</button>
</section>

<!-- ================= CASE STUDIES ================= -->

<section class="section secondary">
  <h2>More Case Studies</h2>

  <div class="mini-cards">
    <a class="mini-card" href="{{ site.baseurl }}/work/phone-support.html">
      <h4>Phone Support</h4>
      <p>0→1 voice channel</p>
    </a>

    <a class="mini-card" href="{{ site.baseurl }}/work/abuse-detection.html">
      <h4>Abuse Detection</h4>
      <p>Trust & safety systems</p>
    </a>

    <a class="mini-card" href="{{ site.baseurl }}/work/family-hub.html">
      <h4>Family Hub</h4>
      <p>Neobank controls</p>
    </a>
  </div>
</section>

<!-- ================= AI AGENTS ================= -->

<section class="section secondary">
  <h2>AI Agents</h2>

  <div class="mini-cards">
    <a class="mini-card" href="{{ site.baseurl }}/ai-agents.html">
      <h4>Support Agent</h4>
      <p>Ticket + call automation</p>
    </a>

    <a class="mini-card" href="{{ site.baseurl }}/ai-agents.html">
      <h4>Moderation Agent</h4>
      <p>Abuse triage</p>
    </a>

    <a class="mini-card" href="{{ site.baseurl }}/ai-agents.html">
      <h4>Ops Agent</h4>
      <p>Workflow routing</p>
    </a>
  </div>
</section>

<!-- ================= SCRIPTS ================= -->

<script>
  function toggleWork() {
    document.querySelectorAll('.work-card.hidden').forEach(card => {
      card.classList.toggle('hidden');
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
