# Chrome Extension Idea: CalNow

## Authors

Andrew Lukashchuk

## Problem Statement

Adding items to a calendar can be a disruptive and error-prone task, especially when it requires switching tabs and manually copying details. It’s easy to make mistakes and time-consuming to come up with accurate descriptions or event metadata. CalNow addresses this by leveraging LLMs to intelligently extract and summarize event details directly from the page a user is viewing—streamlining the entire process into a single click.

## Target Audience

CalNow is designed for a wide audience:
-  Students who frequently add academic deadlines and events to their calendars.
-  Professionals who need to quickly schedule meetings or events as they arise.
-  General users who want an easier way to track events they come across while browsing emails, websites, or social media.

## Description

CalNow is a Chrome extension that allows users to instantly convert webpage content into calendar events. It scans the current page for relevant details—like event name, date, time, and location—and uses AI to auto-fill the calendar entry form. Users can then review and save with just one click, significantly reducing time spent on scheduling.

## Selling Points

1.   One-Click Simplicity – Instantly add events without switching tabs or copying details.
2.   Automatic Detail Extraction – Uses AI to intelligently parse and pull event info from web pages.
3.   Time Efficiency – Saves users valuable time otherwise spent manually entering event data.
4.   External Calendar Support – Integrates seamlessly with Google Calendar, Outlook, and more.
5.   Verifiable & Customizable Input – Users can review and tweak event details before saving.

## User Stories

1.  As a busy professional, I want a one-click button to add events from any webpage so I can schedule meetings effortlessly without having to enter data manually.
2.  As a student, I want the extension to automatically detect event details from academic event pages so that I can quickly add them to my calendar for better schedule management.
3.  As an event organizer, I want to integrate the extension with my Google Calendar so that all my events sync across devices seamlessly.
4.  As a casual browser, I want to be able to customize extracted event details before saving so that I can make any necessary adjustments for accuracy.
5.  As a time-sensitive user, I want an automatic pop-up confirmation after adding an event so that I know my calendar has been successfully updated.

## Notes

Some websites may not follow standard formatting or may present event information as images, which can make automated extraction challenging.

## References & Inspiration

-  [Google Calendar Workspace](https://developers.google.com/workspace/calendar) will be required to have the calendar work with Google calendars
-  [Outlook API](https://learn.microsoft.com/en-us/outlook/rest/reference) will be required for integration with Outlook calendars
