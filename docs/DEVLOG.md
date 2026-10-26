# GuildChatAI — development record

**Author:** Babuni.dev

## Retrospective source reconstruction — 2026-10-26

The repository preserves a small, focused WoW experiment. A guild-chat logging experiment that stores guild chat messages and guild-roster names and exposes `/gcai` to send a supplied message to guild chat. Explore using guild chat as a record and possible interface for later AI-assisted interaction. The visible implementation supplies the clearest record of how the interaction was approached: `GuildChatAI.lua` registers `ADDON_LOADED`, `CHAT_MSG_GUILD`, and `GUILD_ROSTER_UPDATE`, writes into `GuildChatAIDB` and prints captured messages; `/gcai` forwards user-provided text to guild chat. `GuildChatAI.toc` declares interface 11200.

This is a retrospective reconstruction, not a transcript of original design discussions. The current code performs message capture and transmission; no external language model call, AI generation, or working integration bridge is present in the inspected source. Its source and metadata existed before the current documentation pass; original conception and iteration dates are not recoverable from these files alone. In this pass, AI assistance organized the existing evidence into documentation, without changing gameplay or attributing the original idea to AI.

## Verification

Evidence: current `README.md`, addon `.toc` metadata and inspected main `.lua` source; no full historical conversation or runtime test was available. Test against the declared WoW client version; inspect API and Lua syntax compatibility, timestamp formatting and guild-roster event behavior; do not claim that an AI bot is implemented.
