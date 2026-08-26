# HELD - Communist Sightseeing — legal documents

Public hosting for the two documents Google Play requires to be reachable at a
stable URL: the privacy policy (needed in the store listing *and* linked from
inside the app) and the account-deletion instructions (needed for the Data
safety form).

Served by GitHub Pages at:

- https://mkern72.github.io/communist-sightseeing-legal/privacy-policy
- https://mkern72.github.io/communist-sightseeing-legal/account-deletion

## Why this is a separate repository

The app's own repository is private, and GitHub Pages does not serve private
repositories on a free plan — which is the only reason these pages do not live
alongside the app.

It is also deliberately **not** named after the app. A project site for a repo
named `communist-sightseeing` would serve at
`mkern72.github.io/communist-sightseeing/`, so if that repository is ever made
public with Pages enabled, it would claim the same path and silently shadow
these URLs. The distinct name makes that collision impossible.

## Editing

These pages are **generated**, not authored here. The source of truth is
`docs/legal/*.md` in the app repository; edit there first, then update the HTML
here to match. The two must not drift — the app links to these URLs at runtime
from the Profile tab, and the same URLs are recorded in the Play Console forms,
so a change made in only one place is a change users and reviewers see
differently.

`.nojekyll` is present so GitHub Pages serves these files verbatim rather than
running them through Jekyll.
