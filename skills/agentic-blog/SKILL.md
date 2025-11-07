---
name: agentic-blog
description: Writes engaging blog posts about agentic coding experiments, AI-assisted development workflows, and Claude Code usage. Use when the user wants to document their coding experiments, share learnings about AI agents, or create technical blog content about agentic development practices.
---

# Agentic Coding Blog Post Writer

This skill helps you write compelling blog posts about your experiments with agentic coding, AI-assisted development, and Claude Code workflows.

## Instructions

When activated, follow these steps to create a blog post that matches the user's style:

**Core Principle**: Less is more. Write short, insightful posts (200-400 words) that focus on one interesting observation and its philosophical implications. Avoid comprehensive tutorials or detailed how-tos.

### 1. Gather Context

- Ask the user about the experiment or discovery they want to write about
- Focus on finding the ONE interesting insight worth sharing

### 2. Writing Style - Keep It Simple and Focused

**IMPORTANT**: Aim for brevity and clarity. A good blog post should be 200-400 words, not thousands.

Your writing style:

- **Short and direct**: Get to the point quickly without preamble or TL;DR
- **Narrative flow**: Write as a flowing story, not as structured sections
- **Personal and conversational**: Write in first person, share your observations naturally
- **Focus on the insight**: Find the ONE interesting thing and explore it philosophically
- **Thought-provoking endings**: End with a statement that makes readers think, not a bullet list of takeaways
- **Minimal structure**: Use few headers, let the narrative flow
- **Less listy**: Avoid excessive bullet points - use them only when listing technical requirements

### 3. Structure - Less Is More

Instead of multiple sections, use a simple flow:

1. **Start with the discovery**: "I noticed something interesting..."
2. **Explain what you found**: Keep it simple and direct

Avoid:

- TL;DR sections
- Extensive "how it works" explanations
- "Practical Tips" sections
- Long bullet lists
- Traditional "conclusion" sections

### 4. Code and Examples

- Only include code if essential to the point
- Keep examples minimal - show just enough to illustrate
- Focus on the concept, not the implementation details

### 5. Tone and Language

- Write like you're explaining to a colleague over coffee
- No marketing speak or excessive enthusiasm
- No superlatives unless genuine
- Simple, clear language
- Question conventional wisdom when appropriate

### 6. Create a Social Media Summary

After writing the main blog post, create a short summary under a `## Share` heading:

- 2-3 short paragraphs (150-200 words max)
- Start with the core insight
- Keep the philosophical angle
- Use simple bullet points for key points (2-3 bullets max)
- End with an engaging question
- Include `[Read more]` placeholder
- Add relevant hashtags for LinkedIn

Keep the same conversational tone as the main post. Make it feel like a natural excerpt, not a marketing summary.

### 7. Save the Blog Post

**IMPORTANT**: Always save blog posts as markdown files (.md) in the directory:
`/Users/tarmo.terimaa/code/agentic-coding-experiments`

- Generate a descriptive filename based on the blog post title (e.g., `my-experiment-with-ai-agents.md`)
- Use lowercase letters and hyphens for the filename
- Ensure the directory exists before writing the file
- Include the social media summary at the end of the file under `## Share`

## Example Prompts That Trigger This Skill

- "Write a blog post about my experience using Claude Code for refactoring"
- "Help me document my experiment with AI agents"
- "Create a blog post about how I automated my workflow with agentic coding"
- "I want to share my learnings from building with Claude Code"

## Output Format

The skill will produce a complete, ready-to-publish blog post in markdown format, saved to `/Users/tarmo.terimaa/code/agentic-coding-experiments/[descriptive-filename].md`.
