---
name: scoping
description: Turn notes or a transcript from a client call into a milestone plan the client can agree to before any work starts. Use after a discovery or scoping call, or when asked to "write up the scope", "draft the milestones", or "turn these call notes into a plan".
---

# Scope from call notes

Goal: anything that would cause a disagreement at delivery gets settled here, in writing, in plain words the client can't misread. Most delivery pain traces back to scope and logistics that didn't get written down: the client pictured the finished, styled thing when you meant the working core, how it would be delivered went unsaid, or "done" didn't get defined.

## Input

Call notes or a transcript, plus anything the client already sent (job post, brief, files). Read all of it first, and don't ask the client anything their own materials already answer.

## Output

A milestone plan the client can read and agree to. For each milestone:

- **What it delivers**, in the client's own words.
- **Done means:** a short list of outcomes the client can check themselves.
- **Price** for that milestone.
- **Funded before it starts.** Each milestone is paid (or put in escrow) before work on it begins, so the deposit question answers itself.

Then, once for the whole plan:

- **Bug fixes:** anything delivered that doesn't do what the plan says gets fixed free for two weeks after delivery. New features or changes inside those two weeks are new work, not bug fixes. Give the window an end date.
- **Revisions:** a set number of rounds to match the agreed spec, then further changes are a new milestone.
- **How it's delivered:** a live preview link by default, a repo the client owns as the fallback.
- **What I need from you to start:** a bulleted list of only the things that can't move without the client (account access, keys, content, decisions). Anything you can do yourself isn't their task.
- **Close with the next step:** "Fund milestone 1 and I'll get started," not "let me know what you think."

Plain text, short, no jargon the client wouldn't use.

## Before a capability goes in "Done means"

1. **The acceptance test check.** Can you write the one sentence the client would sign? "Texts should work" fails. "A customer texts the business number, a draft reaches the owner within a minute, and on approval it's sent back to that customer" passes, and writing it forces the open questions (which number, drafted or sent automatically) into the open. If you can't write the sentence, ask.
2. **The unhappy path sweep.** The demo path isn't the whole scope. For each capability ask: what if it's a stranger instead of a customer, a wrong address, two requests at once, a returning customer, or the outside service is down? Each one you can't answer is a question for the client or a line on the "not included" list.
3. **Split bundled claims.** "Calls, texts, and email" is three deliverables wearing one line. Give each its own line and its own test, or mark it not included.

## Items that are more than one line

Break these into their parts and price them before quoting:

- **Email:** a sending provider, a verified sending domain (DNS records on a domain the client owns), and a working test send.
- **Writing to a CRM or payment system:** no duplicates if it runs twice, matching returning customers, field mapping, and login tokens that keep working.
- **"Match my designs":** take a typed change list, not an open-ended "make it look like this."
- **"Production ready" or "audit":** name what's checked and what's out of scope, or it doesn't end.
- **Moving off an old platform:** list what the old platform DOES (logins, payments, emails, what the owner can edit in its admin), not just the data it holds. The job with nothing visible to move is the one that goes missing.

## Settle before building

1. **Function vs design, explicitly.** "Milestone 1 = the working core, not yet styled. Milestone 2 = built to your designs." Have the client confirm it back.
2. **Account ownership.** The client owns every account the build runs on (hosting, database, phone provider, CRM). You're a collaborator during the build and get removed at handoff.
3. **Assets up front:** designs, branding, logins, keys, FAQs, whatever the build consumes. Chasing them during the build costs days.
4. **Email and texting as explicit questions.** Clients assume "the app emails people" and won't bring it up. Ask which events should send an email or text, and get every one decided now. Texting in the US needs carrier registration that takes days, so start it early.
5. **Check the risky core first.** If a formula or rule has to be right to the cent (pricing math, eligibility), confirm it against a worked example the client signs off on before building around it.
6. **Walk the main loop end to end before calling anything done.** For a directory: a new member can sign up, pay, and appear, and a visitor can find and contact them. Every page existing isn't the same as the loop working.

## When the client pushes on price

Cut scope, not price. Absorbing work to hold a number is how a fixed price turns into unpaid hours.
