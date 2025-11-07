# How Claude Code Accesses Its Own Docs (And What You Can Learn From It)

I was building a custom skill for Claude Code when I noticed something interesting. Whenever I asked Claude Code about its own features or capabilities, it would use the `WebFetch` tool to grab documentation from this URL:

```
https://code.claude.com/docs/en/claude_code_docs_map.md
```

This markdown file works as an index that contains links to other parts of the documentation. Claude can then follow the links to find the documentation relevant to your query.

This caught my attention because it goes against the grain of what you typically read about embedding documentation into AI agents. It seems that RAG is still the approach most often mentioned for this use case. But it requires you to maintain a vector database, tune chunking strategies, manage embedding models and optimize retrieval quality.

If you can get rid of this complexity, why wouldn't you? I'm sure there are valid technical reasons to go with RAG but I think biggest reason is that most existing docs are built for humans and stored in a format in which they are directly ingestable into a vector database. You don't need to reinvent your documentation system, you can just bolt AI on top of that.

It's a similar dilemma in many other areas. The world around us is not built for the new technologies we have today so we try to bend existing solutions with AI instead of reinventing them more profoundly.

Claude Code is reinventing how we code—and if you're using it daily, pay attention to these patterns. The best way to learn the future of development might just be to observe the tools that are building it.

Some practical tips to learn how claude code works internally:

- Ctrl + o to see the thinking process
- Run `cat ~/.claude/settings.json` or `.claude/settings.local.json` to see your Claude Code configuration and enabled features
- less `~/.claude/debug/latest` for inspecting the debug logs

If you want to take it a step further, you can set up a proxy to log all API calls and see what's happening: https://medium.com/@outsightai/peeking-under-the-hood-of-claude-code-70f5a94a9a62
