# Progress-Slides

Progress-Slides is a specialized Gemini "Skill" designed to transform structured work progress data into a minimal, modern, and professional HTML presentation. Instead of complex slide software, it leverages strict AI output control to generate a single, self-contained file optimized for quick sharing and clean aesthetics.

## Purpose

The primary goal of Progress-Slides is to provide a stable, predictable way to visualize work status. By focusing on layout constraints and minimalist design, it ensures that the focus remains on the content while maintaining a premium "look and feel" without manual formatting.

## File Structure

- **`README.md`**: Provides an overview of the skill, usage instructions, and design philosophy.
- **`SKILL.md`**: The core "Skill" definition. Contains the conversational workflow, 6 visual styles, and layout constraints.
- **`input.yaml`**: A template for structured input data, now including `selected_style`.
- **`output.html`**: A reference of the expected generation result.

## Usage Instructions

To generate a progress deck, follow these steps:

1. **Initialize the Skill**: Copy and paste the entire content of `SKILL.md` into your conversation with Gemini.
2. **Conversational Flow**: 
    - Gemini will check your content.
    - Gemini will present **6 style options** (Minimalist, Dark Signal, Swiss Modern, Botanical, Cyber Terminal, Editorial).
    - Reply with your preferred style name.
3. **Provide Your Data**: Send your work progress data following the structure shown in `input.yaml`.
4. **Generate**: The AI will output the self-contained HTML.
5. **Save and View**: Copy the code into an `.html` file and open it in a browser.

## Visual Styles

Progress-Slides now supports 6 distinct aesthetics:
- **Minimalist**: Clean, white background, system-ui (Standard).
- **Dark Signal**: Indigo/Neon, tech-focused.
- **Swiss Modern**: Bold grids, high-contrast red/white.
- **Botanical**: Soft greens, elegant serif typography.
- **Cyber Terminal**: CRT aesthetics, luminous green text.
- **Editorial**: Magazine style, premium layout and tracking.

## Live Examples

You can preview the 6 visual styles by opening the following HTML files in your browser:

| Style | Preview Link | Description |
| :--- | :--- | :--- |
| **Minimalist** | [minimalist.html](file:///Users/akousist_xml7h/progress-deck/examples/minimalist.html) | Clean, airy, white background. |
| **Dark Signal** | [dark_signal.html](file:///Users/akousist_xml7h/progress-deck/examples/dark_signal.html) | Tech-focused, deep indigo, neon accents. |
| **Swiss Modern** | [swiss_modern.html](file:///Users/akousist_xml7h/progress-deck/examples/swiss_modern.html) | Bold grids, high-contrast red & black. |
| **Botanical** | [botanical.html](file:///Users/akousist_xml7h/progress-deck/examples/botanical.html) | Organic, soft green, elegant serifs. |
| **Cyber Terminal** | [cyber_terminal.html](file:///Users/akousist_xml7h/progress-deck/examples/cyber_terminal.html) | Retro-hacker look, CRT scanlines. |
| **Editorial** | [editorial.html](file:///Users/akousist_xml7h/progress-deck/examples/editorial.html) | High-end magazine, premium typography. |

## How to Use with Other AIs

When you host this project on GitHub or share it with others, here is how different AI interfaces can consume the **Progress-Slides Skill**:

### 1. Direct Chat (Gemini, Claude, ChatGPT)
The simplest way to "install" the skill is to copy the entire content of [SKILL.md](file:///Users/akousist_xml7h/progress-deck/SKILL.md) and paste it into a new chat session.
- **Tip**: Start the message with "You are now following these Skill instructions:" followed by the file content.

### 2. Custom Instructions / System Prompts
If you want the AI to *always* know how to generate these decks:
- Go to the AI's settings (e.g., "Custom Instructions" in ChatGPT or "System Prompt" in Gemini).
- Paste the content of `SKILL.md` there.

### 3. Agentic Tools (Claude Code, Cursor, Windsurf)
If you are using developer-focused AI tools:
- Simply keep `SKILL.md` in your project root.
- Mention `@SKILL.md` or tell the tool to "Follow the logic in SKILL.md to generate a progress report."

### 4. Shared URL
Since the project is on GitHub, you can provide the **Raw URL** of `SKILL.md` to any tool that supports web fetching or browsing.

---

## Design Philosophy

Progress-Slides adheres to a "Less is More" aesthetic:
- **High Contrast**: Pure white background with deep black text for maximum readability.
- **Typography-First**: Uses system-native fonts with generous sizing and whitespace.
- **Standardized Rhythm**: Each section is capped at one full viewport height (`100vh`), creating a focused, slide-like experience.
- **Zero Bloat**: No external CSS frameworks, no JavaScript, and no tracking scripts. Just clean, semantic HTML.

## Verification Checklist

To ensure the generation is stable and follows the Skill requirements, verify the following:
- [ ] The output is a single `<html>` block with no conversational filler.
- [ ] The slides use `<section>` tags for each slide.
- [ ] The font-family is set to `system-ui`.
- [ ] No external URLs or CDNs are referenced in the `<head>`.
- [ ] Each slide is vertically and horizontally centered.

## Key Concept: Output Control

This Skill is not about the complexity of the HTML/CSS itself; it is about **prompt engineering for predictable output**. It demonstrates how to use the LLM as a structured renderer, converting "thought" (YAML data) into "presentation" (HTML) through a series of strict structural and stylistic boundaries.