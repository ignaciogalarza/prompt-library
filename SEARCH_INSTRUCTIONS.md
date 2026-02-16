# Prompt Library Search Instructions

## Purpose
This file contains instructions for searching and retrieving prompts from the library in an intelligent way. When referenced in a chat request, it guides the AI to find the most relevant prompt template and blend it with your specific use case.

## How It Works
When you need a prompt, you'll provide:
1. **Your specific need/use case** - What you want to accomplish
2. **Reference to this file** - Link to SEARCH_INSTRUCTIONS.md

The AI will then:
1. Search through all prompt files in the repository
2. Identify the best matching prompt template(s)
3. Create a new, customized prompt that merges the template with your request
4. Fill in any uncertain areas with `[PLACEHOLDER: description]` markers

## Request Format

Use this format when searching:

```
I'm looking for a prompt to help with: [YOUR_SPECIFIC_NEED]

Ref: SEARCH_INSTRUCTIONS.md
```

**Example:**
```
I'm looking for a prompt to help with: writing engaging social media captions for a fashion brand

Ref: SEARCH_INSTRUCTIONS.md
```

## What You'll Receive

The AI will respond with:

1. **Source Template** - The original prompt file found in the library
2. **Customized Prompt** - A new prompt that:
   - Blends the template with your specific use case
   - Is tailored to your exact need
   - Includes placeholder markers for details you need to fill in
3. **Placeholders** - `[PLACEHOLDER: description]` tags for any unresolved questions or customizations needed

**Example Response:**
```
📁 Source: copywriting/social-media.md

## Your Custom Prompt:
Write an engaging Instagram caption for [PLACEHOLDER: product type] that...
- Targets [PLACEHOLDER: target audience]
- Emphasizes [PLACEHOLDER: key benefit]
- Includes a call-to-action for [PLACEHOLDER: desired action]
```

## Tips for Better Results

- **Be specific** - The more details you provide, the better the customization
- **Describe the outcome** - What do you want as a result?
- **Mention constraints** - Any tone, length, or style preferences?

## Folder Structure

Prompts are organized by category:
- `copywriting/` - Marketing, social media, email, product descriptions
- `coding/` - Code generation, debugging, architecture
- `analysis/` - Data analysis, research, summaries
- `creative/` - Writing, brainstorming, ideation
- `other/` - Miscellaneous prompts

Explore the folders to understand what templates are available!
