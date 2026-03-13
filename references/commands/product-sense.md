# Product Sense Interview Practice — Command Reference

## Purpose

Dedicated practice module for FAANG/Meta/Google-style **Product Sense** interviews. This is NOT the same as a behavioral interview about past product decisions — it's a live, structured thinking exercise where the candidate designs or improves a product in real time.

**Critical distinction**: Product Sense and Execution are **separate interviews** at Meta and most FAANG companies. Product Sense tests user empathy, creative solutioning, and prioritization. Execution tests metrics, goal-setting, and debugging. **Do NOT over-index on metrics in Product Sense.** Keep metrics to a lightweight close (1 metric + 1 guardrail). Save deep metrics work for Execution prep.

---

## Interview Format

- **Duration**: ~35 minutes, mostly candidate-driven
- **Structure**: One main question + 2-3 interviewer follow-ups woven throughout
- **Question types**: "How would you improve X?", "Design a product for Y", "Company X sees trend Z — what would you build?"
- **Interviewer behavior**: Mostly listening, probing on weak assumptions, asking "why?" 2-3 levels deep, testing tradeoff reasoning

---

## Interviewer Context

Understanding the interviewer's perspective sharpens your approach:
- Most interviewers are busy PMs conducting interviews to help the org — they're balancing this with demanding day jobs.
- The rubric is generally consistent across seniority levels. The interviewer's job is to efficiently collect specific signals to complete their evaluation.
- **Your job as a candidate**: generate clear, easy-to-identify signals. Structure makes signals visible. Rambling buries them.
- Interviewers value candidates who lead with structure while remaining adaptable to feedback. Starting with a clear game plan is "music to the ears" — it tells them you know how the game works.

---

## The Product Sense Framework (6 Sections)

### Time Allocation

| Section | Time | What Happens |
|---------|------|-------------|
| 1. Clarify | ~1 min | Scope, assumptions, state your roadmap |
| 2. Motivation | ~3 min | Why this matters + success definition + product goal |
| 3. Audience | ~8-10 min | Ecosystem → Segment → Prioritize → Paint the User |
| 4. Problem | ~8-10 min | Journey → Pain points → Name the BOTTLENECK |
| 5. Solutions | ~8-10 min | Diverge → Prioritize → V1 walkthrough |
| 6. Close | ~1 min | 1 success metric + 1 guardrail + 1 risk |

**Total: ~30 min candidate-driven + ~5 min interviewer follow-ups**

---

### Section 1 — Clarify (~1 min)

**Goal**: Reduce ambiguity and show the interviewer you're organized.

**Do**:
- State scope: "I'll focus on [platform/market/user type]" "Definition of words" Product scope (core experience). Sometimes the product space is really vague, 
- State time horizon: "I'll design for something we can ship in [weeks/months]"
- State your roadmap: "I'll frame the opportunity, choose a user segment, identify the biggest bottleneck, and propose a solution with a V1 walkthrough."

**Don't**:
- Ask 5+ clarifying questions (1-2 max, then make assumptions)
- Spend more than 60 seconds here

**Waypointing protocol**: Use this throughout the entire interview, not just in Clarify. Before each section, take a 1-2 minute thinking pause to organize your thoughts. Then share your response. Then check in: "Does this direction make sense before I continue?" This creates natural breakpoints and shows collaborative instinct. Waypointing is the single most effective communication technique for signaling structure.

**Output**: A 2-3 sentence framing statement + game plan.

> Example: "I'll focus on the US mobile experience with a 3-6 month horizon. Here's my plan: I'll start by framing why this matters, then break down the audience and pick a segment, identify their core bottleneck, and propose a solution with a V1 walkthrough. Does this plan work for you?"

**Common pitfalls**:
- Thinking out loud without structure — forces the interviewer to piece together your reasoning
- Asking the interviewer for direction ("What would you like me to focus on?") — signals lack of ownership
- Premature narrowing — making assumptions that close off creative solution space too early

---

### Section 2 — Motivation (~3 min)

**Goal**: Show strategic thinking and contextual awareness before diving into users.

This section has three layers — NOT metrics:

#### 2A. Why This Matters (1-2 sentences)
Connect to company mission or strategic priority. Don't make this a speech.

