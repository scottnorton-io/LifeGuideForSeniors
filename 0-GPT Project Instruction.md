# 📂 GPT Project Structure

### 1. **Core Instructions File** (`ai.txt` or `llms.txt`)

This is the “constitution” for the project — the permanent rules the AI must follow when building or expanding the guide.

**Example Core Instructions:**

* **Purpose**: Always help seniors uncomplicate their lives by providing clear, friendly, step-by-step guidance.
* **Tone**: Empathetic, supportive, non-technical, confidence-building.
* **Format**: Use interactive sections, checklists, and simple exercises. Always conclude with a clear *action item*.
* **Constraints**: Avoid jargon, don’t overwhelm with options, keep steps achievable.
* **Interactivity**: Present content as click-through modules, fillable templates, or printable checklists where possible.

---

### 2. **Addendums**

Separate, versioned files that refine or expand the main instructions. These allow for iteration without cluttering the core rules.

**Examples:**

* `addendum-tech-simplification-v1.md` → Special instructions for tech-related sections (passwords, video calls, device use).
* `addendum-health-tracker-v1.md` → How to structure medication/energy tracking modules.
* `addendum-money-v1.md` → Budget templates, subscription reviews, and autopay walkthroughs.
* `addendum-style-v1.md` → Narrative guidance: always open with a relatable story, then steps, then action item.

---

### 3. **Guiding File (Dynamic Context)** (`guiding-ai.txt`)

This is the **working memory/context file** where you capture evolving project direction. It tells the AI what stage you’re in and what’s next.

**Example Guiding File Contents:**

* Current stage: Prototyping Notion interactive modules.
* Priority areas: Tech simplification + Daily routines.
* Next deliverable: Draft a fillable medication tracker template.
* Pending questions: Should we build this first as a Notion doc or a Clickable PDF?

---

### 4. **Outputs**

All generated content (templates, outlines, drafts) go in their own folder — versioned and labeled by section.

* `outputs/tech-module-v1.md`
* `outputs/health-checklist-v1.pdf`
* `outputs/daily-routines-v1.notion`

---

# 🚀 Benefits of This Setup

* **Consistency**: Core rules (`ai.txt`) keep every response on-brand.
* **Flexibility**: Addendums allow focused iteration without overwriting the big picture.
* **Direction**: `guiding-ai.txt` acts like a project manager, keeping the AI on track.
* **Scalability**: You can plug in different LLMs (Claude, GPT-5, Gemini) — they’ll all use the same ruleset.

---
