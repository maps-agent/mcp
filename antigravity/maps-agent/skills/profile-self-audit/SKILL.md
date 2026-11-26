---
name: profile-self-audit
description: Walk a business owner through checking their own Google Business Profile against a checklist, item by item, and end with a fix list. Use when someone asks to audit, review or check their Google Business Profile or Google Maps listing, wants a checklist, or asks what is wrong or missing in their profile.
---

# Check your own profile, item by item

Goal: the owner goes through their profile and ends with Pass / Fix / N/A for each area and an ordered fix list.
You do not see the profile: every mark comes from what the user reports.

## Call the tools in this order

1. `fetch` `/guides/google-business-profile-audit-checklist`, every part (`total_parts`). It is the checklist and it
   says what to fix first.
2. If the user wants only one area, use its own checklist instead:
   - categories - `/guides/google-business-profile-category-audit-checklist`, and `find_categories` for Google's
     official names for their trade (US English; give the date the tool returns)
   - links and buttons - `/guides/google-business-profile-links-and-actions-audit`
   - service areas - `/guides/google-business-profile-service-area-audit`
   - duplicates - `/guides/google-business-profile-duplicate-listing-cleanup-checklist`
3. Their trade: `list_articles` with `form` = `industry` and `topic` = the trade; `fetch` a page if one exists.
4. A doubt about one rule: `search`, then `fetch`. A term: `define_term`.
5. A question about what affects ranking: `fetch` `/answers/what-are-googles-local-ranking-factors`. Give what Google
   says. Numbers from surveys or studies are opinion or measurement: name the study. Maps Agent publishes no weights
   for the user's profile.

## Run it as a conversation

Do not paste the whole checklist. Take one area at a time in the page's order, ask a few concrete questions with where
to look, mark Pass / Fix / N/A, move on. Unanswered stays "not checked", never Pass.

If the profile turns out to be suspended or disabled, stop and use `profile-suspended`.

## The result

1. A table: area, mark, what was observed.
2. The fix list, ordered as the page's "what to fix first" table.
3. What was not checked.

Do not invent a score. The page's own warnings (no keywords in the business name, no duplicate profile, and the rest)
apply to every fix you suggest.

## Cite

Give the checklist URL and its `updated` date, plus the page behind any extra rule. Link Google's help page from
`sources` where the rule is Google's.

## When we do not have it

If an area or trade has no page, say so, do not make up a requirement, and offer `send_feedback` with their consent.

## Where next

- Regular upkeep: `profile-owner-week`.
- A view of how they stand against nearby competitors is a different thing from this checklist: the free audit at
  https://maps-agent.com/get-audit, or `audit_business` when they ask and give the exact name, location and Google Maps
  place ID.

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