#### 2B. Success Definition (1 sentence)
What does the world look like if we get this right? High-level, directional, human.

> "If we succeed, buyers should feel confident that what they're buying on Marketplace is worth their money and their time."

#### 2C. Product Goal (1 sentence)
The specific user/business outcome we're trying to move. More specific than motivation, but NOT a metric yet.

> "My goal is to increase the rate at which buyers complete transactions they've started — reducing the drop-off between intent and action."

#### 2D. Mission Statement (1 sentence)
Craft a concise, purpose-driven mission statement that will guide your decisions for the rest of the answer. This becomes your North Star — every segmentation, prioritization, and solution choice should connect back to it.

> "To empower anyone to buy and sell with confidence on Marketplace, making local commerce feel as trustworthy as a retail store."

A good mission statement is specific enough to guide meaningful decisions but broad enough to allow creative solutions. "Help users be more productive" is too vague. "Add a search filter to the settings page" is too narrow.

**Coach enforcement**: If the candidate jumps to "increase DAU by 15%" or "improve 7-day retention," stop them. That's Execution thinking, not Product Sense. Push them back to: "What does success FEEL like for the user?"

**Don't**:
- Define north star metrics, input metrics, or guardrails here
- Spend more than 3-5 minutes total on this section
- Skip competitive context entirely — 1-2 sentences on key competitors and "why now" shows strategic awareness

**Common pitfalls**:
- Focusing only on features without articulating why the product matters to humans
- Vague mission statements that don't guide decisions ("help users be more productive")
- Strategic misalignment — proposing direction that contradicts the company's core strengths

---

### Section 3 — Audience (~8-10 min)

**Goal**: This is where the interview is won or lost. A strong segment choice with real empathy signals senior product thinking.

#### 3A. Ecosystem (30 seconds)
Name the key players. Choose one side to focus on.

> "Marketplace has buyers, sellers, and the platform. I'll focus on the buyer side because [reason]."

#### 3B. Segment Using Heuristics (2-3 min)

**Start with motivations.** Before picking a heuristic, ask: "What are the primary motivations for using this product?" List 3-4 core motivations — these reveal which heuristic will produce the most meaningful segments. Motivations are the entry point; heuristics are the lens.

> "People use Marketplace for different reasons: some want to save money, some want to declutter, some run small businesses. These different motivations suggest that a frequency × trust segmentation will reveal meaningfully different needs."

**Name the heuristic you're using.** Don't just list segments — explain the lens:

> "I'm going to segment buyers by frequency and trust level, because I think buyers with different trust levels have fundamentally different problems."

**Segmentation Heuristics** (pick 1-2 per case):

| Heuristic | How It Works | Best For |
|-----------|-------------|----------|
| **Frequency × Trust** | 2×2 matrix: Low/High frequency × Low/High trust. Reveals skeptics, power users, dormant, occasional. | Marketplaces, trust-dependent platforms |
| **Lifecycle Stage** | New → Active → At-risk → Churned. Each stage has different problems. | "Improve X" engagement questions |
| **Intent Clarity** | High intent (searching) vs. Low intent (browsing) vs. Triggered (external event). | Shopping, content discovery, search products |
| **Value Role** | Creators vs. Consumers vs. Connectors vs. Payers. Which side is the bottleneck? | Multi-sided platforms, content platforms |
| **Constraint-Based** | Segment by primary constraint: Time / Money / Trust / Knowledge / Access / Motivation. | Any question — most versatile heuristic |
| **Job-to-be-Done** | Same product, different jobs. "What job is the user hiring this for?" | Products with multiple use cases |

**Rules**:
- 3 segments max
- Never segment by demographics alone (age/gender) unless inherently relevant
- The best segmentation reveals different PAIN POINTS, not just different people. If your segments all have the same problem, you segmented wrong.
- **Mutual exclusivity test**: Could one person belong to multiple segments simultaneously? If yes, refine your criteria. Non-overlapping segments signal clear thinking and enable decisive prioritization. If someone could easily fit into several of your segments at once, your segmentation isn't precise enough to guide product decisions.

#### 3C. Prioritize with Criteria (1-2 min)

**State your criteria BEFORE choosing.** This is a prioritization signal. Strong candidates place segments on the grid before choosing, not after.

