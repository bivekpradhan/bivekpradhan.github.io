---
layout: post
title: "My Ph.D Work Explanation"
date: 2026-09-23 00:00:00
description: A beginner-friendly, interactive walkthrough of my PhD research on compressible MHD waves, nonlinear coupling, and turbulence in the solar corona.
tags: solar-physics MHD turbulence research
categories: research
giscus_comments: true
related_posts: false
toc:
  sidebar: left
---

The visible surface of the Sun is roughly 5,500&nbsp;°C, yet its outer
atmosphere — the corona — reaches temperatures of a million degrees or
more. Explaining that jump is one of the open problems in solar
physics, and it's the question at the heart of my PhD research:
**how does compressibility alter the nonlinear evolution of Alfvénic
disturbances and the resulting turbulent energy transfer relevant to
solar coronal heating?**

The interactive explainer below walks through the mystery, the
physics of Alfvén waves, the mechanism I study, how organized waves
transition into turbulence, the numerical MHD setup I use (PLUTO
code), and closes with a short self-check quiz.

<div class="l-page">
  <iframe
    id="corona-explainer-frame"
    src="{{ '/assets/html/solar-corona-explainer.html' | relative_url }}"
    title="Interactive explainer: How Can Waves Heat the Solar Corona?"
    style="width: 100%; height: 900px; border: 1px solid var(--global-divider-color, #ddd); border-radius: 12px;"
    loading="lazy">
  </iframe>
</div>

<script>
  (function () {
    var frame = document.getElementById('corona-explainer-frame');
    if (!frame) return;

    function resizeFrame() {
      try {
        var doc = frame.contentWindow.document;
        var height = doc.documentElement.scrollHeight || doc.body.scrollHeight;
        if (height) {
          frame.style.height = (height + 20) + 'px';
        }
      } catch (e) {
        // Cross-origin or not yet loaded — keep the default height.
      }
    }

    frame.addEventListener('load', function () {
      resizeFrame();
      // The page's own tab-switching changes content height without
      // firing a resize event, so poll briefly after each load.
      var ticks = 0;
      var interval = setInterval(function () {
        resizeFrame();
        ticks += 1;
        if (ticks > 40) clearInterval(interval); // ~20s safety cutoff
      }, 500);
    });
  })();
</script>

*If the embedded panel doesn't load, you can also
[open the explainer directly]({{ '/assets/html/solar-corona-explainer.html' | relative_url }}).*
