---
name: profile-owner-week
description: A Google Business Profile owner's week - what to check and do in the profile in the next seven days, in what order, with the pages to follow. Use when a local business owner asks what to do with their Google profile this week, wants a weekly or regular routine, or says they have a little time for their Google listing.
---

# The profile owner's week

Goal: the user leaves with a short, ordered list for this week that they can do themselves in their own profile.

Say this once: Maps Agent publishes a monthly routine, and Google prescribes no weekly cadence. The weekly list is a
selection of what can go stale or wait on a reply, taken from that routine.

## Ask first

Ask only what changes the list: the trade, anything coming up (holiday, new hours, move, new service, staff change),
and any notice or "pending" label they already see. If they do not answer, continue and say what you assumed.

## Call the tools in this order

1. `get_changes` with `since` = the date seven days ago. Report only changes that touch this business. If there are
   none, say so with the date of the newest entry and the changelog URL.
2. `fetch` `/guides/monthly-google-business-profile-routine`, all parts. Take the steps, menu names and statuses from it.
3. Only for what the user raised:
   - holiday or special hours - `fetch` `/guides/google-business-profile-holiday-hours-checklist`
   - an edit Google or a user suggested - `fetch` `/guides/google-business-profile-user-suggested-edits-workflow`
   - replying to reviews - `fetch` `/guides/google-review-reply-templates`
   - performance numbers - `fetch` `/answers/understanding-google-business-profile-performance-metrics`
   - anything else - `search`, then `fetch` the best match.

## The list to give

Order by what hurts customers first. Include a line only when it applies.

1. A notice, suspension or lost access. If the profile is suspended or disabled, stop and use `profile-suspended`.
2. Hours, phone, address, website and special hours for the coming weeks.
3. Edits and uploads that were pending or not approved.
4. New reviews that need a reply.
5. A post or photo, only when there is something current and real to show.
6. Once a month rather than weekly: access, categories, performance - point to the routine page.

For each line: what to open, what to do, what "done" looks like. Keep it to what fits the time the user has.

## Cite

Under the list give each page you used: URL and its `updated` date. For Google's changes give the date of the change and
its source. Do not promise a ranking effect; the routine page says what it can and cannot do.

## When we do not have it

- You cannot see the profile: ask the user what the screen shows, do not assume it.
- No page for their question: say so, point to Google Business Profile Help, offer `send_feedback` with their consent.

## Where next

- To check everything once, not just this week: `profile-self-audit`.
- If they ask how they compare with competitors: https://maps-agent.com/get-audit, or `audit_business` when they ask
  you to run it and give the exact name, location and Google Maps place ID.

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