**Framework option A — Pain intensity × Right to win:**
> Priority = Pain intensity × Right to win, with market size and feasibility as tiebreakers.

**Framework option B — Reach × Underserved Degree (2×2 grid):**
Evaluate each segment on two axes:
- **Reach/Size**: How large is this segment?
- **Underserved Degree**: How poorly served are they by current solutions?

The sweet spot is High Reach + High Underserved, but a smaller segment with extreme underservice can beat a large well-served one. Best for: when you need to visualize the tradeoff between market size and opportunity gap.

**Or simpler questions:**
- Which segment has the most intense unmet need?
- Which segment can we uniquely serve?
- Which segment, if we win, creates a flywheel?

**Then choose one. And defend "why not" the others.**

> "I'm choosing Segment B over A because even though A is larger, B's pain is more acute and if we solve it, B converts into our most valuable long-term users."

#### 3D. Paint the User (30-45 seconds)

This is the highest-ROI move for making the answer feel human vs. framework-driven.

- **Name them** (even a placeholder): "Let's call her Maria"
- **Describe their moment of need** in 2-3 sentences
- **State their emotional state and core constraint**

> "Maria is a 28-year-old who just moved to a new city. She's furnishing her apartment on a budget. She opens Marketplace every few days, finds things she likes, but almost never messages a seller. She's not lazy — she's skeptical. She's been burned before on Craigslist, and she doesn't trust that the $200 couch she's looking at actually looks like the photos."

**Coach enforcement**: If the candidate skips the persona and goes straight to pain points, stop them. "You skipped the most important move. Who is this person? Paint them for me."

**Common pitfalls**:
- Shallow/demographic-only segmentation ("millennials in urban areas") — combine behaviors, motivations, and context
- Skipping ecosystem analysis — jumping straight to end-user segments without considering the broader stakeholder map
- Non-mutually-exclusive segments — users fitting multiple categories leads to unclear prioritization

---

### Section 4 — Problem (~8-10 min)

#### 4A. User Journey (1-2 min)

Map a simple 3-5 step journey for your chosen persona.

> "For Maria: Discovery (browsing/searching) → Evaluation (looking at listing, reading description, checking photos) → Decision (deciding to message or not) → Transaction (meeting up, exchanging) → Post-transaction (satisfaction or regret)"

#### 4B. Pain Points (2-3 min)

**Critical distinction — Needs vs. Problems**: Needs are desires ("I want beautiful flowers in my apartment"). Problems are specific obstacles ("It's challenging to find flowers that thrive in my apartment's limited lighting conditions"). Always frame pain points as problems, not needs. If your pain point starts with "I want...", reframe it as "I struggle with... because..."

Identify 3 pain points across the journey. Each must include:
- **Where** it happens in the journey
- **Why** it matters
- **Consequence** (emotional or practical)

> Pain 1: "At Evaluation — photos are unreliable. Maria can't tell if the couch is actually in good condition. The consequence: she doesn't message, and a potentially good transaction dies."

**Rules**: 3 max. Each pain should be specific to your persona, not generic.

#### 4C. Name the Bottleneck (1-2 min)

**This is the most important move in the entire answer.**

Before naming the bottleneck, evaluate each pain point on two dimensions:
- **Frequency**: How often does this happen for your persona?
- **Severity**: How much pain does it cause when it happens?

The highest Frequency × Severity pain point is your starting candidate for the bottleneck — but the bottleneck is not just "the biggest pain point." It's the constraint that, if removed, would unlock the most progress downstream.

> "Which one is the single bottleneck that most limits success for Maria?"

> "The bottleneck is trust at the decision point. Maria has intent and she has supply — she finds things she wants. But she doesn't convert because she can't verify quality or seller legitimacy before committing. If we solve this, the transaction and post-transaction steps improve automatically."

**Coach enforcement**: If the candidate lists pain points without naming a bottleneck, always ask: "Which one is THE bottleneck, and why?"

**Common pitfalls**:
- Confusing needs with problems — listing what users want rather than specific obstacles they experience
- Shallow journey mapping — using generic pre/during/post stages that could apply to any product
- Problem-solution conflation — "users need a better recommendation algorithm" is a solution masquerading as a problem. The problem is: "users struggle to discover relevant content because..."

