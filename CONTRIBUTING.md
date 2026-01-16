# Contributing to Ethereum Knowledge Base

Thank you for contributing to this knowledge base! This guide will help you add new articles effectively.

## Quick Start for LLMs

If you're an LLM agent creating a PR to add a new article:

1. **Create the Article File**
   - Place it in the appropriate category folder under `articles/`
   - Use lowercase with hyphens for the filename (e.g., `eip-4844-proto-danksharding.md`)
   - Follow the template structure from `templates/article-template.md`

2. **Fill in Metadata**
   - Title: Full article title
   - Description: 1-2 sentence summary
   - Link: URL to original content
   - Date Added: Current date (YYYY-MM-DD)
   - Date Published: When the article was published
   - Tags: 3-5 relevant tags in backticks

3. **Update INDEX.md**
   - Add an entry under the appropriate category section
   - Include the article title (linked), description, tags, and date
   - Increment the "Total Articles" count
   - Update the "Last Updated" date

4. **Content Guidelines**
   - Write a clear summary (2-4 paragraphs)
   - Extract and explain key concepts
   - Include notable quotes with proper formatting
   - Add personal insights or questions
   - Link to related articles in the knowledge base
   - List all references

## Categories

Choose the most appropriate category for your article:

- **consensus/**: Consensus mechanisms, validators, staking, proof-of-stake
- **execution/**: EVM, transactions, smart contracts, opcodes
- **scaling/**: Layer 2, rollups, sharding, state channels
- **protocol/**: EIPs, hard forks, protocol upgrades, governance
- **economics/**: MEV, gas economics, tokenomics, incentive structures
- **security/**: Security audits, vulnerabilities, best practices, attack vectors
- **tools/**: Development tools, wallets, infrastructure, testing frameworks
- **general/**: Overviews, introductions, multi-topic articles

If an article fits multiple categories, choose the primary focus.

## Article Template

```markdown
# [Article Title]

## Metadata

- **Title**: [Full title]
- **Description**: [Brief description]
- **Link**: [URL]
- **Date Added**: [YYYY-MM-DD]
- **Date Published**: [YYYY-MM-DD or "Unknown"]
- **Tags**: `tag1`, `tag2`, `tag3`

---

## Summary

[2-4 paragraphs summarizing the main points]

## Key Concepts

- **Concept 1**: [Explanation]
- **Concept 2**: [Explanation]

## Important Quotes or Highlights

> [Quote from the article]

## Personal Notes

[Insights, questions, or connections to other concepts]

## Related Articles

- [Links to related articles in this KB]

## References

- [Original article link]
- [Additional references]
```

## Tag Guidelines

Use consistent, descriptive tags:

### Consensus & Validation
- `consensus`, `pos`, `pow`, `validators`, `staking`, `beacon-chain`, `merge`

### Execution & Smart Contracts  
- `evm`, `smart-contracts`, `solidity`, `vyper`, `opcodes`, `transactions`

### Scaling
- `layer2`, `rollup`, `optimistic-rollup`, `zk-rollup`, `sharding`, `state-channel`

### Protocol
- `eip`, `protocol-upgrade`, `hard-fork`, `governance`, `ethereum-roadmap`

### Economics
- `mev`, `gas`, `tokenomics`, `incentives`, `issuance`, `eip-1559`

### Security
- `security`, `audit`, `vulnerability`, `attack`, `best-practices`

### Tools & Development
- `devtools`, `wallet`, `infrastructure`, `testing`, `client`

### General
- `beginner`, `overview`, `whitepaper`, `research`, `history`

## Style Guide

### Writing Style
- Use clear, concise language
- Explain technical terms when first introduced
- Maintain an objective, informative tone
- Focus on accuracy and completeness

### Formatting
- Use headers (`##`, `###`) for organization
- Use bullet points for lists
- Use bold for emphasis on key terms
- Use code blocks for technical examples
- Use block quotes (`>`) for article excerpts

### Linking
- Always link to the original source
- Link to related articles within the knowledge base
- Use descriptive link text, not "click here"

## INDEX.md Entry Format

When adding your article to INDEX.md, use this format:

```markdown
### [Article Title](articles/category/filename.md)
- **Description**: Brief one-sentence description
- **Tags**: `tag1`, `tag2`, `tag3`
- **Date**: YYYY-MM-DD
```

Place it in the appropriate category section, maintaining chronological or alphabetical order.

## Pull Request Guidelines

### PR Title
Use a clear, descriptive title:
- ✅ "Add article: EIP-4844 Proto-Danksharding"
- ✅ "Add consensus article on proposer-builder separation"
- ❌ "New article"
- ❌ "Update"

### PR Description
Include:
1. Brief summary of the article topic
2. Why this article is valuable for the knowledge base
3. Category where it's placed
4. Any notable highlights or key insights

### Example PR Description
```
Adding an article about EIP-4844 (Proto-Danksharding) to the scaling category.

This article explains how blob transactions work and their impact on Layer 2 
rollup costs. It's an important piece of Ethereum's scaling roadmap and 
complements our existing articles on rollups and data availability.

Key insights:
- Blob transactions reduce L2 costs by 10-100x
- Temporary data storage (blob TTL)
- Foundation for full danksharding

Category: scaling/
```

## Checklist for New Articles

Before submitting your PR, ensure:

- [ ] Article follows the template structure
- [ ] All metadata fields are filled in
- [ ] Filename uses lowercase with hyphens
- [ ] File is in the correct category directory
- [ ] Tags are consistent with existing tags
- [ ] Summary is clear and informative
- [ ] KEY concepts are explained
- [ ] Original source is linked
- [ ] INDEX.md is updated with a new entry
- [ ] Total article count is incremented
- [ ] Last Updated date is current
- [ ] PR title and description are clear

## Questions?

If you're unsure about:
- Which category to use → Choose the primary focus
- How many tags to add → 3-5 is ideal
- Summary length → 2-4 paragraphs covers most articles
- Whether to include something → When in doubt, include it

## LLM-Specific Notes

If you're an AI assistant adding articles:

1. **Be thorough**: Don't skip sections of the template
2. **Extract value**: Include key concepts and insights, not just metadata
3. **Maintain consistency**: Follow existing patterns in INDEX.md and tag usage
4. **Verify links**: Ensure all URLs are correct and accessible
5. **Use proper dates**: YYYY-MM-DD format
6. **Update counts**: Don't forget to increment total articles and update date

The goal is to create a high-quality, searchable knowledge base that both humans and LLMs can effectively use for learning and reference.
