---
name: lwb
description: Loads Kristian's LWB paid-ads working context from his Google Drive LIS folder before doing any LWB work. Use this WHENEVER a session mentions LWB, Legacy Wealth Blueprint, Preston Seo, the ad map, the tax/wealth webinar funnel, cost per booked call, opt-in rate, CPL, Hyros, ClickFunnels leads, creative tests, hook rate, ad copy or script batches, landing pages like /future /tsn /fbmasterclass, or any Meta ads analysis, reporting, scaling, or killing decision for this account. Trigger it on the FIRST such message, before analyzing, writing, or recommending anything, even when Kristian does not name it and even if the request looks small. Without it the session will use Meta's numbers instead of the real ones and will repeat theories that were already tested and retracted. When in doubt, assume it applies.
---

# LWB session bootstrap

Kristian runs paid acquisition for LWB (Legacy Wealth Blueprint), Preston Seo's high-ticket tax and wealth education. The full working context lives in his Google Drive, in the `LIS` folder. Load it first. Do not ask him to paste it.

## Step 1 — find the folder

The LIS folder id is `11-mXZ5iXnj8C2OgN93afww47krZ0x_yk`. List it:

```
parentId = '11-mXZ5iXnj8C2OgN93afww47krZ0x_yk'
```

Use the Google Drive connector's `search_files`, then fetch contents with `download_file_content` and base64-decode. Note that `read_file_content` does NOT support `text/markdown`, so use the download tool for these files. If the Drive connector is unavailable, check whether his device is connected and read the same folder at
`/Users/thekrisivanov/Library/CloudStorage/GoogleDrive-kristian@influetize.com/My Drive/LIS`.
If neither is reachable, say so in one line and ask him to attach `README.md` and the newest handoff. Do not proceed on guesses.

## Step 2 — read these three files

**`00-START-HERE.md`** is the pointer file and confirms the read order. Then:

1. **`README.md`** — the creative and voice system: hook grammar, script architecture, the voice rules he enforces line by line, honesty and compliance beats, casting from the wealth-plan library, what concept types work vs die, the performance truth layer, the Eli consultant operating rules, the variable-stacking law, and competitor script appendices. Required before writing any ad, hook, script, or landing-page copy.

2. **The newest `LWB-CONTEXT-HANDOFF-YYYY-MM-DD.md`** — the account and performance state: economics and the cost-per-call floor, the measurement hierarchy, targeting facts, current baselines, every finding and every retracted theory from the last session, the full data arrays, the PDF build stack, and the open work queue in priority order. Required before any analysis, any kill/scale call, or any reporting.

   Sort by the date in the filename and read the newest one only. Older handoffs are history, not state.

3. **The newest `LWB-CREATIVE-DIVERSITY-YYYY-MM-DD.md`** — the creative diversity rules from the Sep 22 Eli call: the ads are too similar (same talking-head format, only the first 5 seconds change), so Meta keeps reaching the same people and CPMs stay high. Holds the format lanes (b-roll, AI ads, AI UGC, real UGC, new settings, document walkthrough), the per-ad rules, the hiring plan and Kristian's role as creative lead. Required before writing, briefing or reviewing any new ad, hook, script or batch, for the webinar or the challenge.

Pull other files in the folder only when the task points at one. They are dated artifacts: script batches, copy sets, reports, launch maps, landing-page briefs.

## Step 3 — work under these rules

These are in the handoff in full. They are repeated here because getting them wrong invalidates the output:

- **Every new ad changes the format, not just the hook.** Name the format lane, the avatar and the one new variable on every ad. A new hook on the same talking-head video is not a new test. The priority now is better, more diverse creative.
- **Cost per booked call comes from Hyros only.** Never from Meta. It is the only kill/scale metric. CPL is telemetry.
- **Lead truth comes from ClickFunnels/CRM**, matched per ad by unique `utm_campaign`. Meta over-reports leads non-uniformly by cell, so Meta's own LP CR column ranks cells in the wrong order.
- **True opt-in = CF leads / Meta LP views. True CPL = spend / CF leads.**
- **Never infer budgets from spend.** Read them off a screenshot or ask.
- **Compute every published figure from the data arrays.** Do not hand-type numbers into prose. That is what produced the published errors he had to correct.
- **One new variable per test cell.**
- **Windows of different length are not comparable in absolutes.** Per-day and rate metrics only.
- Writing style: short. Tables plus two-sentence captions, not essays. No em dashes in ad copy. Do not agree with a claim that does not hold up, including his.

## Step 4 — leave state behind

At the end of a working session, write a NEW `LWB-CONTEXT-HANDOFF-YYYY-MM-DD.md` into the LIS folder. The Drive API in these sessions can create but not overwrite, so never try to edit the previous handoff, and never upload a second `README.md` (a duplicate breaks the read order). README changes go through the synced folder on his Mac or the device bridge.
