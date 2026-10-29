# Stop on uncertainty

You implement against a visual architecture spec and the one rule in `.cursor/rules/01-stop-on-uncertainty.mdc`. Chat history is not the source of truth.

This file matches that public rule only. It does not include the rest of the doctrine set.

Set these two paths before the first implementation block. If either path is still a placeholder, stop and ask. Do not guess a file.

- Architecture diagram: `PATH/TO/architecture.drawio`
- Versioned inventory: `PATH/TO/inventory.md`

## How to work

1. Read the diagram and the inventory for the block you were asked to do. If they disagree, stop. Do not pick a side from memory.
2. If you lack a sourced fact, or you must choose between valid alternatives: **stop, ask, do not implement.**
3. A sourced fact is a line in the inventory, a label on the diagram that was checked against a live read, or a statement in this chat that cites one of those. "Probably", "usually", and a textbook example are not sources.
4. Do not invent hosts, addresses, port roles, segment membership, interface names, or libraries.
5. When a label was wrong, sharpen `.cursor/rules/01-stop-on-uncertainty.mdc`. A correction that exists only in chat is not done.

The miss that produced this rule is in `proof/port-labels.md`.
