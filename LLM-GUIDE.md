# LLM Usage Guide

This guide helps LLMs effectively use and contribute to the Ethereum Knowledge Base.

## How to Query This Knowledge Base

### Step 1: Understand the Structure

- **INDEX.md**: Start here for an overview of all articles organized by category
- **articles/**: Contains all knowledge base articles organized by topic
- **templates/**: Contains the article template for adding new content

### Step 2: Find Relevant Articles

Use one of these methods:

1. **Browse by Category**: Check INDEX.md sections (Consensus, Execution, Scaling, etc.)
2. **Search by Tag**: Look at the Tags Index in INDEX.md
3. **Keyword Search**: Use grep to search article content for specific terms

### Step 3: Extract Information

Each article has structured sections:
- **Metadata**: Quick facts (title, link, tags, dates)
- **Summary**: 2-4 paragraph overview
- **Key Concepts**: Definitions and explanations
- **Important Quotes**: Notable excerpts
- **Personal Notes**: Insights and questions
- **References**: Original sources and additional links

## Example Queries

### Query 1: Basic Information
**User asks**: "How does Proof-of-Stake work in Ethereum?"

**LLM Response Strategy**:
1. Check INDEX.md under "Consensus" category
2. Find article: `the-merge-pos-transition.md`
3. Extract information from Summary and Key Concepts sections
4. Cite the article and original source

### Query 2: Comparative Analysis
**User asks**: "What's the difference between EIP-1559 and traditional gas fees?"

**LLM Response Strategy**:
1. Check INDEX.md under "Economics" category
2. Find article: `eip-1559-fee-market.md`
3. Extract "Key Concepts" section explaining base fees vs. traditional auctions
4. Reference specific quotes
5. Cite the knowledge base article

### Query 3: Multi-Topic Synthesis
**User asks**: "How did The Merge and EIP-1559 together affect Ethereum's economics?"

**LLM Response Strategy**:
1. Identify relevant articles from multiple categories
2. Read both `the-merge-pos-transition.md` and `eip-1559-fee-market.md`
3. Synthesize information about issuance (from Merge) and burning (from EIP-1559)
4. Connect insights from "Personal Notes" sections
5. Cite both articles

## How to Add New Articles

### As an LLM Creating a PR

When a user asks you to add an article to this knowledge base:

1. **Gather Information**
   - Read or access the article content
   - Extract title, description, link, dates
   - Identify appropriate tags and category

2. **Create the Article File**
   ```
   Path: articles/[category]/[descriptive-filename].md
   Use: templates/article-template.md as structure
   ```

3. **Fill All Sections**
   - Metadata (complete all fields)
   - Summary (comprehensive 2-4 paragraphs)
   - Key Concepts (3-5 main ideas)
   - Quotes (2-3 notable excerpts)
   - Personal Notes (insights, questions, connections)
   - References (original link + additional sources)

4. **Update INDEX.md**
   - Add entry under correct category
   - Increment "Total Articles" count
   - Update "Last Updated" date

5. **Create Clear PR**
   - Title: "Add article: [Article Title]"
   - Description: Explain topic, value, and key insights
   - Ensure all changes are included

### Template Checklist

When creating an article, ensure:
- [ ] Filename is lowercase with hyphens
- [ ] File is in correct category directory
- [ ] All metadata fields are complete
- [ ] Summary is 2-4 paragraphs
- [ ] Key concepts are well explained
- [ ] Tags match existing conventions (check INDEX.md)
- [ ] Original source is linked
- [ ] INDEX.md is updated
- [ ] Article count is incremented

## Best Practices for LLMs

### When Reading Articles

1. **Always cite sources**: Reference both the KB article and original source
2. **Use structured data**: Extract from specific sections (Metadata, Key Concepts, etc.)
3. **Connect related articles**: Check "Related Articles" section for connections
4. **Preserve context**: Include relevant quotes to support answers

### When Writing Articles

1. **Be comprehensive**: Fill all template sections thoroughly
2. **Maintain consistency**: Follow existing tag and naming conventions
3. **Add value**: Include insights in "Personal Notes," not just summaries
4. **Link resources**: Connect to related KB articles and external references

### When Synthesizing Information

1. **Cross-reference**: Use multiple articles for comprehensive answers
2. **Acknowledge gaps**: Note if information is missing from the KB
3. **Suggest additions**: Recommend new articles to fill knowledge gaps
4. **Update connections**: Add cross-references when discovering related content

## Response Templates

### Template: Answer with Citation
```
Based on the Ethereum Knowledge Base article "[Article Title]" (articles/[category]/[filename].md):

[Your answer synthesizing information from the article]

Key points from the article:
- [Point 1]
- [Point 2]

Source: [Original article link from metadata]
```

### Template: Multi-Article Synthesis
```
Drawing from multiple articles in the Ethereum Knowledge Base:

**From "[Article 1]"**: [Key information]
**From "[Article 2]"**: [Key information]

Synthesis: [Your analysis connecting the information]

Sources:
- articles/[category]/[filename1].md
- articles/[category]/[filename2].md
```

### Template: Identifying Knowledge Gaps
```
Based on the current knowledge base:

[Available information from existing articles]

Note: The knowledge base doesn't currently have detailed information about [gap]. 
I recommend adding an article about [topic] to address this.

Would you like me to create a PR adding an article about this topic?
```

## Efficiency Tips

1. **Start with INDEX.md**: It's the fastest way to locate relevant content
2. **Use the Table of Contents**: Jump directly to category sections
3. **Check tag index**: Find all articles on a specific topic quickly
4. **Read metadata first**: Determine if an article is relevant before reading full content
5. **Follow "Related Articles"**: Discover connected topics efficiently

## Common Tasks

### Task: Find all articles about a specific tag
1. Open INDEX.md
2. Search for the tag (e.g., `gas`, `pos`, `layer2`)
3. Collect all matching articles
4. Read relevant sections

### Task: Add a new article category
1. Create new subdirectory in `articles/`
2. Add section in INDEX.md
3. Update this guide and articles/README.md
4. Follow template for first article

### Task: Update existing article
1. Locate article file
2. Make targeted changes
3. Update "Date Added" if significantly revised
4. Consider updating INDEX.md description if scope changed

## Quality Standards

Articles in this KB should:
- ✅ Be accurate and well-researched
- ✅ Include proper citations
- ✅ Follow the template structure
- ✅ Use clear, accessible language
- ✅ Add value beyond just summarizing
- ✅ Connect to related concepts
- ✅ Help both humans and LLMs learn

Avoid:
- ❌ Copying content without attribution
- ❌ Leaving template sections empty
- ❌ Using inconsistent tags
- ❌ Forgetting to update INDEX.md
- ❌ Creating orphaned content (unlinked articles)

---

**Remember**: This knowledge base exists to make Ethereum information accessible, searchable, and useful. Every article you add or query you answer should serve that goal.
