# BUILD-A-CHROME-EXTENSION-FOR-PRODUCTIVITY-MANAGEMENT

COMPANY: CODTECH IT SOLUTIONS

NAME: KAVIYATHAMIZHAN T K

INTERN ID: CT08WC44

DOMAIN: MERN STACK WEB DEVELOPMENT

DURATION: 8 WEEEKS

MENTOR: NEELA SANTOSH

DESCRIPTION : 

Overview: The Productivity Tracker Chrome Extension is a lightweight browser tool designed to help users monitor and manage their web activity. Built using HTML, CSS, JavaScript, and Chrome Extension APIs, this extension allows users to track the amount of time spent on different websites, block distracting domains, and view daily productivity reports — all locally without needing an internet connection or backend database.

Features
Website Activity Tracking
The Chrome extension listens for tab changes and captures the domain of the active website. When users switch between tabs or change browser focus, the extension logs the amount of time spent on each site. This data is stored locally and sent periodically to the backend server for persistent logging and analytics.

Distraction Blocking
Users can define a personalized list of distracting websites (e.g., facebook.com, youtube.com, reddit.com). Once added to the block list, the extension intercepts navigation attempts to those domains and redirects users to a custom “Blocked Site” page. This helps users stay focused during work or study sessions

Helps improve focus and prevent procrastination.

Daily Productivity Reports
Every day, the backend aggregates usage data and produces a summary of time spent across all tracked domains. Users can view reports highlighting:

Top visited websites

Total time spent online

Breakdown of productive vs unproductive time

Time-wasting trends over the week

This allows users to identify problematic patterns and adjust their behavior accordingly.
Data is visualized in a clean interface for quick analysis.

Reports reset daily, encouraging consistent productivity.

Offline Support: Works entirely in the browser with no external server or database.

Stores data using localStorage for privacy and simplicity.

Technology Stack
Chrome Extension (Frontend):
JavaScript: Core logic and interactions

HTML/CSS: UI for popup, options, and blocked pages

Chrome Extension APIs: tabs, storage, webNavigation for tracking and control

JavaScript: Handles time tracking, blocking logic, and data processing.

Chrome Extension APIs: Enables interaction with browser tabs, tracking activity, and managing local data storage.

How It Works: 

The extension detects when a user switches tabs or visits a new website.

It records the active time spent and sends a POST request to the backend.

If the site is in the block list, it automatically redirects the user to a warning screen.

The backend stores logs and preferences tied to the user account.

At any time, the user can open the popup to view a summary or access the full report.

A daily report endpoint aggregates usage statistics using MongoDB queries and returns insightful summaries.

Tracking Usage: The background script detects when a tab is active or switched.

It records the time a domain is visited and updates the stored data accordingly.

Blocking Distractions: A predefined list of blocked sites is compared with the current tab’s URL.

If a match is found, the site is either closed or redirected to a custom warning page.

Displaying Reports: The popup (popup.html) fetches time-tracking data from localStorage.

It displays a summary of top visited sites and time spent.

Potential Enhancements: Sync Across Devices: Use Chrome Sync API to maintain consistency between multiple browsers.

Custom Timers: Let users set work/break intervals using a Pomodoro-style timer.

Notifications: Alert users when they’ve spent too much time on a specific site.

Graphical Analytics: Add charts for visual time breakdowns using Chart.js or similar.

Future Enhancements
Weekly email reports using NodeMailer + Cron

Integration with Google Calendar or Notion

Machine learning to classify sites as productive/unproductive

Dark mode + enhanced UI/UX

Mobile extension support for Android (via Kiwi browser)



Conclusion: Conclusion
This project demonstrates how browser-based tools combined with a robust backend architecture can effectively help users reclaim their focus and manage digital distractions. It integrates real-time monitoring with a user-friendly interface and secure cloud storage, making it an excellent productivity companion and a solid portfolio piece that showcases practical use of Chrome Extension APIs,and client-server communication via RESTful APIs.

OUTPUT : 
![Image](https://github.com/user-attachments/assets/c3821814-c6e9-4e01-b44d-69c49a769ebc)
