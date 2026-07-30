---
layout: default
title: RetTrack
description: RetTrack tracks your purchases, return deadlines, and receipts, and reminds you before the return window closes.
permalink: /
wide: true
---

<section class="band hero">
  <div class="band-inner hero-grid">
    <div class="hero-copy">
      <h1 class="hero-title">Never miss a return window</h1>
      <p class="hero-text">RetTrack keeps your purchases, return dates, and receipts in one place, and reminds you before the deadline passes.</p>
      <a class="cta-button" href="https://apps.apple.com/app/rettrack-returns-purchases/id6775811683" target="_blank" rel="noopener">Download on the App Store</a>
      <p class="hero-note">Free to start. No account required.</p>
    </div>
    <div class="hero-visual">
      <div class="purchase-card">
        <div class="ring-wrap">
          <svg class="ring" viewBox="0 0 120 120" aria-hidden="true" focusable="false">
            <circle class="ring-track" cx="60" cy="60" r="52" />
            <circle class="ring-progress" cx="60" cy="60" r="52" />
          </svg>
          <div class="ring-label">
            <span class="ring-number">12</span>
            <span class="ring-unit">days left</span>
          </div>
        </div>
        <div class="purchase-name">Cashmere Coat</div>
        {%- assign purchased_epoch = site.time | date: '%s' | minus: 1555200 -%}
        {%- assign return_epoch = site.time | date: '%s' | plus: 1036800 -%}
        <div class="purchase-date"><span class="purchase-date-label">Purchased</span> <span id="purchase-date">{{ purchased_epoch | date: '%-d %B' }}</span></div>
        <div class="purchase-date"><span class="purchase-date-label">Returns by</span> <span id="return-date">{{ return_epoch | date: '%-d %B' }}</span></div>
        <div class="purchase-price">EUR 320</div>
      </div>
    </div>
  </div>
</section>

<section class="band" data-reveal>
  <div class="band-inner">
    <h2 class="section-title">See it in the app</h2>
    <div class="gallery">
      <img
        src="{{ '/assets/images/screenshots/track.jpg' | relative_url }}"
        alt="The RetTrack home screen listing active purchases, with a count of how many need attention and a return-by date shown on every item."
        width="720"
        height="1561"
        loading="lazy"
        decoding="async"
      >
      <img
        src="{{ '/assets/images/screenshots/details.jpg' | relative_url }}"
        alt="A purchase detail screen showing price, purchase date, return-by date and status, with rows for a saved product link, a photo and a comment."
        width="720"
        height="1561"
        loading="lazy"
        decoding="async"
      >
      <img
        src="{{ '/assets/images/screenshots/pro.jpg' | relative_url }}"
        alt="The Pro screen showing an active lifetime plan, a checklist of Pro features, and a spending insights chart."
        width="720"
        height="1561"
        loading="lazy"
        decoding="async"
      >
    </div>
  </div>
</section>

<section class="band is-raised">
  <div class="band-inner">
    <div class="statement" data-reveal>
      <h2 class="section-title">Returns are not missed on purpose</h2>
      <p class="section-text">They are missed because the deadline was never written down anywhere. The receipt is in a drawer, the shipping email is buried, and the window closes quietly. <strong>RetTrack</strong> gives every purchase a date and a reminder, so forgetting stops costing you money.</p>
    </div>
  </div>
</section>

