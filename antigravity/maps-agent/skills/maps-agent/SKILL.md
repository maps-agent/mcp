---
name: maps-agent
description: Google Business Profile and Google Maps knowledge from Maps Agent - answers, guides, glossary, research and Google's dated changes, each with its page. The general entry for any question about a local business's profile or its visibility in Google Maps - reviews, categories, photos, posts, local SEO terms, what the research says, Maps Agent plans. For a weekly routine, a suspended profile or a profile check, use the scenario skill it names.
---

# Maps Agent

What Maps Agent has published about Google Business Profile and Google Maps for local businesses. The server reads
public pages. It does not see the user's account: no tool opens or edits a profile.

## Start with a scenario when one fits

| The user wants | Skill |
| --- | --- |
| to know what to do with the profile this week | `profile-owner-week` |
| help with a suspended or disabled profile, or an appeal | `profile-suspended` |
| to check their own profile item by item | `profile-self-audit` |

## Which tool to call

- `search` - start here: a question in plain words returns matching pages with id, date and URL.
- `fetch` - read a page in full (pass the id, URL or path). A long page comes in parts: when `total_parts` is above 1,
  read the other parts with `part` before you summarise steps.
- `list_articles` - what exists in one form (answer, guide, research, glossary, blog, industry, comparison, changelog,
  page), optionally by topic.
- `define_term` - a local SEO term in plain words.
- `get_research` - one study with its method, sample, window and sources.
- `get_checklist` - a published checklist or template for a profile task, in full (pass the task in plain words; no
  topic lists them all).
- `get_ranking_factors` - Maps Agent's summary of what moves a place in Google Maps (`scope` maps) or into AI answers
  (`scope` ai_answers). When it says the summary is not published yet, read the closest pages it returns.
- `find_categories` - Google's official US English category names for a trade, with the date they were read.
- `get_changes` - what Google changed in profiles, Maps and local search since a day.
- `get_plans` - Maps Agent plans, prices and whether places are open. Only when the user asks about the service.
- `audit_business` - starts a free visibility audit of one business. Only when the user asks for it; it needs the exact
  name, location and Google Maps place ID.
- `send_feedback` - tell Maps Agent what was missing or wrong. Only with the user's consent, without personal details.

## How to cite

- Give the page URL for every statement you take from a page, and the page's `updated` date.
- A page lists its own sources (`sources`). When the rule is Google's, name Google's page and link it too.
- A figure from a study: name the study and its sample and window. Do not turn it into a promise.
- Separate what the page says from your own advice about the user's case.

## When we do not have it

If `search` returns nothing that answers the question, say that Maps Agent has no published page on it. Do not fill the
gap with a guess presented as ours. Point to Google's help or support, and offer to send the gap with `send_feedback`.

No sign-in or key. Terms: https://maps-agent.com/terms.

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
