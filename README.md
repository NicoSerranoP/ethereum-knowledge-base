# ethereum-knowledge-base

A knowledge base of all Ethereum related info I read. This repo will be used with LLMs to keep track of all information I read.

## 📚 Overview

This repository serves as a structured knowledge base for Ethereum-related articles, papers, and resources. Each article is stored as a markdown file with comprehensive metadata, making it easy for both humans and LLMs to search, understand, and reference the content.

## 🗂️ Structure

```
ethereum-knowledge-base/
├── INDEX.md                    # Central catalog of all articles
├── README.md                   # This file
├── templates/
│   └── article-template.md    # Template for new articles
└── articles/
    ├── README.md              # Articles directory guide
    ├── consensus/             # Consensus mechanisms, validators
    ├── execution/             # EVM, transactions, smart contracts
    ├── scaling/               # Layer 2, rollups, sharding
    ├── protocol/              # EIPs, protocol upgrades
    ├── economics/             # Tokenomics, MEV, gas
    ├── security/              # Audits, vulnerabilities
    ├── tools/                 # Development tools, infrastructure
    └── general/               # General information
```

## ✨ Features

- **Structured Metadata**: Each article includes title, description, link, date, and tags
- **LLM-Friendly**: Formatted for easy parsing and understanding by AI systems
- **Searchable**: Organized by categories with a comprehensive tag system
- **Cross-Referenced**: Articles link to related content within the knowledge base
- **Easy to Extend**: Simple template-based system for adding new content

## 🚀 How to Add a New Article

### Manual Method

1. Choose the appropriate category directory in `articles/`
2. Create a new `.md` file with a descriptive name (use lowercase and hyphens)
3. Copy the template from `templates/article-template.md`
4. Fill in all sections:
   - Metadata (title, description, link, dates, tags)
   - Summary of the article
   - Key concepts explained
   - Important quotes or highlights
   - Your personal notes and insights
   - Related articles and references
5. Update `INDEX.md` with an entry for your new article
6. Submit a Pull Request

### Using LLMs (Recommended)

You can ask an LLM (like Codex, ChatGPT, or Claude) to create a PR with a new article. Provide the LLM with:

1. Link to the article you read
2. Category it belongs to
3. Any specific notes or highlights you want to include

**Example prompt:**
```
Add the article from [URL] to the ethereum-knowledge-base repository. 
It's about [topic] and should go in the [category] folder.
Include these key points: [your notes]
```

The LLM will:
- Create a properly formatted markdown file
- Fill in all metadata
- Add it to the correct category
- Update the INDEX.md
- Submit a PR

## 📋 Article Template

Each article follows this structure:

- **Metadata Section**: Title, description, link, dates, tags
- **Summary**: 2-4 paragraph overview of main points
- **Key Concepts**: Definitions and explanations of important terms
- **Important Quotes**: Notable excerpts from the article
- **Personal Notes**: Your thoughts, questions, and insights
- **Related Articles**: Links to other articles in the knowledge base
- **References**: Original source and additional resources

## 🏷️ Tagging System

Use tags to make articles easily discoverable. Common tags include:

- `consensus`, `pos`, `pow`, `validators`
- `evm`, `smart-contracts`, `solidity`
- `layer2`, `rollup`, `optimistic`, `zk`
- `eip`, `protocol-upgrade`
- `gas`, `mev`, `tokenomics`
- `security`, `audit`
- `devtools`, `infrastructure`

## 📖 Using the Knowledge Base

### For Humans

- Browse the [INDEX.md](INDEX.md) to see all articles organized by category
- Search for specific tags or topics
- Follow the "Related Articles" links to explore connected topics

### For LLMs

When querying this knowledge base with an LLM:

1. Reference the INDEX.md for an overview of available content
2. Point to specific article files for detailed information
3. Use the metadata and tags to find relevant articles
4. Leverage the structured format for accurate information extraction

**Example LLM query:**
```
Based on the ethereum-knowledge-base repository, explain how Proof-of-Stake 
works in Ethereum, using the articles about consensus mechanisms.
```

## 🤝 Contributing

Contributions are welcome! Whether you're adding new articles, improving existing ones, or enhancing the structure:

1. Fork the repository
2. Create a feature branch
3. Make your changes following the template and style guide
4. Update INDEX.md if adding new articles
5. Submit a Pull Request

## 📝 License

This knowledge base is for personal use and learning. All referenced articles and sources retain their original copyrights.

## 🎯 Goals

- Build a comprehensive personal knowledge base about Ethereum
- Make it easy to recall and reference information
- Enable LLMs to provide accurate, sourced answers about Ethereum
- Track learning progress and understanding over time
- Connect related concepts across different articles