<section class="band" data-reveal>
  <div class="band-inner">
    <h2 class="section-title">How it works</h2>
    <div class="step-grid">
      <div class="step">
        <div class="step-head">
          <span class="step-number">1</span>
          <span class="step-icon">
            <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
              <rect x="3.75" y="3.75" width="16.5" height="16.5" rx="4" />
              <path d="M12 8.5v7" />
              <path d="M8.5 12h7" />
            </svg>
          </span>
        </div>
        <h3 class="step-title">Add the purchase</h3>
        <p class="step-text">Store, price, purchase date, and return date. About ten seconds per item.</p>
      </div>
      <div class="step">
        <div class="step-head">
          <span class="step-number">2</span>
          <span class="step-icon">
            <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
              <path d="M17.75 9.25a5.75 5.75 0 0 0-11.5 0c0 4.25-1.5 5.75-1.5 5.75h14.5s-1.5-1.5-1.5-5.75z" />
              <path d="M10.25 18.5a2 2 0 0 0 3.5 0" />
            </svg>
          </span>
        </div>
        <h3 class="step-title">Get reminded</h3>
        <p class="step-text">A notification before the return window closes, not after it has passed.</p>
      </div>
      <div class="step">
        <div class="step-head">
          <span class="step-number">3</span>
          <span class="step-icon">
            <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
              <path d="M12 20.25V12" />
              <path d="M12 12 6.75 6.75" />
              <path d="M12 12l5.25-5.25" />
              <path d="M6.75 10.5V6.75h3.75" />
              <path d="M17.25 10.5V6.75h-3.75" />
            </svg>
          </span>
        </div>
        <h3 class="step-title">Decide</h3>
        <p class="step-text">Mark the item returned or kept. RetTrack keeps a running total of what you have recovered.</p>
      </div>
    </div>
  </div>
</section>

<section class="band is-raised" data-reveal>
  <div class="band-inner">
    <h2 class="section-title">What you can keep track of</h2>
    <div class="feature-grid">
      <div class="feature-card">
        <span class="icon-tile">
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <circle cx="12" cy="12" r="8.25" />
            <path d="M12 7.25V12l3.25 1.9" />
          </svg>
        </span>
        <span class="feature-title">Return deadlines</span>
        <span class="feature-text">See how many days are left at a glance.</span>
      </div>
      <div class="feature-card">
        <span class="icon-tile">
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <path d="M6.25 3.75h11.5v16.5l-2.875-1.5-2.875 1.5-2.875-1.5-2.875 1.5z" />
            <path d="M9.25 8.5h5.5" />
            <path d="M9.25 12.25h5.5" />
          </svg>
        </span>
        <span class="feature-title">Receipts and photos</span>
        <span class="feature-text">Attach proof of purchase so you are not searching for it later.</span>
      </div>
      <div class="feature-card">
        <span class="icon-tile">
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <path d="M10.6 13.4a3.4 3.4 0 0 0 4.8 0l2.6-2.6a3.4 3.4 0 0 0-4.8-4.8l-1 1" />
            <path d="M13.4 10.6a3.4 3.4 0 0 0-4.8 0L6 13.2a3.4 3.4 0 0 0 4.8 4.8l1-1" />
          </svg>
        </span>
        <span class="feature-title">Product links</span>
        <span class="feature-text">Open the original listing straight from the item.</span>
      </div>
      <div class="feature-card">
        <span class="icon-tile">
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <path d="M13.75 3.75H7.5A1.75 1.75 0 0 0 5.75 5.5v13A1.75 1.75 0 0 0 7.5 20.25h9a1.75 1.75 0 0 0 1.75-1.75V8.25z" />
            <path d="M13.75 3.75v4.5h4.5" />
            <path d="M9 13h6" />
            <path d="M9 16.25h4" />
          </svg>
        </span>
        <span class="feature-title">Notes</span>
        <span class="feature-text">Size, colour, and why you were unsure in the first place.</span>
      </div>
      <div class="feature-card">
        <span class="icon-tile">
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <rect x="3.75" y="4.75" width="16.5" height="4.5" rx="1.5" />
            <path d="M5.5 9.25v8.5a1.75 1.75 0 0 0 1.75 1.75h9.5a1.75 1.75 0 0 0 1.75-1.75v-8.5" />
            <path d="M10 13h4" />
          </svg>
        </span>
        <span class="feature-title">History</span>
        <span class="feature-text">Every completed purchase, returned or kept, in one archive.</span>
      </div>
      <div class="feature-card">
        <span class="icon-tile">
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <circle cx="12" cy="12" r="8.25" />
            <path d="M12 16.25V7.75" />
            <path d="M8.5 11.25 12 7.75l3.5 3.5" />
          </svg>
        </span>
        <span class="feature-title">Recovered total</span>
        <span class="feature-text">How much money you have actually got back.</span>
      </div>
    </div>
  </div>
