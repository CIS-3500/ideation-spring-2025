# Chrome Extension Idea: Penn Course Search ++ — Prompt‑Powered Course Decision Assistant

## Authors  
Ioannis Kalaitzidis (jokala)  
Claire Zhao (clairezz)  
Maria Ramos ( )  
Chaelsey Park (chaelsey)

---

## Problem Statement  
The existing **Penn Course Search Extension** already fetches Penn Course Review (PCR) data for a single course ID, but students still — 

* Manually copy details into ChatGPT to ask: “Is this a good fit?”  
* Struggle to **compare two similar electives** side‑by‑side.  
* Risk copy‑paste errors when highlighting course IDs on Path@Penn.  

These gaps force repeated tab‑switching and drain decision‑making time during the hectic registration window.

---

## Target Audience  
Penn undergraduates and master’s students who:

* Juggle GenEd, major, and minor requirements.  
* Use Penn Course Review metrics (Difficulty, Workload, Rating) to balance schedules.  
* Already rely on LLMs for quick advice but find prompt creation tedious.  

---

## Description  
**Penn Course Search ++** builds on the open‑source extension by adding four tightly‑integrated features that eliminate copy‑paste friction and enable data‑driven course comparisons:

| # | Feature | Goal |
|---|---------|------|
| **1** | **Single‑Course GPT Prompt Generator** | One‑click copy of a crafted prompt that includes course stats + user interests. |
| **2** | **Checkbox Course Selection UI with Persistent History** | Reliable, confirmable way to stage courses for comparison across sessions. |
| **3** | **Smart Two‑Course Visual Comparison Panel** | Side‑by‑side metrics view (diff, workload, rating, prereqs) in expanded popup. |
| **4** | **Two‑Course GPT Prompt Builder** | One‑click prompt that asks an LLM to recommend between the two staged courses. |

---

## Selling Points  
1. **Zero Copy‑Paste to GPT** – Prompts generated and copied automatically.  
2. **Error‑Proof Selection** – Checkbox validation prevents wrong course IDs.  
3. **Persistent History** – Reuse courses chosen yesterday without re‑highlighting.  
4. **Visual Insight First** – Quick table comparison before even invoking GPT.  
5. **Fully Local & Private** – No user data leaves the browser; PCR API is public.

---

## User Stories  

1. As a sophomore, I want a one‑click GPT prompt for **one course** so I can know if it fits my SSH requirement.  
2. As a student narrowing electives, I want to **select two courses with checkboxes** so I’m sure the right courses are compared.  
3. As a time‑crunched registrant, I want a **visual diff table** so I can spot which course has lower workload instantly.  
4. As a returning user, I want yesterday’s saved courses to appear under **History** so I can continue my research.  
5. As a GPT user, I want a **comparison prompt** that explains which of two courses suits my stated interests best.  
6. As an accessibility‑focused user, I want keyboard navigation for checkboxes so I don’t rely on mouse highlighting.  
7. As a double major, I want prompts to include both my majors so GPT understands my academic context.  
8. As a freshman, I want the extension to warn me if a course requires prereqs I haven’t taken.  
9. As a user with limited time, I want toast notifications confirming copies so I know the action succeeded.  
10. As a PowerGPT user, I want to tweak the tone (“persuade me” vs. “critique it”) before copying the prompt.

---

## Technical Implementation

### A. Architecture Overview

| Component | Role |
|-----------|------|
| **Content Script** | Detects course highlights, extracts course IDs. |
| **Popup React App** | Renders course cards, checkbox lists, comparison panel, prompt buttons. |
| **Background Script** | Manages persistent course history in `chrome.storage.local`. |
| **GPT Prompt Module** | Pure JS utility that formats course objects into prompt strings. |

---

### B. Feature Details & User Flow

#### 1. Single‑Course GPT Prompt Generator
* **Trigger:** “Generate GPT Prompt” button on course card.  
* **Flow:** Pull PCR data + user profile → build template → `navigator.clipboard.writeText()` → toast “Prompt copied!”  
* **Prompt Length:** ≤ 150 words to stay under GPT context.

#### 2. Checkbox Course Selection with History
* **Lists:**  
  * *Currently Selected* – unchecked by default → user verifies.  
  * *Previously Selected* – loaded from storage.  
* **Data Model:**  
```ts
interface SavedCourse {
  id: string; title: string; diff: number; work: number; rating: number;
  confirmed: boolean; ts: number;
}
```

### Validation  
- **Buttons:** “Compare” and “Build Prompt” are enabled **only when exactly two courses are confirmed** via checkboxes.

---

### 3. Smart Two‑Course Visual Comparison  

| Aspect | Details |
|--------|---------|
| **UI** | Popup width expands to **650 px** and mounts a `<ComparisonTable>` React component. |
| **Highlighting** | • Green badge on **lower** Difficulty / Workload.<br>• Gold star on **higher** Rating. |
| **Edge Cases** | If any metric is missing (N/A), corresponding cell is greyed‑out for clarity. |

---

### 4. Two‑Course GPT Prompt Builder  

| Step | Description |
|------|-------------|
| **Trigger** | “Build Prompt” button appears in the comparison view. |
| **Template Fields** | Course stats + stored user majors/minors + free‑text preference (e.g., “I prefer lighter workload and engaging discussions”). |
| **Output** | Prompt is copied to clipboard; optional manual textarea allows last‑second edits before copying. |

---

### C. Key Selectors / API Use  

- **PCR Data Endpoint:** `https://penncoursereview.com/api/v1/course/{id}`  
- **Highlight Regex:** <code>\b[A-Z]{2,4}\s?\d{4}\b</code> (detects `CIS 1200`, `MATH2400`, etc.)  
- **Chrome Storage Keys**  
  - `currentSelections` – session list of courses pending confirmation  
  - `courseHistory` – persistent list of previously confirmed courses  

---

## Notes  

### Limitations  
1. Works only for courses available in the PCR API dataset.  
2. GPT call remains **manual copy‑paste** in MVP (avoids handling API keys).  
3. UI optimized for desktop Chrome; mobile Chrome support deferred.

### Future Enhancements  
- Inline GPT request if user supplies their OpenAI key.  
- Auto‑generate Penn schedule grid when > 2 courses are selected.  
- Export comparison table directly to Markdown for advising e‑mails.

---

## Timeline & Effort

| Week | Milestone |
|------|-----------|
| **1** | Fork repo, create `feature/checkbox-selection` branch, scaffold checkbox state. |
| **2** | Implement persistent history + checkbox UI badges. |
| **3** | Build `<ComparisonTable>` component; add popup width toggle. |
| **4** | Add single‑course GPT prompt generator; clipboard utility. |
| **5** | Add two‑course GPT prompt builder; tone customization dropdown. |
| **6** | Polish UX, write unit tests, prep class demo. |

> **Total development effort:** ~25 hours across six weeks (4‑person team)

---

## References & Inspiration  
- **Original project:** *PennCourseChromeExtension* by Franci Branda‑Chen et al.  
- **Prompt‑engineering patterns** for comparison and recommendation tasks.  
- **Figma** accessibility guidelines for color‑contrast (badge design).

---

### ➡ Next Steps  
- [ ] Create `feature/checkbox-selection` branch and scaffold `<CheckboxList>` component.  
- [ ] Need starter TypeScript snippets or Redux‑style context for shared course state? *Let me know!*
