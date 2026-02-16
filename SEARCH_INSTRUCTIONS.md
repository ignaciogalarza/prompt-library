# Prompt Library Search Instructions

## 🎯 PRIMARY GOAL (For AI Models)
When this file is referenced, your task is to:
1. Extract the user's specific need/request
2. Read ALL prompt .md files from this repository's folders (copywriting/, coding/, analysis/, creative/, other/)
3. Find the BEST matching prompt template based on relevance to their request
4. Blend/merge the template WITH the user's specific request to create a NEW customized prompt
5. Return: (a) source file path, (b) customized prompt with [PLACEHOLDER: ...] markers for unresolved details

## How to Use This File
When you reference this file in a request, ANY AI model will:
1. Search through all prompt files in the repository
2. Identify the best matching prompt template(s)
3. Create a new, customized prompt that merges the template with your request
4. Fill in any uncertain areas with `[PLACEHOLDER: description]` markers

## Request Format

When you want to trigger this behavior, simply use:

```
do: "[YOUR_SPECIFIC_REQUEST]" use: SEARCH_INSTRUCTIONS.md
```

Or more explicitly:
```
I'm looking for a prompt to help with: [YOUR_SPECIFIC_NEED]

Ref: SEARCH_INSTRUCTIONS.md
```

**Examples:**
```
do: "writing engaging social media captions for a fashion brand" use: SEARCH_INSTRUCTIONS.md
```

```
do: "creating a debugging strategy for production errors" use: SEARCH_INSTRUCTIONS.md
```

**The AI will immediately understand:** Search the repository, find the best matching prompt file, customize it with this request, and return both the source and the customized version.

## Step-by-Step Algorithm (For AI Models)

When this file is referenced, execute this process:

1. **Parse Request** - Extract the user's specific need from their message
2. **List Prompts** - Read all `.md` files in: `copywriting/`, `coding/`, `analysis/`, `creative/`, `other/`
3. **Match** - Find the best matching prompt by semantic relevance to the user's request
4. **Blend** - Merge the template prompt with the user's specific request to create a customized version
5. **Identify Gaps** - Mark any uncertain/missing details with `[PLACEHOLDER: description]` format
6. **Return** - Show source file + customized prompt

## What You'll Receive

The AI will respond with:

1. **Source Template** - The path to the original prompt file found (e.g., `copywriting/social-media.md`)
2. **Customized Prompt** - A NEW prompt that:
   - Blends the template with your specific use case
   - Is directly tailored to your exact need
   - Includes `[PLACEHOLDER: ...]` markers for any unresolved questions
3. **Ready to Use** - Copy the customized prompt and fill in the placeholders with your details

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