</section>

<section class="band" data-reveal>
  <div class="band-inner">
    <h2 class="section-title">Free and Pro</h2>
    <div class="plan-grid">
      <div class="plan">
        <h3 class="plan-title">Free</h3>
        <p class="plan-line">Everything you need to stop missing deadlines.</p>
        <ul class="plan-list">
          <li>Add purchases and return dates.</li>
          <li>Reminders before the window closes.</li>
          <li>Mark items returned or kept.</li>
          <li>Full history of past purchases.</li>
        </ul>
      </div>
      <div class="plan is-pro">
        <span class="plan-badge">PRO</span>
        <h3 class="plan-title">RetTrack Pro</h3>
        <p class="plan-line">For people tracking more than a few things.</p>
        <ul class="plan-list">
          <li>Unlimited saved purchases.</li>
          <li>Reminders on your own schedule.</li>
          <li>Search and sort across everything.</li>
          <li>Spending insights and trends.</li>
          <li>Up to three photos per item.</li>
          <li>Export your history to CSV.</li>
        </ul>
        <p class="plan-note">Pro is available as a monthly or yearly subscription, or as a one-time Lifetime purchase.</p>
      </div>
    </div>
  </div>
</section>

<section class="band is-raised">
  <div class="band-inner">
    <div class="statement" data-reveal>
      <h2 class="section-title">Return windows, store by store</h2>
      <p class="section-text">How long do you actually have at each store, and when does the clock start counting? We keep plain-English summaries of the rules that are easy to get wrong.</p>
      <a class="cta-button is-secondary" href="{{ '/return-policies/' | relative_url }}">Browse return policies</a>
    </div>
  </div>
</section>

<section class="band" data-reveal>
  <div class="band-inner">
    <h2 class="section-title">Questions</h2>
    <div class="faq">
      <div class="faq-item">
        <h3 class="faq-question">Do I need an account?</h3>
        <p class="faq-answer">No. You can use RetTrack as a guest. Sign in only if you want your purchases to sync across devices.</p>
      </div>
      <div class="faq-item">
        <h3 class="faq-question">Is RetTrack free?</h3>
        <p class="faq-answer">Yes. Adding purchases, setting return dates, getting reminders, and keeping your history are all free. Pro adds unlimited purchases and extra tools.</p>
      </div>
      <div class="faq-item">
        <h3 class="faq-question">Which stores does it work with?</h3>
        <p class="faq-answer">All of them. RetTrack is not connected to any retailer. You enter the purchase and the return date yourself, which means no store is unsupported.</p>
      </div>
      <div class="faq-item">
        <h3 class="faq-question">What if I have already missed a deadline?</h3>
        <p class="faq-answer">Some stores are stricter than others, and a few will still help you in person. RetTrack exists so that you are not finding out on day thirty-one.</p>
      </div>
    </div>
  </div>
</section>

<section class="band is-sage closing" data-reveal>
  <div class="band-inner">
    <h2 class="closing-title">Stop losing money to forgotten returns</h2>
    <p class="closing-line">RetTrack is free to start and takes about ten seconds per purchase.</p>
    <a class="cta-button" href="https://apps.apple.com/app/rettrack-returns-purchases/id6775811683" target="_blank" rel="noopener">Download on the App Store</a>
  </div>
</section>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "RetTrack",
  "operatingSystem": "iOS",
  "applicationCategory": "ShoppingApplication",
  "description": "RetTrack tracks your purchases, return deadlines, and receipts, and reminds you before the return window closes.",
  "url": "https://apps.apple.com/app/rettrack-returns-purchases/id6775811683",
  "image": "{{ '/assets/images/rettrack-logo-mark.png' | absolute_url }}"
}
</script>
