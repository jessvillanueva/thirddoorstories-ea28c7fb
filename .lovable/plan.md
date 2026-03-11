

## Make the "Unlatched" Newsletter More Explicit

The current `EmailCaptureBar` is generic — it just says "Get early access to new episodes and essays. No spam." There's no mention of the newsletter name "Unlatched" or what it actually is.

### Changes to `src/components/EmailCaptureBar.tsx`

Update the copy to explicitly brand it as the **Unlatched** newsletter:

- Add a bold title: **"Unlatched"** (the newsletter name)
- Add a tagline pulled from the Beehiiv page: "Investigating the hidden paths young builders take when college and hustle culture aren't always the answer."
- Keep the subscribe form and existing functionality unchanged
- Add a small link to the Beehiiv archive page so people can preview past issues

The updated layout:
```text
┌─────────────────────────────────────────────────┐
│  Unlatched — The Newsletter                     │
│  Investigating the hidden paths young builders  │
│  take when college and hustle culture aren't     │
│  always the answer. No spam.                    │
│                                                 │
│  [your@email.com          ] [Subscribe]         │
│                                                 │
│  Read past issues →                             │
└─────────────────────────────────────────────────┘
```

This is a single-file change to `EmailCaptureBar.tsx` — the component is already used in the footer site-wide, so the branding will propagate everywhere.

