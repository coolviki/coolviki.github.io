---
layout: default
title: "AI running coach prompt: am I ready for my first half marathon?"
description: "The exact prompt I used with Claude and my Garmin data, six weeks before my first 21K, to get a brutally honest readiness check."
permalink: /prompts/ai-running-coach/
---
<article class="post">
    <header class="post-header">
        <a class="post-back" href="{{ '/blog/' | relative_url }}">← All writing</a>
        <h1 class="post-title">AI running coach prompt</h1>
        <p class="post-meta">The exact prompt behind <a href="{{ '/blog/my-first-21k-and-what-it-taught-me/' | relative_url }}"><em>My first 21K and what it taught me</em></a></p>
    </header>

<div class="post-content" markdown="1">

On 5 September 2026, six weeks before my first half marathon, I gave this prompt to my AI coach (Claude), which had access to my real Garmin data. I asked it not to flatter me, and it didn't.

## Before you use it

This prompt calls Garmin tools by name (`get_activities`, `get_hrv_trend` and so on), so it only works when your AI assistant is connected to your Garmin account. I used the open-source **[garmin_mcp](https://github.com/Taxuspt/garmin_mcp)** server, connected to Claude Desktop.

If you paste it into a plain chat with no Garmin connection, the assistant won't be able to pull your data. The prompt tells it to say so rather than guess.

**To adapt it:** change the race name, race date, today's date, weeks out and distance to match your own race.

## The prompt

<div class="prompt-block">
<button class="copy-btn" type="button" data-target="coach-prompt">Copy</button>
<pre id="coach-prompt">You are my running coach. I'm running the Vedanta Delhi Half Marathon on Sunday 18 October 2026 — my first 21k. Today is 5 September, so 6 weeks out. Pull my Garmin data and assess where I actually stand:

1. get_activities for the last 16 weeks. For each running week, give me: total km, number of runs, longest run, and average pace.
2. get_training_load_trend for 8 weeks — CTL, ATL, TSB.
3. get_hrv_trend and get_sleep_summary_range for 4 weeks.
4. get_training_status and get_vo2max_trend.
5. get_race_predictions.
6. get_activity plus get_activity_splits on my three longest recent runs — check HR drift from first half to second half (aerobic decoupling).

Then tell me, bluntly:

A. VERDICT — pick one and justify with numbers:
   - Ready to race a time goal
   - Ready to finish comfortably
   - Ready to finish with a run/walk strategy
   - Not ready; 21k on 18 Oct carries real injury risk

B. THE NUMBERS THAT DECIDE IT — my longest run to date, my 4-week average weekly volume, my consistency (runs/week), and how long I've been running consistently. Compare each against what a first-time half marathoner needs 6 weeks out.

C. RISK FLAGS — ramp rate above 10%/week, HRV trending down, chronic sleep debt, aerobic decoupling above 5%, any TSB below -30.

D. REALISTIC FINISH TIME — a range, not a point estimate, with the assumptions behind it.

Rules: use only real data from the tools. If a metric is missing or the history is too short, say so rather than estimating. Don't flatter me — if the honest answer is that I should target a 10k instead, say that.</pre>
</div>

## What I got back

> Ready to finish with a run/walk strategy. You are at the **bottom** of this band, not the top.

Six weeks later, I finished in **3:02:13**.

- [Read the full readiness assessment and 6-week plan (PDF)](/assets/files/half-marathon-readiness-and-6-week-plan.pdf)
- [Read the post-race report card (PDF)](/assets/files/half-marathon-6-week-training-report-card.pdf)

## Glossary

| Term | What it means |
|---|---|
| **CTL** | Chronic Training Load: your fitness, roughly a 6-week rolling average of training stress |
| **ATL** | Acute Training Load: your fatigue, roughly a 7-day rolling average |
| **TSB** | Training Stress Balance (CTL − ATL): your form. Very negative means overreached |
| **HRV** | Heart Rate Variability: a recovery signal. A falling trend can mean accumulated fatigue |
| **Aerobic decoupling** | How much your heart rate drifts upward in the second half of a steady run. Under 5% suggests a solid aerobic base |

</div>

    <footer class="post-footer">
        <p class="post-disclaimer">Not medical advice. Check with a doctor before ramping up your training.</p>
        <a class="post-back" href="{{ '/blog/' | relative_url }}">← All writing</a>
    </footer>
</article>

<script>
document.querySelectorAll('.copy-btn').forEach(function (btn) {
    btn.addEventListener('click', function () {
        var text = document.getElementById(btn.dataset.target).innerText;
        var done = function () {
            btn.textContent = 'Copied';
            setTimeout(function () { btn.textContent = 'Copy'; }, 2000);
        };
        if (navigator.clipboard && navigator.clipboard.writeText) {
            navigator.clipboard.writeText(text).then(done, function () { btn.textContent = 'Select & copy'; });
        } else {
            btn.textContent = 'Select & copy';
        }
    });
});
</script>
