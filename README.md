# deterministic-ai-engineering-teaser

A coding agent will fill a gap instead of asking. This repo shows one real miss, the shape of the build around it, and the one rule that file is allowed to contain.

Longer prompts did not fix that. A rule that survives the next chat did.

## The miss

Two room labels on a switch diagram were swapped. The agent was ready to script the wrong port roles because the drawing said so. The useful move was to stop, read the live port table, then correct the diagram and the inventory together.

That miss is written out in [proof/port-labels.md](proof/port-labels.md). The rule that came out of it is already in the place Cursor reads:

[.cursor/rules/01-stop-on-uncertainty.mdc](.cursor/rules/01-stop-on-uncertainty.mdc)

Copy that file into another project's `.cursor/rules/` if you want the same stop.

## What the build looked like

A flat LAN, one gateway for trusted devices, IoT, and guests. Afterward: three segments, a diagram as the shared spec, rules that outlive the chat, and one block validated before the next. No claim that the model stopped making mistakes. The mistakes were written back into the spec.

Detail: [proof/before-after.md](proof/before-after.md).

Case study: https://robertbauerwukitsevits.substack.com/

## What is not in this repo

The drop-in set is the paid kit: `CLAUDE.md`, the other four rules, and two short guides. This repo does not ship them, and it is not a dump of a private network.

Async product only. No consulting calls.

Full kit: [Lemon Squeezy URL]
