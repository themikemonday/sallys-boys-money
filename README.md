# Sally's Boys' Money

A small, private record of what each of two (or more) kids has, and where it went. One self-contained HTML file — no install, no account, no server, no tracking. Everything typed into it stays in the browser on the device it was typed on.

Built for one parent's iPhone, works anywhere.

**[Open it](https://themikemonday.github.io/sallys-boys-money/)** · Add to Home Screen for the full-screen version.

---

## What it's for

The problem this solves is an ordinary one: kids have money that comes and goes — birthday cash, a bit for chores, something spent on Lego or a bike helmet — and without a record, nobody can say with confidence what's actually left, or what a balance is made of. It ends up as a guess, or an argument about who remembers correctly.

So this app has one job: for each kid, keep a running total of what he has, built entry by entry, with the history underneath it so the number is never just asserted — it's always the sum of a story you can scroll back through.

One parent records the entries. It isn't a shared ledger the kids edit themselves, and it isn't a budgeting app with categories or goals — it's the plain arithmetic a spreadsheet would do, made faster to open than a spreadsheet.

## What's in it

**Home** — a card for each kid with his current balance in Australian dollars. Tap one to see his history.

**A kid's screen** — his balance at the top, big and clear (a balance below zero shows in red — it isn't blocked, just shown honestly), then **Money in** and **Money out** buttons, then his history underneath, newest first: date, note, the amount, and the balance right after that entry. Tap any entry to edit it or delete it — deleting asks for confirmation in the page itself, never a browser pop-up.

**Manage boys** — add a name, rename one, or remove one. No names are hardcoded anywhere in this file; whoever uses the app types them in once, and they live only in that browser's storage.

Money is kept as whole cents internally, so long-running totals never drift by a cent the way repeated decimal arithmetic can.

## What it deliberately doesn't have

- **No categories, budgets, or spending limits.** It's a record, not a planner.
- **No charts or goals.** A balance and a history are the whole picture.
- **No automatic allowance or pocket money.** Every entry is typed in by hand, on purpose.
- **No accounts, no sync, no login.** One phone, one person recording.
- **No server of any kind.** Nothing here is ever sent anywhere.

## Your data

It lives in this browser's local storage, on this device. There is no server and no account, so:

- **Back up / restore**, under Back up / restore on the home screen, saves a file you keep and can load back in.
- On iOS, a Home Screen app gets **separate storage from Safari** — so one can look empty while the other is full. Nothing has been deleted. **Copy all my data** and **Paste data in**, both in the same place, move it across between the two.

This repository holds the app and nothing else. No family's actual money records are in it.

## Technical

One HTML file, no dependencies and no build step. Vanilla JS, `localStorage` with a prefix unique to this app (`themikemonday.github.io` serves several small apps from one origin, so each keeps to its own storage key). Works offline and opens straight from disk. Light and dark follow the system, via `prefers-color-scheme`.

---

Built at home for one family, and shared in case the shape is useful to someone else. There's no support and no roadmap.
