# Launchpad token research

## Verify holder distribution from the full event history

- Start from the token contract address and the block where the token was created.

- Collect every Transfer event from the creation block to the latest block through a public explorer API or an RPC endpoint.

- Sum the net balance for each address from those events and divide each top balance by total supply to get its share.

- Verify each top holder with a direct balance call at the latest block before you report its share.

- Never estimate a holder share from recent buyers or recent traders only.

- Treat a holder share as unverified until the full event check and the balance check both finish.

## Check activity, liftoff state and sellability

- Re-check graduation and liftoff progress immediately before a buy decision because a mission can graduate within minutes.

- Read the swap count and volume over the last hours and treat zero swaps as no activity even when the holder count looks healthy.

- Compare the current sell quote for the intended buy size across the candidate tokens and treat identical flat quotes as a sign of thin trading.

- Exclude graduated missions and tokens the user already holds unless the user says otherwise for that run.

- Apply any other exclusion the user gave for the run before you rank the candidates.

## Present a buy decision with verified figures only

- Report the top holder share, the top five holder share, the holder count, the swap activity and the liftoff progress for each candidate.

- Mark every figure as verified or unverified and name the check that verified it.

- Say plainly when a figure is still unverified instead of filling the gap with an estimate.

- Rank the candidates by verified figures only and name the single strongest reason for the top pick.

- Name the exact moment the scan was taken so a later reader can tell how stale it is.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Alternatives for better results

- Re-run the holder check and the sell quote right before signing when minutes have passed since the first scan.

- Ask the user for the intended buy size first when the sell quote depends on it.

- Skip a token when its full event history cannot be read instead of reporting an estimated holder share.
