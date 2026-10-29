# Before / after

Anonymized. No addresses, no hardware names, no site details.

## Before

- One flat LAN. Trusted devices, storage, IoT, and guests shared it.
- The architecture lived in chat notes and one-off scripts.
- After a reset, the model still "remembered" the old gateway and the old attachments.

## After

- Three segments: trusted, IoT, guest. IoT does not reach trusted unless an allow is written down.
- One diagram for zones, port roles, and a done/open checklist. Humans and the model read the same file.
- Constraints live in project rules. Chat is disposable.
- Work moved one block at a time: core, edge, cutover, isolation, then services. Each block was checked before the next started.

## What still failed

The diagram was wrong once (see [port-labels.md](port-labels.md)). A textbook interface name did not match the live packet path. Those misses stayed in the notes and the rules. They were not patched only in the chat.