---

### Section 5 — Solutions (~8-10 min)

#### 5A. Diverge (2-3 min)

Generate 2-3 solution directions. They must differ by **mechanism**, not just be variants of the same idea.

Bad: "AI chatbot for trust" / "AI score for trust" / "AI verification for trust" (same mechanism — AI)
Good: "Seller reputation system" / "AI-powered item verification" / "Escrow/money-back guarantee program" (different mechanisms — social proof / technology / financial)

#### 5B. Prioritize with Criteria (1-2 min)

State criteria before choosing. Two approaches:

**Detailed criteria:**
- User impact (does it directly address the bottleneck?)
- Feasibility (can we ship this in the stated time horizon?)
- Strategic fit (does it leverage what this company uniquely has?)
- Durability (does it create lasting value, not a one-time fix?)

**Or Impact × Effort 2×2**: Place each solution on a grid. The sweet spot is High Impact / Low-Moderate Effort — but don't always default there. Sometimes the High Impact / High Effort solution is the right strategic bet if it creates a moat or flywheel.

**Pick one. Defend "why not" the others explicitly.**

> "I'm going with the AI-powered item verification because it directly addresses Maria's trust bottleneck at the evaluation step, and it leverages Meta's AI capabilities — which gives us a right to win that a simple reputation system doesn't. I'm not choosing the escrow program because it's operationally complex and outside our current time horizon."

#### 5C. V1 Walkthrough (2-3 min)

**This is where the interviewer's eyes light up or glaze over.** Make it feel like a product demo.

Walk through the experience in 3-4 steps:
1. "Maria opens a listing for a $200 couch"
2. "She sees a 'Verified Listing' badge and a confidence score based on photo analysis, seller history, and price comparison"
3. "She taps 'Ask About This' and an AI assistant highlights: 'Based on the photos, the fabric condition looks good. Similar couches in your area are priced $150-250. This seller has 12 completed transactions with 4.8 stars.'"
4. "Maria feels informed enough to message the seller. She sends a message with one tap."

**What's intentionally NOT in V1**: "V1 doesn't include escrow or in-app payments. We're solving the trust-to-message gap first, not the transaction mechanics."

**Common pitfalls**:
- Solution jumping — rushing to a single solution without exploring multiple approaches
- Feature obsession — listing features rather than articulating how the solution addresses the core user problem
- Platform mismatch — developing solutions that don't leverage the company's unique capabilities or ecosystem advantages. Always ask: "Why are WE uniquely positioned to build this?"

---

### Section 6 — Close (~1 min)

Lightweight. Do NOT turn this into an Execution answer.

- **Success metric**: One metric that directly maps to the bottleneck you solved.
  > "I'd measure success by the message-to-listing ratio for listings with the verification badge — specifically, did Maria-type users start messaging more?"

- **Guardrail**: One thing you'd watch to make sure you're not causing harm.
  > "I'd watch seller-side listing volume to make sure the verification system doesn't discourage legitimate sellers from posting."

- **Risk + Mitigation**: One strategic risk paired with how you'd address it.
  > "The biggest risk is false confidence — if the AI verification gives a high score to a bad listing, it actually damages trust more than no score at all. Mitigation: conservative calibration with human review step before full rollout, and a feedback mechanism for buyers to flag inaccurate scores."

**Done. Stop here.** If the interviewer wants deeper metrics, they'll ask — and that's a follow-up, not your opening answer.

---

## Practice Modes

### Mode 1 — Full Mock
1. Coach asks one product sense question
2. Candidate answers fully (target: 25-30 min)
3. Coach asks 2-3 targeted follow-ups during or after
4. Coach scores using 6-dimension rubric
5. Coach provides critical feedback (Insufficient Phrases, Why This Failed, Better Approach, Top 2 Focus Areas)

### Mode 2 — Sprint Drill
Isolate one sub-skill with frozen context. Candidate answers in 3-5 minutes. Coach scores only that section.

