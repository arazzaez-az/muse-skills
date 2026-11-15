# Cloud browser pre-flight

## Check the blockers before you start

- Open the target page with `browser.browse` and read what it actually shows before you tell the user work is running.

- Look for a login wall, a captcha, a wallet connect button, a 429 or 403 response, and a loading error before you plan the next step.

- Treat a missing wallet extension in the cloud browser as a hard blocker for any task that needs a wallet signature or a wallet popup.

- Ask the user for the one missing piece only after you name the exact blocker, and name the exact step they would take on their own device.

## Prove the page works before you report progress

- Report only what the browser actually returned, and quote the error or the page state you saw.

- Wait until a page has loaded and the action you need is visible before you describe that action as in progress.

- Claim a screenshot, a file, or a completed action only after you hold the file or the confirmation in hand.

- If a tab reloads, crashes, or loses state, say so at once and start again from the load check instead of describing work that never happened.

## Stop a deterministic block and hand it over

- Stop retrying a deterministic block after one failed attempt and one different check, such as a fresh window or a different route.

- Treat a 429 or 403 response, a missing wallet extension, and a login wall with no credential as deterministic blocks that the same retry cannot fix.

- Allow fresh attempts at a human captcha, and stop after five identical captcha failures and report the block.

- Never promise to keep trying until a blocked task succeeds, and never schedule repeated reloads of a page that already returned the same block.

- Hand the task over with the exact address, the exact blocker, and the single step the user takes on their own device, then stop.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Alternatives for better results

- Offer a read-only check through a public API or explorer when the site itself blocks the browser.

- Offer to draft the text, the form entries, or the transaction details so the user pastes them in one step on their own device.

- Offer to retry later after a stated interval when the block is a rate limit with a known cooldown, and name that interval.
