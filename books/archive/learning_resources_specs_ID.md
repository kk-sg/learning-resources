# Learning Resources Specs: ID Book Challenge

**Document Type:** Challenge Specifications  
**Challenge:** 21 Books in 24 Days - Instructional Design Deep Dive  
**Created:** March 21, 2026  
**Status:** Completed

---

## Overview

This document defines the specifications and requirements for the ID Book Challenge learning resource generation.

---

## Challenge Metadata

| Field | Value |
|-------|-------|
| **Challenge Name** | 21 Books in 24 Days - Instructional Design Deep Dive |
| **Start Date** | 2026-02-21 |
| **End Date** | 2026-03-16 |
| **Participant** | K |
| **Focus** | E-learning and AI |
| **Delivery Time** | 21:00 (9 PM) |
| **Timezone** | Asia/Singapore |
| **Total Days** | 24 |
| **Total Books** | 21 |
| **Review Days** | 3 (Days 12, 19, 24) |

---

## Delivery Location

| Field | Value |
|-------|-------|
| **Platform** | Telegram |
| **Chat ID** | -1003750328075 |
| **Topic ID** | 216 |
| **Topic Name** | Learning Resources |

---

## End Goals

1. Build comprehensive reference library
2. Improve skills in e-learning and AI
3. Create portfolio-ready concepts and frameworks

---

## Daily Content Specifications

### Required Output Per Day

| Component | Specification |
|-----------|---------------|
| **Content Length** | 20,000+ characters |
| **Case Studies** | 5 case studies (E-learning & AI focus) |
| **Takeaways** | 5 actionable takeaways |
| **Reflection Questions** | 5 reflection questions |
| **File Format** | Markdown (.md) file |
| **Delivery Method** | Summary message + .md file attachment |

---

## Content Structure Template

```markdown
# Day X: [Book Title]
**Author:** [Author Name]
**Focus:** E-learning & AI
**Date:** [Delivery Date]

---

## 📖 BOOK OVERVIEW

### Why This Book Matters
[2-3 paragraphs explaining the book's significance]

### Key Differentiator
[What makes this book unique/valuable]

### The Central Philosophy/Thesis
[Core message in 1-2 sentences]

---

## 🎯 CORE FRAMEWORK(S)

### [Framework Name]
**What It Is:**
[Explanation]

**Key Elements:**
- Element 1
- Element 2
- Element 3

**How to Apply:**
[Practical application steps]

**E-Learning/AI Application:**
[Specific AI/e-learning use cases]

---

## 💡 5 ACTIONABLE TAKEAWAYS FOR E-LEARNING & AI

### 1. [Takeaway Title]
**Action:** [Specific action to take]
**Why It Matters:** [Explanation]
**E-Learning/AI Application:** [How to apply with AI]

[Repeat for takeaways 2-5]

---

## 🧪 5 CASE STUDIES FOR E-LEARNING & AI

### Case Study 1: [Title]

**Situation:**
[Context]

**Problem:**
[Challenge]

**Solution:**
[What was done]

**AI Enhancement:**
[How AI was/could be applied]

**Results:**
[Outcomes with metrics]

**Lesson:**
[Key takeaway]

[Repeat for case studies 2-5]

---

## ❓ 5 REFLECTION QUESTIONS

1. [Question 1 - specific and actionable]
2. [Question 2]
3. [Question 3]
4. [Question 4]
5. [Question 5]

---

## 🌅 TOMORROW'S PREVIEW

**Day X+1: [Book Title]**
*by [Author]*

We'll explore:
- [Preview point 1]
- [Preview point 2]
- [Preview point 3]

---

## 📚 ADDITIONAL RESOURCES

- **Book Website:** [URL if available]
- **Author:** [Author info]
- **Related Books:** [Connections to other books in challenge]

---

*Content prepared by Kai Kai (凯凯) ✨ for the 21-Day ID Book Challenge*  
*Saved to: learning-resources/books/ID/[filename].md*
```

---

## Challenge Schedule

### Phase 1: Classics (Days 1-11)

| Day | Book | Author |
|-----|------|--------|
| 1 | Design for How People Learn | Julie Dirksen |
| 2 | The Accidental Instructional Designer | Cammy Bean |
| 3 | Michael Allen's Guide to e-Learning | Michael Allen |
| 4 | Leaving ADDIE for SAM | Michael Allen & Richard Sites |
| 5 | Map It | Cathy Moore |
| 6 | e-Learning by Design | William Horton |
| 7 | e-Learning and the Science of Instruction | Ruth Clark & Richard Mayer |
| 8 | The Essentials of Instructional Design | Abbie H. Brown & Timothy D. Green |
| 9 | The Non-Designer's Design Book | Robin Williams |
| 10 | Make It Stick | Peter C. Brown et al. |
| 11 | The Gamification of Learning and Instruction | Karl M. Kapp |

### Phase 2: Review Day (Day 12)

| Day | Type | Focus |
|-----|------|-------|
| 12 | Review | Classics Synthesis (Books 1-11) |

### Phase 3: Hidden Gems (Days 13-18)

| Day | Book | Author |
|-----|------|--------|
| 13 | The Mom Test | Rob Fitzpatrick |
| 14 | Start with WHY | Simon Sinek |
| 15 | The Art of Explanation | Lee LeFever |
| 16 | Style: Lessons in Clarity and Grace | Joseph M. Williams & Joseph Bizup |
| 17 | Resonate | Nancy Duarte |
| 18 | Creative Confidence | Tom & David Kelley |

