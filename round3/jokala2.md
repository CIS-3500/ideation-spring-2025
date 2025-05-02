✅ Checkbox Course Selection Feature – Purpose & Utility
🔧 Background
The current course selection method relies on users highlighting course names on Path@Penn, which can be error-prone:
    •    If a user accidentally highlights too much or too little text, the extension may not correctly extract the course ID or name.
    •    Users receive no visual confirmation of their current or past selections, increasing the chance of comparison errors.
🧠 Solution: Checkbox Interface with History + Validation
To improve reliability, the Chrome extension implements a checkbox interface that reflects and validates highlighted selections.
🧩 How It Works
    1    After Highlighting a Course:
    ◦    The extension scrapes the course name/ID and stores the corresponding Penn Course Review data.
    ◦    That course is added to a visual list with a checkbox in a section titled:
    ▪    ✓ Currently Selected
    ▪    📁 Previously Selected (History)
    2    "Currently Selected" Section:
    ◦    This section shows the courses the user has selected in this session.
    ◦    The user can manually confirm (check) whether each selection was correct, preventing accidental mis-selection from going unnoticed.
    ◦    Only checked courses proceed to comparison.
    3    "History" Section:
    ◦    This section stores courses selected in prior sessions (cached locally via chrome.storage.local).
    ◦    Users can:
    ▪    Re-include prior courses in a new comparison by checking the box.
    ▪    Reference past data without needing to re-highlight.
    ▪    Ensure consistency if they're iterating or refining course choices over time.
🛠️ Technical Utility
    •    Ensures data integrity by requiring manual user confirmation before a course is used for matching.
    •    Tracks user preferences and review data without redundancy, improving performance and UX.
    •    Allows the extension to defer processing until the user verifies the selection, avoiding logic errors tied to real-time highlighting.
    •    Offers a fallback UI that makes the extension more fault-tolerant against highlight glitches.
💡 Example Workflow:
    1    Student highlights CIS 1200 → Extension adds it to "Currently Selected", unchecked.
    2    Student sees the checkbox, confirms it's the intended class, and checks it.
    3    Student highlights CIS 1210 → Same flow.
    4    Student opens the extension later, sees past picks (CIS 1600, CIS 2400) in "Previously Selected".
    5    Chooses to include CIS 1600 again for a new comparison.

🧭 Summary of Benefits
    •    ✔️ Eliminates user error from faulty highlighting
    •    ✔️ Adds transparency and control over what's being compared
    •    ✔️ Supports iterative comparison across sessions
    •    ✔️ Boosts confidence in the extension's selections and analysis
Would you like help writing the contentScript.js and popup logic to implement this checkbox interface with persistent history?

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
