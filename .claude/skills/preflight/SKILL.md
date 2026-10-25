---
name: preflight
description: Check this laptop is ready for the Techella gameshow (Git, Node.js, this repo, GitHub connection) and help fix anything that isn't. Use when the user says "preflight", "am I ready", "check my setup", "is my laptop ready for the workshop", or invokes /preflight.
---

# Preflight — are you ready for the Gameshow?

The person running this may never have used a terminal. Be warm, plain-English, and brief. No jargon without a one-line explanation.

## Steps

1. Run the check from the repo root:

   ```bash
   bash scripts/preflight.sh
   ```

   If that fails because you're not in the repo, find the `techella-unlikely-gameshow` folder (usually in Documents) and run it from there.

2. Turn the output into a short checklist for the person:
   - ✅ for PASS, ⚠️ for WARN, ❌ for FAIL, ℹ️ for INFO
   - One line each, in plain English (e.g. "Node.js: installed" not "node v22.1.0 detected")

3. For each ❌ or ⚠️, explain what it means in one sentence, then **offer to fix it**:
   - **Things you can fix yourself:** set the Git name/email (ask for their name and email first, never make them up), run `git pull`, restore missing folders with `git checkout -- .`.
   - **Things they must do:** installing Git or Node.js. Give the exact link from the script's fix line and the one choice to make (e.g. "pick the LTS button"). Don't try to run installers yourself.

4. After fixing anything, run the script again to confirm.

5. Finish with one line:
   - All PASS → "You're ready for the Gameshow. See you at Techella!"
   - Only WARN → "You're ready. The ⚠️ items are nice-to-haves."
   - Any FAIL → what's left, and "If you can't fix it before the day, come anyway: you can vote on your phone and follow on screen."

## Don't

- Don't install anything with admin/sudo rights.
- Don't ask for or touch API keys, passwords or GitHub tokens. Following along needs none.
- Don't change any files in the repo except restoring missing folders.