### Phase 4: Review Day (Day 19)

| Day | Type | Focus |
|-----|------|-------|
| 19 | Review | Hidden Gems Synthesis (Books 12-17) |

### Phase 5: Modern Practice (Days 20-23)

| Day | Book | Author |
|-----|------|--------|
| 20 | Learning Experience Design Essentials | Cara North |
| 21 | Talk to the Elephant | Julie Dirksen |
| 22 | Reverse Training Design | Mark Mrohs |
| 23 | What I Wish I Knew Before Becoming an ID | Luke Hobson |

### Phase 6: Final Review (Day 24)

| Day | Type | Focus |
|-----|------|-------|
| 24 | Review | Complete Synthesis (All 21 Books) |

---

## Tracker File Structure

**Location:** `/home/kk/.openclaw/workspace/learning-resources/reading-challenge-tracker.json`

### Root Fields

```json
{
  "challengeName": "string",
  "startDate": "YYYY-MM-DD",
  "endDate": "YYYY-MM-DD",
  "participant": "string",
  "focus": "string",
  "deliveryTime": "HH:MM",
  "timezone": "string",
  "currentDay": "number",
  "status": "scheduled|in_progress|completed",
  "schedule": [...],
  "telegramTopic": {...},
  "endGoal": [...]
}
```

### Schedule Entry Fields

```json
{
  "day": "number",
  "date": "YYYY-MM-DD",
  "type": "book|review",
  "bookNumber": "number (optional)",
  "title": "string",
  "author": "string (optional)",
  "status": "scheduled|delivered",
  "deliveryMethod": "manual|cron",
  "deliveredAt": "ISO 8601 timestamp (optional)",
  "messageId": "string (optional)",
  "notes": "string (optional)"
}
```

### Telegram Topic Fields

```json
{
  "chatId": "string",
  "topicId": "string"
}
```

---

## Automation Details

### Cron Job Configuration

| Field | Value |
|-------|-------|
| **Job ID** | ce02cb4a-abb4-4342-a5e5-aed786707561 |
| **Schedule** | `0 21 * * *` (daily at 9 PM) |
| **Timezone** | Asia/Singapore |
| **Agent** | main |
| **Session Target** | isolated |
| **Wake Mode** | now |

### Delivery Workflow

1. Read tracker to get current day/book
2. Research book via web search
3. Generate deep dive content (20,000+ characters)
4. Save .md file to workspace
5. Send summary to Telegram (normal reply)
6. Send .md file attachment (message tool)
7. Update tracker (status → delivered, increment currentDay)

---

## File Storage

### Generated Content

**Location:** `/home/kk/.openclaw/workspace/learning-resources/books/ID/`

**Naming Convention:** `{day_number}-{book_title_kebab_case}.md`

**Examples:**
- `01-design-how-people-learn.md`
- `02-accidental-instructional-designer.md`
- `12-review-classics-synthesis.md`

### Supporting Files

| File | Location | Purpose |
|------|----------|---------|
| Tracker | `learning-resources/reading-challenge-tracker.json` | Challenge state |
| Specs | `learning-resources/archive/learning_resources_specs_ID.md` | This document |
| Memory | `memory/2026-02-24.md` | Daily notes |

---

## Quality Standards

### Content Requirements

- ✅ All content must focus on **E-learning & AI applications**
- ✅ Frameworks must include **practical application steps**
- ✅ Case studies must include **measurable results**
- ✅ Takeaways must be **actionable** (not just informational)
- ✅ Reflection questions must be **specific** (not generic)

### Writing Standards

- **Tone:** Professional, practical, encouraging
- **Perspective:** Second person ("you") for engagement
- **Formatting:** Consistent markdown with emoji markers
- **Length:** 20,000+ characters (verified)

### Review Day Standards

- ✅ Synthesize concepts across multiple books
- ✅ Create integrated frameworks
- ✅ Show connections between authors/ideas
- ✅ Provide meta-patterns and unifying themes

---

## Success Metrics

| Metric | Target | Actual |
|--------|--------|--------|
| Books Delivered | 21 | 21 |
| Review Days | 3 | 3 |
| Completion Rate | 100% | 100% |
| On-Time Delivery | 100% | ~83% (some delays) |
| Content Length | 20,000+ chars | 27,000-55,000 chars avg |
| Case Studies | 5 per day | 5 per day |
| Takeaways | 5 per day | 5 per day |
| Reflection Questions | 5 per day | 5 per day |

---

## Lessons Learned

### What Worked

- ✅ Deep dive format provided comprehensive value
- ✅ AI focus made content immediately applicable
- ✅ Case studies grounded theory in practice
- ✅ Review days created synthesis and retention
- ✅ Tracker file enabled automation

### What Could Improve

- ⚠️ Cron job timeout (10 min) too short for content generation
- ⚠️ Some delivery delays due to automation issues
- ⚠️ Manual intervention required for early days
- ⚠️ File naming inconsistencies (some duplicate day numbers)

---

## Related Resources

- **ID Book Challenge Files:** `/home/kk/.openclaw/workspace/learning-resources/books/ID/`
- **Tracker:** `/home/kk/.openclaw/workspace/learning-resources/reading-challenge-tracker.json`
- **Memory Files:** `/home/kk/.openclaw/workspace/memory/`

---

*Document created: March 21, 2026*  
*Archived in: learning-resources/archive/*
