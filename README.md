# telegram-report

A one-tap abuse report page. Opens the visitor's mail app with the report
email to `abuse@telegram.org` pre-filled — To, Subject and Body — so the
reporter only has to press Send.

## Live

https://shadow01cyber.github.io/telegram-report/

## How it works

- A `mailto:` link built with `encodeURIComponent` carries the full report.
- On page load it tries to open the mail app automatically (~0.7s delay).
- The sticky button is the fallback if auto-open is blocked.
- The full email body is rendered on the page for transparency.