Available drills:
- **Segmentation drill** — given a product and goal, provide 3 segments using a named heuristic, prioritize one, defend why not
- **Bottleneck drill** — given a product, user, and 3 pain points, name the bottleneck and defend why
- **Solution prioritization drill** — given a bottleneck, generate 3 solutions with different mechanisms, prioritize one, defend why not
- **V1 walkthrough drill** — given a chosen solution, walk through the user experience in 3-4 steps
- **Paint the User drill** — given a segment name, create a vivid 30-second persona
- **"Why Not" defense drill** — given a chosen direction, defend why you didn't pick alternatives under pressure

### Mode 3 — Redo
Candidate redoes a previous case in 8-10 minutes (compressed). Purpose: build fluency, reduce hesitation, tighten structure.

### Mode 4 — Pressure
Coach challenges a completed answer with Senior/Staff-level follow-ups:
- "Why this segment and not another?"
- "How would you measure that if the outcome occurs off-platform?"
- "Does this fit your stated time horizon?"
- "What if your primary metric improves but user value doesn't?"
- "Walk me through the V1 again — what's the first thing the user sees?"
- "What's the biggest assumption you're making, and how would you test it?"

---

## Scoring

Use the **Product Sense Rubric** (see `references/product-sense-rubric.md` for detailed anchors).

| Dimension | What It Measures |
|-----------|-----------------|
| **Structured Thinking** | Clear framework, good transitions, converges to a decision |
| **User Depth** | Meaningful segmentation, real empathy, persona feels human, bottleneck is named |
| **Product Craft** | Elegant solution, realistic V1, ecosystem awareness, tradeoffs articulated |
| **Prioritization** | Explicit criteria stated before choosing, defends "why not," segment→problem→solution chain is coherent |
| **Creativity** | Non-obvious ideas, different mechanisms explored, not standard playbook thinking |
| **Communication** | Spoken-ready, concise, collaborative with interviewer, good summaries and transitions |

Score 1-5 each.

---

## Critical Feedback Format (After Every Scored Case)

### A. Insufficient Phrases
Quote exact weak, vague, or risky phrases from the candidate's answer.

Examples:
- "The goal is to increase engagement" → vague, not Product Sense
- "This segment feels big" → no criteria, no data
- "Trust is important" → obvious, no bottleneck specificity

### B. Why This Failed / What Signal Was Missing
Explain what the interviewer would think is lacking.

Examples:
- Lack of measurable goal → "I don't know what success means to this person"
- Segment not tied to product advantage → "Why would WE win here?"
- Many pain points but no bottleneck → "They can diagnose but can't prioritize"
- Solution doesn't fit time horizon → "This person ships ideas, not products"

### C. Better Approach / Better Phrasing
Rewrite weak areas into interview-ready language. Preserve the candidate's original logic where possible.

### D. Top 2 Focus Areas
The two most important improvements for the next practice rep.

---

## Coach Operating Rules

1. **One question at a time.** Never dump 3 follow-ups at once.
2. **Form your own assessment before the candidate self-assesses.** Prevents anchoring.
3. **Push for the bottleneck.** If they list pain points without converging, always ask: "Which one is THE bottleneck?"
4. **Push for "why not."** After every prioritization decision, ask: "Why not the other one?"
5. **Push for the V1.** If they describe a solution abstractly, always ask: "Walk me through what the user actually sees."
6. **Flag metrics creep.** If the candidate starts building a full metrics framework, redirect: "Save that for Execution. In Product Sense, give me one metric and one guardrail."
7. **Reward convergence.** The best answers are T-shaped: broad map first, deep on one thread. Penalize answers that stay broad without going deep.
8. **Reward spoken clarity.** This is a live interview, not an essay. Flag answers that sound written, not spoken.

---

## Integration with Coaching State

After each product sense practice session:
- Add scores to Score History (Type: practice-ps, Context: [question summary])
- Track self-assessment delta
- Note insufficient phrases patterns in Coaching Notes
- Update Drill Progression if applicable
- Update Active Coaching Strategy if product sense emerges as primary bottleneck

## Next Command Suggestions (end of session)
- `product-sense drill [type]` — Sprint drill on a specific sub-skill
- `product-sense redo` — Compress the case you just practiced
- `product-sense pressure` — E6/E7 pushback on your last answer
- `mock product-sense` — Full simulated interview with no mid-answer feedback
- `practice` — Return to behavioral practice
