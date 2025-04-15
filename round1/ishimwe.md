
# LinkedIn Job Clipper Chrome Extension

## 🌟 Overview

**LinkedIn Job Clipper** is a Chrome extension designed to streamline the process of job applications by allowing users to easily copy job descriptions from LinkedIn with a single click. The copied content can then be directly pasted into ChatGPT or other AI tools to analyze, summarize, or personalize application materials.

## 🚀 Why This Is Helpful

- **Time-Saving:** Job seekers no longer need to manually select and copy job descriptions.
- **AI Integration:** Enables quick input into ChatGPT for tasks like resume tailoring, skill-gap analysis, or cover letter generation.
- **User Convenience:** One-click clipboard functionality directly on the LinkedIn interface.
- **Future-Proof:** Easily extendable into a more robust tool—such as clipping and saving multiple jobs, or integrating prompt templates for personalized outputs.

---

## ✨ Potential Future Expansions

### 1. **Job Clipping History**
Allow users to save multiple job descriptions locally or in cloud storage for later use.

### 2. **Prompt Engineering UI**
Include a prompt builder section that feeds both the job description and user's LinkedIn profile content into ChatGPT with prompts like:
- “What parts of this job match my skills?”
- “What skills am I missing?”
- “Draft a tailored cover letter for this role.”

---

## 🧩 Core Features (MVP)

- [x] Detect when the user is on a LinkedIn job page.
- [x] Extract the job description from the DOM.
- [x] Add a floating or fixed “Copy Job Description” button to the page.
- [x] Copy the job description text to the clipboard when clicked.
- [ ] (Optional) Notify user with a toast/snackbar message like “Copied!”

---

## 🛠️ How to Build It

### Step 1: Setup Your Extension
- Create a `manifest.json` file (v3 recommended).
- Set permissions: `"activeTab"`, `"scripting"`, and `"clipboardWrite"`.

```json
{
  "manifest_version": 3,
  "name": "LinkedIn Job Clipper",
  "version": "1.0",
  "permissions": ["activeTab", "scripting", "clipboardWrite"],
  "action": {
    "default_popup": "popup.html",
    "default_icon": "icon.png"
  },
  "content_scripts": [
    {
      "matches": ["*://*.linkedin.com/jobs/*"],
      "js": ["content.js"]
    }
  ]
}
