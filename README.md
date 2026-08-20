AOE-SEO-V2

A nine-step SEO/AEO article production chain for Super Dispatch content.

This repository contains the skills that move an article from initial keyword strategy through research, drafting, verification, WordPress-ready markup, and final visual prompts. Each skill is designed to hand its output to the next step in the chain.

Workflow

Step

Skill

Purpose

Primary output

1

sd-seo-keyword-brief-article-writer-part-1.skill

Analyze the target keyword, search intent, funnel stage, related entities, research questions, and E-E-A-T needs.

Structured Research Brief JSON

2

sd-seo-research-pack-article-writer-part-2.skill

Research the brief, gather trustworthy sources, statistics, competitive context, and SERP insights.

Structured Research Pack JSON

3

sd-seo-outline-article-writer-part-3.skill

Turn the research pack into a draft-ready article structure based on the content mode and search intent.

Structured Outline JSON

4

sd-seo-draft-article-writer-part-4.skill

Write the full SEO-optimized article using the outline and research pack.

Markdown draft + metadata JSON

5

sd-seo-aeo-takeaways-article-writer-part-5.skill

Extract and inject a data-dense ### Key Takeaways section for answer-engine visibility.

Draft with Key Takeaways block

6

sd-seo-verification-article-writer-part-6.skill

Grade SEO/keyword execution, fact-check claims, and verify that takeaway figures match the article body.

Verification report + pass/fail gate

7

sd-seo-post-process-article-writer-part-7.skill

Enrich the verified draft with internal links, video embeds, supplemental schema, and CTA instructions.

Enriched markdown + structured report + schema blocks

8

sd-seo-divi-markup-article-writer-part-8.skill

Convert the post-processed article into WordPress-ready HTML.

Self-contained CMS-ready HTML fragment

9

sd-seo-article-visual-prompts-part-9.skill

Create prompts and guidance for article visuals, featured images, alt text, filenames, and placement.

Structured visual-prompt JSON

Chain

Keyword / Topic
    ↓
1. Keyword Brief
    ↓
2. Research Pack
    ↓
3. Article Outline
    ↓
4. Article Draft
    ↓
5. AEO Key Takeaways
    ↓
6. Verification Gate
    ↓
7. Post-Processing
    ↓
8. WordPress Markup
    ↓
9. Visual Prompts
    ↓
Publish-ready article package

How to use

Run the skills in order from Step 1 through Step 9. Downstream steps depend on the structured output and context produced upstream.

The verification step is a quality gate rather than an enrichment step. If verification finds a blocking issue, return the work to the appropriate upstream step, correct it, and re-run the affected downstream steps before continuing.

Repository structure

AOE-SEO-V2/
├── README.md
├── sd-seo-keyword-brief-article-writer-part-1.skill
├── sd-seo-research-pack-article-writer-part-2.skill
├── sd-seo-outline-article-writer-part-3.skill
├── sd-seo-draft-article-writer-part-4.skill
├── sd-seo-aeo-takeaways-article-writer-part-5.skill
├── sd-seo-verification-article-writer-part-6.skill
├── sd-seo-post-process-article-writer-part-7.skill
├── sd-seo-divi-markup-article-writer-part-8.skill
└── sd-seo-article-visual-prompts-part-9.skill

Notes

Keep the numbered sequence intact. The filenames make the execution order explicit.

Step 2 includes the Super Moves benchmark reference inside its skill bundle.

Step 7 may rely on live internal resources for enrichment such as internal-link catalog data.

Step 8 prepares the article body for WordPress; supplemental schema generated in Step 7 is handled separately.

Step 9 generates visual instructions and prompts rather than generating the images itself.

Goal

The goal of this chain is a repeatable article-production workflow that combines SEO strategy, answer-engine optimization, evidence-backed writing, quality control, CMS preparation, and visual planning in one consistent nine-step process.
