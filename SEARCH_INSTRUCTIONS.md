# Prompt Library Search Instructions

## 🎯 PRIMARY GOAL (For AI Models)
When this file is referenced, your task is to:
1. Extract the user's specific need/request
2. Search ALL .md prompt files in this entire repository (recursively across all folders)
3. Find the BEST matching prompt template based on relevance to their request
4. **DO NOT CREATE NEW FILES** - generate the customized prompt as output only
5. Blend/merge the template WITH the user's specific request to create a NEW customized prompt
6. Return: (a) source file path with 1-line justification, (b) customized prompt with [PLACEHOLDER: ...] markers

## How to Use This File
When you reference this file in a request, ANY AI model will:
1. Search through ALL .md files in the entire repository (all folders at any level)
2. Identify the best matching prompt template
3. Generate a new, customized prompt merging the template with your request (as text output only)
4. Include source file reference with justification
5. Fill in any uncertain areas with `[PLACEHOLDER: description]` markers

## Request Format

When you want to trigger this behavior, simply use:

```
do: "[YOUR_SPECIFIC_REQUEST]" use: SEARCH_INSTRUCTIONS.md
```

**Examples:**
```
do: "writing engaging social media captions for a fashion brand" use: SEARCH_INSTRUCTIONS.md
```

```
do: "creating a debugging strategy for production errors" use: SEARCH_INSTRUCTIONS.md
```

## Step-by-Step Algorithm (For AI Models)

When this file is referenced, execute this process:

1. **Parse Request** - Extract the user's specific need from their message
2. **List Prompts** - Search for and read ALL `.md` files anywhere in this repository (recursively through all folders and subfolders)
3. **Match** - Find the BEST matching prompt by semantic relevance to the user's request
4. **Justify** - Prepare a 1-line explanation for why this template was selected
5. **Blend** - Merge the template prompt with the user's specific request to create a customized version
6. **Identify Gaps** - Mark any uncertain/missing details with `[PLACEHOLDER: description]` format
7. **Output Only** - Do NOT create/save files. Output the customized prompt to chat only.
8. **Return** - Show: source file + justification + customized prompt

## What You'll Receive

The AI will respond with:

1. **Source Template with Justification** - The file path and WHY it was selected in 1 line
   - Example: `📁 copywriting/email-marketing.md — Selected because it provides structure for multi-part campaigns with clear value prop emphasis`
2. **Customized Prompt** - A NEW prompt that:
   - Blends the template with your specific use case
   - Is directly tailored to your exact need
   - Includes `[PLACEHOLDER: ...]` markers for unresolved questions
3. **Ready to Use** - Copy the customized prompt and fill in placeholders with your details

## Important: No File Creation
- The AI will search and read existing prompt templates
- The AI will NOT create new files in the repository
- The customized prompt is generated and shown in chat only
- You can save it manually if needed

## Tips for Better Results

- **Be specific** - The more details you provide, the better the customization
- **Describe the outcome** - What do you want as a result?
- **Mention constraints** - Any tone, length, or style preferences?

## Repository Structure

The library contains prompt templates organized in folders. The AI will search through all of them automatically:
- Folder structure can evolve
- AI will find all .md files regardless of folder location
- Add new folders and templates as needed
