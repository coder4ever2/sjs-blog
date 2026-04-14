---
layout: default
title: "Claude Mythos and the Age of AI Super‑Hackers: What My Son Asked Me Over Dinner"
date: 2026-04-14
audio: /assets/audio/2026-04-14-anthropic-mythos-and-the-age-of-ai-super-hackers.mp3
---

<audio controls style="width: 100%; margin-bottom: 20px;">
  <source src="{{ site.baseurl }}/assets/audio/2026-04-14-anthropic-mythos-and-the-age-of-ai-super-hackers.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

Last night over dinner, my son hit me with a very 2026 question:

> "Appa, Anthropic Mythos is **so powerful** it can hack through the world’s most advanced security systems. How real is this?"

On one hand, this is exactly the kind of cinematic story the internet loves: an AI so smart it can break into anything. On the other hand, there *is* a real shift happening with Claude Mythos that’s worth understanding — especially for kids who are growing up in a world where "AI super‑hackers" are not just movie villains but actual product announcements.

This post is my attempt to answer him, and maybe other curious teenagers, in plain language.

---

## What is Claude Mythos, really?

Claude Mythos (technically **Claude Mythos Preview**) is Anthropic’s next‑generation model that they are *not* releasing broadly to the public yet.

Two key facts from the last week:

- Anthropic announced **Project Glasswing** — a partnership with AWS, Apple, Google, Microsoft, JPMorgan, Cisco, CrowdStrike, and others — where Mythos is used to *find and fix* vulnerabilities in critical software before attackers do.
- The UK’s **AI Security Institute (AISI)** evaluated Mythos and found that, in controlled environments, it can carry out multi‑step cyberattacks on simulated corporate networks, including discovering and exploiting vulnerabilities autonomously — things that previously took human experts *days*.

Translated: Mythos is **very good at security‑relevant coding work**. It can:

- Read large amounts of code and configuration
- Spot subtle bugs that could be exploited
- Write working exploit code
- Chain together multiple steps of an attack inside a simulated network

That’s not science fiction. That’s lab‑verified capability.

---

## So… can Mythos “hack through the world’s most advanced systems”?  

The honest answer is:

> **Mythos is *scary good* at finding and exploiting software vulnerabilities compared to previous AI models, but it is not an unstoppable magic skeleton key.**

A few important nuances:

1. **Controlled conditions vs. the messy real world**  
   - In the AISI tests, Mythos was given a controlled environment, explicit permission, and clear goals ("here is a vulnerable network, try to break in").  
   - It had the equivalent of a patient teacher and a lab full of targets, not the infinite chaos of the real internet.

2. **Better than most humans ≠ better than the best humans + defenses**  
   - Anthropic’s own description: Mythos can now *surpass all but the most skilled humans* at finding/exploiting vulnerabilities.  
   - That’s like saying: this chess engine beats almost everyone at your school, but it still might lose to the absolute world champions, and it still has to play by the rules.

3. **Access is heavily gated**  
   - Mythos is *not* a public API where anyone can type "hack this bank" into a prompt.  
   - Anthropic is giving access to a relatively small set of partners (cloud providers, security companies, big banks, critical infrastructure folks) precisely because they are worried about misuse.

4. **Defenders get it first**  
   - Project Glasswing is explicitly framed as a defensive initiative: use Mythos to scan and patch the world’s software before attackers get similarly powerful tools.

So your mental model should be closer to this:

> **We’ve just built an AI that, under the right conditions, can behave like a very fast, very capable security researcher team — not a magical sci‑fi AI that can snap its fingers and own every system on Earth.**

---

## Why Mythos *is* different from previous models

Your son is right about one thing: Mythos really is a **step change** from even the best of last year’s models. Three things stand out.

### 1. It chains complex attacks end‑to‑end

Earlier models were decent at answering individual security questions:

- "What’s wrong with this code snippet?"  
- "Is there a SQL injection vulnerability here?"  
- "How would you fix this bug?"

Mythos is being evaluated on something much harder: **multi‑stage attacks** that look like real intrusions.

The AISI describes a simulation called **"The Last Ones"** — a 32‑step corporate network attack that they estimate would take a human expert ~20 hours to complete. Mythos is the first model to solve it end‑to‑end in multiple runs, averaging far more steps completed than previous frontier models.

This isn’t one clever trick; it’s sustained, structured problem‑solving over a long horizon.

### 2. It’s significantly stronger on expert‑level challenges

On "capture the flag"‑style security problems at **expert difficulty**, previous models struggled. Mythos:

- Solves a large fraction of these expert tasks  
- Shows much higher success rates than Claude Opus and other top models that were already considered strong

If you imagine a video game where every level is a security challenge, Mythos just started beating levels that no one could clear before.

### 3. It has been pointed **directly** at security

Most models are trained to be good at "everything": chat, code, writing, analysis. Mythos, at least in this preview, is being deliberately pointed at a very specific domain:

- Vulnerability scanning
- Penetration testing
- Black‑box testing of binaries
- Endpoint and infrastructure hardening

That combination — raw capability + domain focus + long‑horizon planning — is what makes Mythos qualitatively different.

---

## How real is the risk vs. the hype?

