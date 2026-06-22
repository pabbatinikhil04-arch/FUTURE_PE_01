# AI Website Copy Generator — Vivekananda Spoken English Academy (T. Nagar, Chennai)

**Future Interns — Prompt Engineering Task 1 (2026)**

---

## Business Chosen

**Vivekananda Spoken English Academy**
No. 9, Madley Road, T. Nagar, near Madley Subway, Chennai – 600017

This is a **real, currently operating coaching institute** in T. Nagar,
Chennai, found via public business listings. It teaches spoken English,
grammar, personality development, and interview/business communication
skills, with multilingual (Hindi-to-English) trainers, free demo classes,
and air-conditioned classrooms open all seven days a week.

I chose this business specifically because:
- Local coaching institutes like this rarely have website copy that's
  actually written to address the customer's real hesitation (the fear of
  *speaking*, not a lack of vocabulary) — most just list course names.
- Its real, verifiable details (bilingual teaching, 7-day scheduling,
  free demo classes) gave me genuine differentiators to write from, instead
  of inventing fake stats — which is the actual skill this task is testing.

> **Note on accuracy:** All business facts used in this copy (location,
> course list, teaching methodology, trainer language support, working
> hours, demo class policy) were sourced from public business directory
> listings, not invented. No fee amounts, founding year, or placement
> guarantees are stated anywhere in this copy, because those weren't
> reliably confirmed — the brief explicitly flags this so the AI doesn't
> fabricate them (see `prompts/00_business_brief.md`).

---

## Tool Used

**Claude** (claude.ai) — used to design the reusable prompt framework and
generate all final copy.

---

## Repository Structure

```
website-copy-project/
├── prompts/
│   ├── 00_master_system_prompt.md     → reusable core prompt (works for ANY local business)
│   ├── 00_business_brief.md           → this client's intake data
│   ├── 01_homepage_prompt.md          → generates headline, sub-headline, intro
│   ├── 02_services_prompt.md          → generates per-service descriptions
│   ├── 03_cta_prompt.md               → generates 3 distinct CTA sections
│   └── 04_tone_adaptation_prompt.md   → proves the system works across tones/business types
├── outputs/
│   ├── 01_homepage_copy.md            → final generated homepage copy
│   ├── 02_services_copy.md            → final generated services page copy
│   ├── 03_cta_copy.md                 → final generated CTA sections
│   └── 04_tone_adaptation_demo.md     → side-by-side tone comparison
└── README.md
```

---

## Prompt Logic

The system is split into two layers so it's **reusable for other clients**,
not a one-off script:

1. **Master System Prompt** (`00_master_system_prompt.md`) — fixed rules
   that apply to *any* local business: no AI-sounding filler words, every
   section needs one concrete specific detail, match the stated tone
   exactly, never fabricate stats — write a placeholder instead.

2. **Business Brief** (`00_business_brief.md`) — the only thing that
   changes per client. It's structured like a real client intake form:
   business name, location, services, customer, tone, real differentiators,
   and explicit constraints on what *not* to claim.

3. **Task prompts** (`01`–`04`) sit on top of both and ask for one specific
   deliverable each — homepage, services, CTAs, tone variants — with exact
   structural rules (word counts, sentence counts, what each sentence must
   do) so the output is consistently scannable and ready to drop into a real
   webpage, not a wall of generic paragraphs.

To reuse this for a different business (a salon, a clinic, a cafe): keep
`00_master_system_prompt.md` exactly as is, replace `00_business_brief.md`
with the new client's details, and re-run prompts `01`–`03`.

---

## Key Features Demonstrated

- ✅ Clear, benefit-driven copy — every section names a specific customer
  frustration before offering the solution
- ✅ Business-specific language — uses Vivekananda Academy's actual
  differentiators (bilingual trainers, 7-day scheduling, free demo class),
  not generic "best in class" filler
- ✅ Strong, honest CTAs — booking, trust-building, and location-based,
  with no fabricated urgency or fake stats
- ✅ Reusable prompt structure — proven via the tone-adaptation output,
  which shows the same logic producing different results for a salon-style
  friendly tone vs. a clinic-style professional tone
- ✅ Ready-to-publish copy — word counts and structure are built for direct
  use on a real homepage/services page, not just a brainstorm

---

## Learn & Earn Note

Next step per the task brief: share this copy with the actual academy,
walk them through how it's clearer than what's likely on their current
listing pages, and offer to help set it up on a real site (e.g. via
Lovable or Framer AI) as a small paid engagement.
