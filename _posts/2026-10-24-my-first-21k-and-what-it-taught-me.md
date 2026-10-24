---
title: "My first 21K and what it taught me"
date: 2026-10-24
description: "Six weeks before my first half marathon, my AI coach said I'd finish at the bottom of the stack, if at all. Here's how the next six weeks went."
image: /assets/images/blog/21k/share.jpg
---
On 5th September 2026, six weeks before my first half-marathon, I asked my AI coach to be brutally honest, and it told me that I'd finish at the bottom of the stack, if I finished at all. This is how the next six weeks unfolded.

## The Plateau

Honestly, after my first 10K I had got into a good regime of running, never too much, never too little - just stuck with discipline for a little over 3.5 years(Disclaimer the data in this post starts May, 2025 when I got my new watch) doing about 12 km every week. But clearly things were looking too familiar, too complacent and as with anything else in your life, being too comfortable for too long is not a very comfortable position to be in.

<figure class="wide">
  <a href="{{ '/assets/images/blog/21k/plateau-69-weeks.webp' | relative_url }}" target="_blank" rel="noopener"><img src="{{ '/assets/images/blog/21k/plateau-69-weeks.webp' | relative_url }}" alt="Bar chart of weekly running distance from May 2025 to October 2026: 69 weeks hovering around a 12 km weekly average, titled "69 weeks. Never a week missed. Never a week further."" width="1400" height="824" loading="lazy" decoding="async"></a>
</figure>

The same holds true for my 25-year career. Counterintuitive as it may sound, I have enjoyed the most when things were challenging and dreaded complacency and familiarity from the bottom of my heart.

## The Goal

Things changed in June, when registrations opened for the Vedanta Delhi Half Marathon for 18th October. Hesitantly, I signed up for the 21K thinking I would figure something out closer to the date. To be honest I had less than 20% conviction that I would even turn up, forget about completing it.

But when I look back the first step is always the most difficult ever, be it your life or this race.

## The Toolkit