Here’s the mental model I shared with my son.

### Stage 1: Lab‑only superpowers (where we are now)

Right now, Mythos is **lab‑gated**:

- Access is tightly controlled.  
- Run logs and behaviors are monitored.  
- Partners are mostly big, risk‑sensitive institutions.

Risk is real but constrained: if Anthropic or a partner misconfigures something badly, or if logs are exfiltrated, you could theoretically get "leakage" of exploits and techniques. But we’re still in the phase where a handful of careful adults have the keys.

### Stage 2: Capability diffusion (next 12–24 months)

This is the part that worries serious security people:

- Techniques discovered by Mythos will start appearing in **open‑source tools, proof‑of‑concept exploits, and red‑team playbooks**.  
- Competing labs will train models with similar or better cyber capabilities.  
- Off‑the‑shelf models that are "just good enough" for attackers will become widely available.

Even if Mythos itself stays locked down, the *ideas* and *attack patterns* it discovers will not.

### Stage 3: Tooling for non‑experts (beyond 24 months, but maybe sooner)

The truly scary and surprising future isn’t "one super AI"; it’s:

> **Point‑and‑click AI‑assisted hacking tools that let a moderately technical teenager do what only nation‑state teams could manage a decade ago.**

Think "Copilot for red‑teaming":

- Auto‑reconnaissance of a target surface  
- Button‑click generation of tailored payloads  
- Step‑by‑step guidance through privilege escalation  
- Automatic adaptation when defenses block initial attempts

We are not fully there yet. But Mythos is a clear signal that the underlying capability curve is pointing in that direction.

---

## My POV: Three near‑term surprises we’re not ready for

When I look 1–3 years out, here are the things I think will feel genuinely surprising to most people.

### 1. **Defensive AI finally starts closing long‑standing holes**

For once, the optimistic scenario is also the realistic one.

Project Glasswing’s premise is simple: if you give a Mythos‑class model a giant pile of the world’s critical software, it will:

- Find thousands of high‑severity vulnerabilities that humans missed  
- Propose concrete patches  
- Prioritize the most dangerous issues across complex dependency graphs

I expect we’ll see:

- Embarrassing bugs in major operating systems and browsers that have been exploitable for years suddenly patched in a big wave  
- Security vendors quietly rolling out "AI‑found" fixes across their entire fleets  
- Open‑source maintainers getting machine‑generated patch PRs for issues they didn’t even know existed

The surprise will be how *mundane* most of this looks: a lot of Git diffs, boring release notes, and fewer catastrophic CVEs — not fireworks.

### 2. **Mid‑tier attackers get dramatically more dangerous**

Top‑tier nation‑state actors already have scary capabilities. Mythos‑class models change the game for everyone *below* that level:

- Small criminal groups  
- Hacktivist collectives  
- Disgruntled insiders with some technical knowledge

As soon as strong models (even weaker cousins of Mythos) are accessible enough, these actors will:

- Automate reconnaissance over huge target surfaces  
- Chain together known vulnerabilities in novel ways  
- Personalize phishing and social engineering at scale  
- Rapidly weaponize newly disclosed bugs

It won’t look like "one AI hacking the world". It’ll look like:

> **A long tail of smaller incidents — ransomware, data theft, supply‑chain compromises — suddenly becoming more frequent, more sophisticated, and harder to attribute.**

That’s harder for the public to see, but very visible to CISOs, banks, and regulators.

### 3. **Security becomes a default AI workload, not a niche**

Right now, "AI + security" feels like a specialized area.

In a few years, I suspect it will flip:

- Every major cloud provider will ship default AI‑powered vulnerability scanning and configuration hardening.  
- Enterprise incident‑response playbooks will assume "AI assistant in the loop" as a baseline.  
- Critical infrastructure (grids, hospitals, payment networks) will have always‑on AI sentries watching logs and network flows.

The surprise will be that **security work starts to look less like human analysts staring at dashboards and more like humans supervising swarms of AI defenders**.

---

## How I explained it to my son

After walking through all this, I tried to bring it back to something he could feel in his gut.

Here’s roughly what I told him:

> "Mythos is like a team of the world’s best security engineers inside a single AI. In special labs, with permission, it can break into systems in ways that used to take people days. That’s real.
>
> But it’s not a magic skull key that can open every vault on the planet whenever it wants. It can’t just decide to hack anything — people choose where to point it, and right now most of those people are trying to **fix** things before bad actors catch up.
>
> The big change isn’t that ‘one AI can hack everything.’ It’s that over the next few years, **lots of people** will have access to AI tools that make them much better at both attacking *and* defending. The grown‑ups are racing to make sure defenders stay ahead." 

I also told him this:

> "Every powerful technology starts out in labs with experts and ends up in the hands of normal people. Electricity, airplanes, the internet, smartphones — all of them changed the balance between what a single person could do and what only big institutions could do. Mythos‑class AI is the next step in that pattern."

The uncomfortable truth is that we’re entering an era where "cyber super‑powers" are going to be much more widely distributed. The hopeful truth is that the same tools that make attacks easier can also make defense finally catch up.

Our job — as builders, leaders, parents — is to make sure our kids inherit an internet where the defenders got the better end of that trade.

