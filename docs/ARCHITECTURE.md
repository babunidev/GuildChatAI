# GuildChatAI — architecture snapshot

**Author:** Babuni.dev

## File inventory

`GuildChatAI.lua`, `GuildChatAI.toc`, `README.md`, `LICENSE`

## Observed implementation

`GuildChatAI.lua` registers `ADDON_LOADED`, `CHAT_MSG_GUILD`, and `GUILD_ROSTER_UPDATE`, writes into `GuildChatAIDB` and prints captured messages; `/gcai` forwards user-provided text to guild chat. `GuildChatAI.toc` declares interface 11200.

## Verification boundary

This description comes from reading source and metadata; it does not establish successful operation in a live game client.
