---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 2
cv_pdf: /assets/pdf/mycv.pdf # you can also use external links here
#cv_format: rendercv# options: rendercv, jsonresume
description: Click on the button below to download my full CV, or view it directly on the page.
---

<div class="row" style="margin-bottom: 20px;">
  <div class="col-md-12 text-center">
    <a href="{{ '/assets/pdf/mycv.pdf' | relative_url }}" class="btn btn-sm z-depth-1" target="_blank" rel="noopener noreferrer">
      <i class="fa-solid fa-file-pdf"></i> Download PDF
    </a>
  </div>
</div>

<div class="row">
  <div class="col-md-12" style="height: 100vh; min-height: 800px;">
    <iframe src="{{ '/assets/pdf/mycv.pdf' | relative_url }}" width="100%" height="100%" style="border: none;" allow="autoplay">
      <p>It appears your web browser doesn't support embedded PDFs. 
      <a href="{{ '/assets/pdf/mycv.pdf' | relative_url }}">Click here to download the PDF file.</a></p>
    </iframe>
  </div>
</div>
<!-- Use code with caution.🔍 Why this solves the issue:layout: page: Swapping from cv to page tells Jekyll not to look for _data/cv.yml or resume.json. This cleans up all default text blocks entirely.{{ '/assets/pdf/mycv.pdf' | relative_url }}: Using Jekyll's template tags ensures that even if you use a custom domain, GitHub Pages will always calculate the exact, correct URL path to your asset folder.Responsive Height (100vh): The embedded frame matches the height of the user's browser window, giving it a premium, seamless application layout.Would you like help adjusting the width of the frame container so it aligns tightly with the width of your navigation bar, or would you like to explore forcing mobile devices to open it in a new window since phones usually don't support inline frames? -->
