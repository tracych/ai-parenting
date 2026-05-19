# Conversation Spark

A small, warm tool for parents: replace "How was school?" with questions that actually get real answers.

## What it is

A curated bank of ~300 conversation-starter questions for parents and kids, tagged by:

- **Age band:** 4-6, 7-9, 10-12, 13-16
- **Situation:** car ride, dinner, bedtime, hard day, lazy morning, walk together, before a big event, after a big event
- **Depth:** light (curious / silly), medium (reflective), deep (values / identity)
- **Theme:** friendship, fears, gratitude, dreams, school, family, world, creativity, mistakes, kindness

You pick the moment. The tool deals you three cards. You ask one. You and your kid have an actual conversation.

## Who it's for

Parents and caregivers of kids ages 4-16. The tool stays warm and inviting (not clinical) and never assumes a particular family shape, culture, or gender setup.

## Why it helps

- Most "check-in" questions get one-word answers. Specific, surprising questions get real ones.
- The recency engine remembers what it has already shown you (in this browser) and won't repeat a question for 14 days, so dinner doesn't get repetitive.
- A streak tracker gently rewards the habit of asking *something* every day.
- Favorites and Used-recently pages help you remember what worked.

## How to use

1. Open `index.html` in any modern browser.
2. Pick your kid's **age band** and the **situation** you're in. Optionally narrow by depth or theme.
3. Tap **Spark 3 questions**. Three cards flip up.
4. For each card:
   - **Save** the ones you love (they show up in Favorites).
   - **Used today** marks a question as actually asked — it also bumps your streak.
   - **Swap this one** replaces just that card.
5. Tap **Reshuffle** for three new ones in the same filter.
6. Check **Favorites** and **Used recently** in the top nav.

All data — favorites, used history, streak — lives in your browser's local storage. Nothing is sent anywhere.

## Optional: BYO API key (custom context)

There's an optional panel at the bottom of the Start page. You can paste your own Anthropic API key and a one-line context (e.g. *"kid had a rough day at recess"*) and get a single custom question tailored to the moment.

- This is **optional**. The tool is fully usable without it.
- Your key is stored only in your browser's local storage and is sent directly from your browser to Anthropic. It is never sent to any other server.
- Uses the `claude-3-5-haiku-latest` model with a tight prompt aimed at a warm, age-appropriate, invitation-style question.

## Design principles for the question bank

- Invitations, never interrogations.
- Avoid prying or clinical phrasing that could hurt a struggling kid.
- Don't assume a specific family setup.
- Mix curiosity, silliness, gratitude, and depth — kids need all of it.

## Run it

No build step, no dependencies, no internet required (unless you use the optional BYO-key panel).

```
open conversation-spark/index.html
```

Or just double-click the file.
