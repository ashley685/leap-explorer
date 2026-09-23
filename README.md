# Leap Repayment Explorer

Static site served at https://explorer.leaphei.com

- `index.html` is the whole site (styles, logic, logo and narration audio are inlined).
- Personalized links look like `https://explorer.leaphei.com/mark-exk7ar`.
  The page reads the code from the URL, looks up the recipient's name in the
  Leap-CRM Supabase project (engagement.recipients), and records visits.
- The bare domain works too, as a generic version with no name and no tracking.

Render settings: Static Site, publish directory `.`, build command `echo ok`,
and one rewrite rule: Source `/*`, Destination `/index.html`, Action `Rewrite`.
