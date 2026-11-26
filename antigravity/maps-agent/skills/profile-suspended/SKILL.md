---
name: profile-suspended
description: Step by step help with a suspended or disabled Google Business Profile - find which restriction it is, prepare, appeal once, follow the status. Use when a business says its Google profile or listing was suspended, disabled, restricted, removed or disappeared after a notice, or asks about reinstatement, an appeal, a pending or denied appeal.
---

# The profile is suspended

Goal: the user knows which state they are in, what to do next themselves, and what not to do.

## Say this before anything else

Do not create a new profile for the same business, and do not send a second appeal for the same issue while one is
waiting for a decision. Both are in the appeal checklist - cite it. Add no reasons or consequences the page does not give.

## Answer in the first reply

Do not hold the steps back until the user has answered questions. With what they told you, pick the page, read it, give
the steps, and then ask only what could change them. Suspended and not appealed yet is enough: use the appeal checklist.

## Find the state

What decides the route: the exact words of the notice or status; whether the profile still shows on
Google Maps when signed out; whether other profiles on the same Google account are affected; the country (appeal routes
differ for the UK and EEA); whether an appeal was already sent and what status it shows.

| What they see | Read |
| --- | --- |
| not sure it is a suspension (missing, can't manage, verification asked) | `/answers/fixing-your-google-business-profile-when-it-breaks-or-is-suspended` |
| visible on Maps but cannot be managed, or "soft / hard suspension" | `/answers/what-is-a-soft-google-business-profile-suspension` |
| the Google account itself is restricted, or several profiles at once | `/guides/restricted-google-account-business-profiles` |
| suspended or disabled, not appealed yet | `/guides/google-business-profile-suspension-appeal-checklist` |
| appeal shows Submitted for too long | `/guides/google-business-profile-appeal-still-pending` |
| "Can't be appealed" | `/guides/google-business-profile-appeal-cannot-be-appealed` |
| approved, still no access or not public | `/guides/google-business-profile-access-disabled-after-approved-appeal` |
| suspended again after reinstatement | `/guides/google-business-profile-suspended-again-after-reinstatement` |
| virtual office or P.O. Box | `/guides/google-business-profile-suspended-for-virtual-office-or-po-box` |
| someone else took the profile over | `/guides/recover-hijacked-google-business-profile` |

## Call the tools

1. `fetch` the page for their state. The result has `total_parts`: call `fetch` again with `part` = 2, 3 and so on
   until you have read them all, before you write the answer. Do not answer from the title or a search snippet.
2. Anything the table misses: `search` with their notice in plain words, then `fetch`.
3. A term they do not know (reinstatement, appeal status): `define_term`.
4. `get_changes` with `since` about 90 days back, when the question is whether Google changed something recently.

## The answer

1. The state, as they described it, and what it does not yet prove.
2. The next steps in order: read the reason and policy link Google shows; account restriction first if there is one;
   make the profile follow the guidelines; gather evidence that matches the profile; submit one appeal in the official
   tool; record the date and the status; the route after a denial.
3. A short record for them to fill in (notice, policy link, what was fixed, files, date sent, status).
4. What not to do.

Give time limits exactly as the page states them, with the page's date. Never predict that the appeal will succeed or
guess the reason Google did not show.

## Cite

Each step carries the Maps Agent page URL and its `updated` date; link Google's help page from the page's `sources` for
the rule itself and for the appeal tool.

## When we do not have it

- Maps Agent cannot contact Google, file the appeal or see why Google acted. Say so.
- A notice or case with no matching page: say there is no published page for it, send them to Google Business Profile
  support (`/guides/contact-google-business-profile-support` explains how), and offer `send_feedback` with their
  consent and without business or personal details.

Do not offer `audit_business` or plans while the profile is suspended unless the user asks.

## Tools

| Tool | Purpose |
| --- | --- |
| `search` | Search Maps Agent knowledge |
| `fetch` | Read a page in full |
| `list_articles` | List published pages |
| `define_term` | Define a local SEO term |
| `get_research` | Read a study with its method |
| `get_ranking_factors` | What moves a place in Google Maps and AI answers |
| `get_checklist` | Get a checklist or template |
| `find_categories` | Find Google Business Profile categories |
| `get_changes` | What Google changed |
| `get_plans` | Maps Agent plans and prices |
| `audit_business` | Audit a business on Google Maps |
| `send_feedback` | Send Maps Agent feedback |
