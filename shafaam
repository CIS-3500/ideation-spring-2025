# Chrome Extension Idea: Distracto‑Nix

## Authors

Shafaa Munjal

## Problem Statement

Many users struggle to stay focused because sites like Reddit, Twitter, and YouTube are just a click away. Existing solutions (browser overlays, manual blocklists) can be bypassed or are a hassle to configure. There’s a need for a frictionless, one‑click way to **completely** prevent access to specified distractor sites across **all** tabs until the user chooses to re‑enable them.

## Target Audience

- Knowledge workers (developers, writers, designers) needing uninterrupted work sessions  
- Students and researchers aiming to minimize online procrastination  
- Remote workers and freelancers juggling multiple online tools  
- Anyone who wants a zero‑loophole digital discipline tool

## Description

Distracto‑Nix is a lightweight Chrome extension that toggles a global Focus Mode with one click. When Focus Mode is ON, it uses Chrome’s `declarativeNetRequest` API to block—and immediately close—your chosen distractor websites in all tabs. Click again to restore normal browsing.

## Selling Points

1. **One‑Click Activation**: Instantly block distractions via the toolbar icon.  
2. **Network‑Level Blocking**: Prevents pages from loading, not just hiding them behind an overlay.  
3. **Auto‑Close Tabs**: Any open distractor tabs are closed as soon as Focus Mode is enabled.  
4. **Clear Visual Indicator**: A red “ON” badge on the icon shows when you’re in Focus Mode.  
5. **Customizable Blacklist**: Easily add or remove domains to fit your personal workflow.

## User Stories

1. **As a user**, I want to toggle Focus Mode on/off by clicking the extension icon so that I can quickly switch between work and browsing.  
2. **As a user**, I want any open Reddit, Twitter, or YouTube tabs to automatically close when Focus Mode is on so that I’m not tempted to reopen them.  
3. **As a user**, I want the extension to block loading of specified distractor sites in all new and existing tabs while Focus Mode is on so that I cannot bypass the block.  
4. **As a user**, I want a visible badge on the extension icon indicating when Focus Mode is active so that I always know my current focus status.  
5. **As a user**, I want to configure which websites are treated as distractions via a simple settings interface so that the extension fits my personal workflow.

## Notes

- **Potential Challenges**: Handling wildcard subdomains (e.g., `*.reddit.com`), syncing settings across devices, performance impact of dynamic rule updates.  
- **Alternative Approaches**: Overlay‑based blocking vs. network‑level blocking; integrating a Pomodoro timer for scheduled focus sessions.  
- **Future Enhancements**: Scheduled auto‑activation (e.g., 9 AM–5 PM work hours), emergency “unlock” with a cooldown timer.

## References & Inspiration

- Chrome Extension `declarativeNetRequest` API docs: https://developer.chrome.com/docs/extensions/reference/declarativeNetRequest/  
- StayFocusd (existing productivity extension)  
- Articles on digital minimalism and focus techniques  
