# Kash Analytics — Dashboard Overview

A small, independent analytics dashboard built on top of the **public Kash API**.
It runs fully in the browser, uses no private keys or logins, and reads only public
data. The goal is simple: show useful things about Kash markets that the main app
does not show yet. It is a community tool — not affiliated with the Kash team.

Below is what each page does and why it is useful.

---

## Insights

**What it does:** It gives a "big picture" of the whole platform. It breaks volume
and trades down by category, shows how concentrated activity is in the top markets,
and puts the most-traded markets next to the highest-volume ones.

**Why it matters:** It helps anyone see, at a glance, where real attention and money
are going — which topics are alive, and which markets look active versus which just
look big. This kind of cross-market summary is not in the main app.

**In one line:** A clear overview of where the real engagement is across Kash.

---

## Resolution Calibration

**What it does:** Once markets are resolved, this page tests whether Kash's prices
were *accurate*. The idea is simple: markets priced at around 70% should turn out
"yes" about 70% of the time. It measures this and gives a single accuracy score
(a "Brier score": lower is better).

**Why it matters:** Accurate pricing and trustworthy resolution are the heart of any
prediction market. This page turns that promise into a number anyone can see. (Kash
is young and has few resolved markets so far, so this page fills in over time — it
honestly says so instead of showing a fake result.)

**In one line:** It checks, with real data, whether Kash's prices come true as often
as they should.

---

## 🎯 Consistency

**What it does:** For markets with many possible outcomes (like "Who will win the
2026 World Cup?"), it adds up the chances of all the outcomes. In a fair market they
should add up to exactly 100%.

**Why it matters:** It is a quick health check on the pricing engine. The result here
is a *good* sign for Kash: the outcomes add up to 100%, which means the market
maker prices everything in a mathematically clean way — there is no hidden extra
margin like a traditional bookmaker has. If the engine ever broke, this page would
catch it immediately.

**In one line:** It confirms Kash prices multi-outcome markets fairly and correctly.

---

## Markets

**What it does:** A simple, searchable list of all live markets. You can filter by
category and sort by volume, number of trades, probability, or which markets end
soonest. Each card links straight to the market on Kash.

**Why it matters:** It is a fast, clean way to browse and find markets — a handy
companion to everything above.

**In one line:** A quick, filterable directory of every live market.

---

## How it was built

Everything here is calculated live, in your browser, from the public Kash API only.
No logins, no private data, no special access. The whole dashboard is a single file
that anyone can open or host. It is meant as a friendly, useful add-on that makes
Kash's own data easier to understand and trust.