Almost 2 months ahead of the half-marathon I had not yet started training for the 21K, but then one fine day as I was exploring some practical application of Model Context Protocol (MCP - and yes, how can we leave AI out of anything these days) I hit upon an Open source MCP connector for my Garmin watch [here](https://github.com/Taxuspt/garmin_mcp). The setup in itself requires another blog post for another day, but this is what it looked like

<figure class="wide">
  <a href="{{ '/assets/images/blog/21k/garmin-mcp-setup.webp' | relative_url }}" target="_blank" rel="noopener"><img src="{{ '/assets/images/blog/21k/garmin-mcp-setup.webp' | relative_url }}" alt="Diagram of the setup: Garmin watch syncs to Garmin Connect; a Raspberry Pi runs garmin_mcp, and Claude Desktop on a MacBook reaches it through an SSH tunnel" width="1266" height="1036" loading="lazy" decoding="async"></a>
</figure>

Other than that a proper pair of running shoes (Adidas Evo SL), hydration kit and energy gels are things I gathered along the way.

## The Coach

5th September 2026 is the date I still remember as the turning point of my 21K journey. Barely six weeks ahead of the run, I shot my first prompt to my AI coach (it's a 40-line one, in case you are interested [here is the link to the prompt]({{ '/prompts/ai-running-coach/' | relative_url }}))

And the not so flattering response was

<figure class="wide">
  <a href="{{ '/assets/images/blog/21k/coach-verdict.webp' | relative_url }}" target="_blank" rel="noopener"><img src="{{ '/assets/images/blog/21k/coach-verdict.webp' | relative_url }}" alt="The AI coach's verdict: "Ready to finish with a run/walk strategy. You are at the bottom of this band, not the top", with a table comparing my numbers against what first-timers need six weeks out" width="1400" height="699" loading="lazy" decoding="async"></a>
</figure>

If you want to see a detailed readout of what the coach gave [here it is]({{ '/assets/files/half-marathon-readiness-and-6-week-plan.pdf' | relative_url }}) and read till the end where I get a proper score against the plan.

Sounds so much like life, where you have objectives, start the year with some gaps, build a plan and evaluate yourself at the end. But the starting point is having the "Coach" to guide you and having the grit to follow the plan. I was lucky I had both.

## The Discipline

For someone who had not run more than 10 km ever and starting the plan in humid September Delhi, the first step was simple - Following the plan which I did in most cases.

Below is what my 6 weeks training did to my plateau,

<figure class="wide">
  <a href="{{ '/assets/images/blog/21k/plateau-to-training-block.webp' | relative_url }}" target="_blank" rel="noopener"><img src="{{ '/assets/images/blog/21k/plateau-to-training-block.webp' | relative_url }}" alt="Weekly distance chart showing the 69-week plateau at about 12 km a week, then the six-week training block climbing to over 30 km a week" width="1360" height="800" loading="lazy" decoding="async"></a>
</figure>

Week over week over the next six weeks I increased my weekly mileage and stuck to a start time of around 5:30 AM despite it being a weekday or a weekend.

**Long term consistency beats short-term intensity.** And at times what we label as "Boring" boring runs, boring investment, "boring" slog gives us the maximum returns over time. I had to slow down like crazy to be able to finish the half-marathon and look at what it did to my heart rate which had to be brought down to be able to sustain a 3 hour run.

<figure class="wide">
  <a href="{{ '/assets/images/blog/21k/slower-pace-lower-heart-rate.webp' | relative_url }}" target="_blank" rel="noopener"><img src="{{ '/assets/images/blog/21k/slower-pace-lower-heart-rate.webp' | relative_url }}" alt="Two charts titled "Getting slower was the plan": average pace slowed from 7:04 to 8:48 per km after the plan began, while average heart rate fell from 154 to 148 bpm" width="1400" height="976" loading="lazy" decoding="async"></a>
</figure>

## The Race

Super excited and a little nervous. I headed off for the half-marathon on 18th October. Alarm set for 3:30 in the morning, cab at 4:15 AM in the morning, A banana for breakfast followed by gels and electrolytes in my hydration pack for the run.

While I was standing in my wave waiting to start the run, I met my ex-colleague who was a pro in running marathons and had done dozens of them over the years. The only advice he gave me was to have fun along the way. That worked, but the biggest challenge during the run was again the run/ walk strategy, resisting the temptation to outrun the runner next to you and preserving the energy for all of those 21k. On the positive side, the cool Delhi October breeze right from the gun point through Lodhi Road, the majestic India Gate, the mesmerizing Rashtrapati Bhavan, the war-memorial, back from Nizamuddin and ending the race from where we started it all "Jawaharlal Nehru Stadium" made all the 6 weeks of effort worth it.

<figure>
  <img src="{{ '/assets/images/blog/21k/race-route.webp' | relative_url }}" alt="Race route map through central Delhi with the run summary: 21.31 km in 3:00:55 at 8:29 min/km" width="828" height="1472" loading="lazy" decoding="async">
</figure>

The crowd cheering, fellow runners pumping you up "Go Vikram Go" – Yes the name on the bib now made sense – made it look a lot less challenging. Started my acceleration over the last couple of kms and ended with a negative split which in simple terms means running the second half faster than the first. So in that sense truly ended on a high.

## The Result

3 hours, 2 mins and 13 seconds for Bib# 11589 would remain etched in my memory forever. The training did help me in limiting my physical exhaustion and I definitely felt way stronger than I have ever felt after any of the 10K.

<figure>
  <img src="{{ '/assets/images/blog/21k/certificate.webp' | relative_url }}" alt="Race certificate: Vikram Kumar, bib 11589, Vedanta Delhi Half Marathon 2026, half marathon, 18 October 2026, chip time 3:02:13" width="707" height="1000" loading="lazy" decoding="async">
</figure>

I asked my AI coach to rate my 6 weeks of training and I got an overall score of A- (bad sleep + lack of strength training cost me an A+). [Here is the detailed report]({{ '/assets/files/half-marathon-6-week-training-report-card.pdf' | relative_url }}).

Any sane person looking at the result would say that I was in the bottom 10 percentile of the people who participated (which is correct), but I will still say I am in that 0.1% of the population who have been able to complete the half-marathon within the cut off time, despite the AI coach telling me 6 weeks back that I will be at the bottom of the stack, **if** I am able to complete the run.

<figure>
  <img src="{{ '/assets/images/blog/21k/finish-medal.webp' | relative_url }}" alt="Vikram smiling and holding up his finisher's medal outside Jawaharlal Nehru Stadium after the race" width="960" height="720" loading="lazy" decoding="async">
</figure>

So coming back to the title of this article, what did this 6 weeks of sweat and pain teach me ?

- Comfort is the real plateau - 69 weeks of consistent running were getting too comfortable.
- Find a coach who wouldn't flatter you - "You are at the bottom of the stack" got me started.
- Boring compounds - Running slower made me go longer.

Post doing my first 10K 4 years back I wasn't sure if I would ever attempt a 21K. Likewise post doing my 21K I am not sure if I would ever attempt a full marathon :-) .

P.S. - Except the charts being generated by Claude, everything else was written with love so ignore any typos and grammatical errors.
