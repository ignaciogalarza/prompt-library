# Prompt Library

A personal collection of reusable prompt templates. Search and retrieve them intelligently through chat to find the perfect prompt for your specific use case.

## 🔍 How to Search for Prompts

Use this simple format in chat:

```
do: "[YOUR_SPECIFIC_REQUEST]" use: SEARCH_INSTRUCTIONS.md
```

**Example:**
```
do: "I need help writing a product description for an e-commerce site" use: SEARCH_INSTRUCTIONS.md
```

I will:
1. Search all prompt templates in this repository
2. Find the best matching template
3. Customize it with your specific request
4. Return the source file + justification + customized prompt

See [SEARCH_INSTRUCTIONS.md](SEARCH_INSTRUCTIONS.md) for complete details.

## 📋 What You'll Get

Each search result includes:
- **Source template** - Which prompt file was used
- **Why selected** - 1-line explanation of relevance
- **Customized prompt** - Your new prompt with `[PLACEHOLDER: ...]` markers
- **Ready to use** - Fill in placeholders and go

## 📁 Adding Prompts

Add your own prompt templates as `.md` files anywhere in this repository. Organize them however you like—the search will find all of them automatically.

**Example structure:**
```
prompt-library/
├── copywriting/
│   ├── email.md
│   └── social-media.md
├── coding/
│   └── debugging.md
└── analysis/
    └── research.md
```
