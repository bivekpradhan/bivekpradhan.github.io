---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 2
cv_pdf: /assets/pdf/mycv.pdf # you can also use external links here
#cv_format: rendercv # options: rendercv, jsonresume
description: Click on the button below to download my full CV, or view it directly on the page.
---

<style>
  .cv-download-row { margin-bottom: 1.25rem; text-align: center; }
  .cv-download-row .btn { padding: 0.55rem 1.4rem; font-size: 1rem; }

  .cv-viewer {
    width: 100%;
    height: 100vh;
    min-height: 800px;
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    overflow: hidden;
  }
  .cv-viewer iframe { width: 100%; height: 100%; border: none; display: block; }

  /* Mobile fallback card, hidden by default, shown instead of the iframe on small/touch screens */
  .cv-mobile-fallback {
    display: none;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 0.75rem;
    height: 100%;
    padding: 2rem 1.25rem;
    text-align: center;
  }
  .cv-mobile-fallback i { font-size: 2.5rem; color: var(--global-theme-color); }
  .cv-mobile-fallback p { margin: 0; max-width: 32ch; line-height: 1.6; }

  @media (max-width: 768px) {
    .cv-viewer { height: 70vh; min-height: 420px; }
    .cv-viewer iframe { display: none; }
    .cv-mobile-fallback { display: flex; }
    .cv-download-row .btn { width: 100%; max-width: 320px; }
  }
</style>

<div class="row cv-download-row">
  <div class="col-md-12">
    <a href="{{ '/assets/pdf/mycv.pdf' | relative_url }}" class="btn btn-sm z-depth-1" target="_blank" rel="noopener noreferrer">
      <i class="fa-solid fa-file-pdf"></i> Download PDF
    </a>
  </div>
</div>

<div class="row">
  <div class="col-md-12">
    <div class="cv-viewer">
      <iframe src="{{ '/assets/pdf/mycv.pdf' | relative_url }}" allow="autoplay">
        <p>It appears your web browser doesn't support embedded PDFs.
        <a href="{{ '/assets/pdf/mycv.pdf' | relative_url }}">Click here to download the PDF file.</a></p>
      </iframe>

      <!-- Shown on phones/small screens instead of the iframe, since most mobile
           browsers can't render an embedded PDF reliably -->
      <div class="cv-mobile-fallback">
        <i class="fa-solid fa-file-pdf" aria-hidden="true"></i>
        <p>Inline PDF preview isn't well supported on mobile browsers.</p>
        <a href="{{ '/assets/pdf/mycv.pdf' | relative_url }}" class="btn btn-sm z-depth-1" target="_blank" rel="noopener noreferrer">
          <i class="fa-solid fa-up-right-from-square"></i> Open CV in new tab
        </a>
      </div>
    </div>
  </div>
</div>
