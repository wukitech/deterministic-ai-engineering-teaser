# One miss — swapped port labels

The diagram named two rooms on two switch ports. The labels were swapped. Nothing in the chat looked wrong, because the drawing was treated as the source.

The next change was about to follow those labels into a script.

What actually helped:

1. Stop. Do not implement from a label that has not been checked.
2. Read the live port table.
3. Update the diagram and the inventory in the same pass, after the live read.

"I think this port is the office" is not a source. A live table is. The rule in `.cursor/rules/01-stop-on-uncertainty.mdc` is that check, written so the next chat still has it.
