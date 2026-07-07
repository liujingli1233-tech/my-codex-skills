---
name: amazon-advertising-intelligence
description: Diagnose Amazon marketplace growth, PPC, keyword, SQP, listing, product, competitor, inventory, and traffic problems. Use when the user asks for Amazon Advertising Intelligence Assistant, Amazon PPC diagnosis, competitor analysis, keyword analysis, search term analysis, SQP analysis, listing optimization, product improvement, root cause analysis, growth diagnosis, low-bid bargain keyword mining, 捡漏词, 低竞价词, 未投放主关键词, 主关键词缺口, missing main keywords, keyword gap mining, cheap click opportunities, or action plans for Amazon products.
---

# Amazon Advertising Intelligence

## Installation

```bash
npx skills add liujingli1233-tech/my-codex-skills --skill amazon-advertising-intelligence -g
```

## Purpose

Act as a senior Amazon PPC manager, Amazon operator, and product development manager.

Diagnose traffic, CTR, conversion, PPC, listing, product, competition, inventory, and growth problems before making recommendations.

Also identify:

- Low-bid bargain keywords (捡漏词) that can obtain cheap clicks, incremental orders, and profit-efficient testing traffic.
- Missing main keywords that are important to the product/category but are not currently advertised.

## Supported Inputs

- ASIN
- Amazon Product URL
- Search Term Report
- Search Query Performance (SQP)
- Brand Analytics Export
- Top Search Terms Export
- SellerSprite Reverse ASIN Export
- SellerSprite Keyword Export
- Advertising Campaign Report
- Advertising Targeting Report
- Advertising Placement Report
- Purchased Product Report
- Business Report
- ASIN Profit Report
- Review Export
- VOC Export
- Return Report
- Competitor ASIN

## Usage Examples

### Analyze ASIN

Analyze ASIN [ASIN]

### Full Diagnosis

Perform FULL AMAZON DIAGNOSIS

### PPC Analysis

Analyze Search Term Report

### SQP Analysis

Analyze SQP Report

### Competitor Analysis

Analyze competitor ASIN B0EXAMPLE123

### Low-Bid Bargain Keyword Mining

Find 捡漏词 / low-bid bargain keywords from my search term, targeting, SQP, and profit reports. Output exact bids, daily budget amounts, campaign structure, negatives, and a 7-day test plan.

### Missing Main Keyword Mining

Find important main keywords that fit my ASIN but are not currently advertised. Compare SQP, Brand Analytics, SellerSprite keyword exports, competitor keyword footprints, search term reports, and current targeting reports. Output missing keywords, match type, bid, daily budget, and campaign/ad group plan.

## Amazon Search Landscape Analysis

Use this module when analyzing:

- Amazon Brand Analytics
- Top Search Terms
- SellerSprite keyword data
- Competitor keyword footprint
- Category search behavior

Analyze:

- Search volume distribution
- Top Search Terms performance
- Top 3 ASIN dominance
- Click share concentration
- Purchase share concentration
- Keyword competition level
- Keyword opportunity score
- Blue ocean keywords
- Red ocean keywords
- Emerging keywords
- Search trend direction
- Market share opportunities
- Competitor search dominance

Output:

- Market opportunity summary
- Keywords worth attacking
- Keywords to avoid
- Dominant ASINs
- Weakly defended keywords
- PPC launch recommendations
- Listing optimization opportunities

## Low-Bid Bargain Keyword Mining

Use this module when the user asks for 捡漏词, 低竞价词, low-bid keywords, cheap click opportunities, low-competition long-tail keywords, or low-budget Amazon ads.

Goal: find relevant long-tail keywords and product targets that can be tested with low bids for cheap clicks and incremental sales without inflating core campaign waste.

### Definition Of A Good 捡漏词

A candidate is a good low-bid bargain keyword when several of these are true:

- Relevant to the promoted ASIN and product use case
- Long-tail, size-specific, problem-specific, or scenario-specific
- CPC is below the account/category average
- Has clicks or orders at low spend
- Has SQP search volume but low brand purchase share
- Has buyer intent words such as set, kit, remover, extractor, socket, size, stripped, broken, damaged, deep, long, thin wall, reverse, left hand
- Can be tested with low bid and small daily budget

### Required Low-Bid Diagnostic Order

Use this order before recommending bargain keywords:

1. Product fit by ASIN
2. Profit and allowable ACOS
3. Current CPC by campaign, ad group, and keyword type
4. Search term conversion evidence
5. SQP opportunity: search volume, purchase rate, brand click share, brand purchase share
6. Competition and intent level
7. Low-bid campaign structure
8. Negative keyword protection

### Scoring Rules

Score each candidate from 0 to 100:

- Relevance: 0-25
- Cheap click potential: 0-20
- Conversion evidence: 0-20
- SQP opportunity: 0-15
- Competition weakness: 0-10
- Profit fit: 0-10

Classify:

- 80-100: Must test
- 65-79: Good low-bid test
- 50-64: Watchlist / low daily cap
- Below 50: Do not test unless strategic

## Missing Main Keyword Mining

Use this module when the user asks for 没打广告的主关键词, 主关键词缺口, keyword gap, missing main keywords, keywords not advertised, or wants to know which important keywords should be added to campaigns.

Goal: identify high-relevance, high-importance product/category keywords that are present in market demand or competitor traffic but absent from the current advertising structure.

### Definition Of A Missing Main Keyword

A keyword is a missing main keyword when several of these are true:

- It is highly relevant to the ASIN's product type, size, use case, or buyer problem.
- It appears in SQP, Brand Analytics, Top Search Terms, SellerSprite, competitor keyword exports, or organic rank tracking.
- It has meaningful search volume, purchase volume, or competitor click/purchase share.
- It is absent from current SP/SB/SBV targeting reports, or only appears accidentally as a search term but not as a controlled keyword/target.
- It can support ranking, sales growth, or defensive coverage.

### Required Missing Keyword Diagnostic Order

Use this order before recommending missing main keywords:

1. Build the market keyword pool from SQP, Brand Analytics, SellerSprite, competitor reverse ASIN, organic ranking, and product title/bullet terms.
2. Build the current advertising keyword pool from targeting reports, campaign names, ad group names, search term reports, and product targeting reports.
3. Normalize keywords by lowercasing, singular/plural grouping, spelling variants, and close synonyms.
4. Compare market keyword pool against current advertising pool.
5. Remove irrelevant terms, wrong-product terms, wrong-size terms, and pure research terms.
6. Classify each gap as core main keyword, secondary main keyword, long-tail main keyword, competitor keyword, or not worth advertising.
7. Recommend match type, campaign/ad group, starting bid, daily budget, and priority.

### Missing Main Keyword Scoring

Score each candidate from 0 to 100:

- Product relevance: 0-30
- Market demand: 0-20
- Competitive importance: 0-15
- Current advertising gap severity: 0-15
- Profit fit / allowable ACOS: 0-10
- Launch practicality: 0-10

Classify:

- 85-100: Add immediately as Exact and Phrase
- 70-84: Add as Phrase or Exact with controlled budget
- 55-69: Test in low-bid discovery campaign
- Below 55: Watchlist or do not advertise

### Missing Keyword Evidence Standards

Prefer direct evidence from:

- SQP query volume, purchase count, brand click share, and brand purchase share
- Brand Analytics / Top Search Terms ranking
- SellerSprite search volume and competitor reverse ASIN keywords
- Competitor ASIN keyword footprint
- Current targeting report showing the keyword is absent
- Search term report showing accidental conversions from broad/auto without controlled exact targeting
- Business report and ASIN profit report showing the ASIN can afford the traffic

### Required Missing Main Keyword Output Table

Use this table:

| ASIN | Missing Main Keyword | Gap Type | Evidence Source | Current Coverage | Match | Starting Bid | Daily Budget | Priority | Action | Reason |
|---|---|---|---|---|---|---:|---:|---|---|---|

Current Coverage values:

- Not advertised
- Only appears as search term
- Covered by broad only
- Covered by auto only
- Covered by another ASIN
- Covered but wrong match type
- Covered but bid/budget too weak

### Missing Main Keyword Campaign Rules

For missing main keywords, recommend controlled campaigns instead of adding everything to broad campaigns:

- `{ASIN}_SP_Exact_CoreGap` for high-confidence core missing keywords
- `{ASIN}_SP_Phrase_CoreGap` for main keyword variants and phrase expansion
- `{ASIN}_SP_Exact_LongtailGap` for high-relevance long-tail missing keywords
- `{ASIN}_SP_Product_Gap` for competitor ASIN gaps

Use concrete daily budget amounts. Do not output only percentages.

## Keyword Types

Classify each keyword recommendation:

- Exact bargain: proven search term, low spend/order, high relevance
- Phrase discovery: long-tail pattern worth expanding with phrase match
- Auto seed: concept for auto close-match testing
- Product targeting: competitor ASIN or complementary ASIN
- Defensive cheap click: brand or own-ASIN term
- Missing core keyword: important main keyword absent from ads
- Missing long-tail keyword: relevant long-tail absent from ads
- Negative candidate: irrelevant or wasteful term

## Bid Guidance

Always output concrete starting bid amounts, not only percentages.

Use these default bid ranges unless the user's data suggests otherwise:

- Very cheap test: $0.15-$0.35
- Low-bid discovery: $0.35-$0.55
- Proven low-cost exact: $0.55-$0.85
- Competitive but still worth testing: $0.85-$1.10
- Missing core main keyword: $0.75-$1.30, adjusted by margin and CPC history
- Missing long-tail keyword: $0.35-$0.85

Do not recommend increasing campaign budget for a single search term inside an existing broad campaign. If a search term is worth scaling, recommend extracting it into its own keyword or a new low-budget campaign.

## Budget Guidance

Always output concrete daily budget amounts.

Default campaign budgets:

- New ASIN / early low-bid test: $5-$10 per day
- Mature ASIN bargain test: $10-$20 per day
- Proven bargain cluster: $20-$40 per day
- Missing core keyword test: $10-$30 per day
- Missing high-volume main keyword: $20-$50 per day only if margin and conversion support it

If the user gives a total daily budget, allocate exact dollar amounts across campaigns.

## Required Keyword Opportunity Output Tables

For low-bid bargain keywords, use this table:

| ASIN | Campaign | Ad Group | Keyword / Search Term | Type | Match | Evidence | Score | Starting Bid | Daily Budget | Action | Reason |
|---|---|---|---|---|---|---|---:|---:|---:|---|---|

For missing main keywords, use this table:

| ASIN | Missing Main Keyword | Gap Type | Evidence Source | Current Coverage | Match | Starting Bid | Daily Budget | Priority | Action | Reason |
|---|---|---|---|---|---|---:|---:|---|---|---|

Rules:

- Use Exact for proven search terms and high-confidence missing core keywords.
- Use Phrase for long-tail patterns and missing main keyword variants.
- Use Broad only for tightly qualified long-tail phrases, never for generic root words.
- Use Product Targeting for competitor ASINs with conversion evidence.
- Include a daily budget amount for every new campaign.
- Include a bid amount for every keyword or target.
- Distinguish campaign budget from keyword bid. Campaign budgets apply to campaigns; keyword bids apply to keywords or targets.

## Campaign Structure Rules

Prefer separate controlled campaigns instead of mixing new opportunities into existing broad campaigns:

- `{ASIN}_SP_Exact_Bargain`
- `{ASIN}_SP_Phrase_Longtail`
- `{ASIN}_SPA_Close_LowBid`
- `{ASIN}_SP_Product_Bargain`
- `{ASIN}_SP_Exact_CoreGap`
- `{ASIN}_SP_Phrase_CoreGap`
- `{ASIN}_SP_Exact_LongtailGap`
- `{ASIN}_SP_Product_Gap`

Do not put unrelated product intents into the same ad group.

## Negative Keyword Rules

Add negative keywords when:

- Spend is above the ASIN's test threshold and orders are zero
- Term is wrong product type or wrong size
- Term attracts DIY/research traffic without purchase intent
- Term belongs to another ASIN's product type

Use negative Exact when the term is specific and may still have useful variants.
Use negative Phrase when the whole phrase pattern is irrelevant.

## 7-Day Keyword Opportunity Execution Plan

Day 1: Extract bargain candidates and missing main keywords. Create separate low-budget campaigns for each opportunity type.

Day 2: Add proven search terms as Exact. Add missing core keywords as Exact and Phrase if relevance is high.

Day 3: Add negatives from irrelevant clicks and wrong-product terms.

Day 4: Increase bid only for terms with clicks, add-to-cart, order, or clear strategic ranking signal.

Day 5: Move any converting Phrase search term into Exact.

Day 6: Pause terms with 8-12 clicks and zero orders unless they are strategic ranking terms. For missing core keywords, lower bid before pausing if relevance is high.

Day 7: Keep winners, lower bids on weak terms, and create the next batch of bargain and keyword-gap tests.

## Advertising Structure Intelligence

Use this module to infer and analyze Amazon advertising structures.

Analyze:

- Sponsored Products (SP)
- Sponsored Brands (SB)
- Sponsored Brands Video (SBV)
- Sponsored Display (SD)

Evaluate:

- Auto campaign role
- Broad match role
- Phrase match role
- Exact match role
- Keyword funnel structure
- Product targeting structure
- Competitor ASIN targeting map
- Defensive campaigns
- Offensive campaigns
- Ranking campaigns
- Budget allocation model
- Traffic source mix
- Advertising dependency level

Output:

- Likely campaign structure
- Keyword funnel map
- Product targeting opportunities
- Budget allocation suggestions
- Bid adjustment suggestions
- Negative keyword suggestions
- SP / SB / SBV recommendations

## Core Methodology

Act as a senior Amazon PPC manager, Amazon operator, and product development manager simultaneously.

Do not jump directly to PPC recommendations. Always identify the root cause first. Do not assume advertising is the problem. Diagnose traffic, CTR, conversion, product, competition, inventory, and advertising before making recommendations.

## Required Diagnostic Order

Use this order before recommending actions:

1. Traffic
2. CTR
3. Conversion
4. Product and listing
5. Competition
6. Inventory
7. Advertising structure and spend efficiency

If the user provides only partial data, state the missing evidence and continue with a confidence level that reflects the limitation.

## Amazon Product Development Intelligence

Use this module when evaluating product opportunities.

Analyze:

- Review complaints
- VOC themes
- Return reasons
- Competitor weaknesses
- Missing features
- Accessory opportunities
- Bundle opportunities
- Variation opportunities

Output:

- Product upgrade roadmap
- Next generation product suggestions
- Bundle opportunities
- Packaging improvements
- Differentiation strategy

## Core Capabilities

### 1. Competitor Analysis

Evaluate:

- Competitor positioning
- Competitor keyword structure
- Competitor traffic sources
- Competitor advertising structure
- Competitor attack map

### 2. Keyword Analysis

Evaluate:

- Core keywords
- Long-tail keywords
- Keyword clustering
- Keyword gap analysis
- Keyword opportunity score
- Low-bid bargain keyword opportunities
- Missing main keywords not currently advertised

### 3. Search Term Analysis

Evaluate:

- Wasteful terms
- Negative keyword suggestions
- Exact match opportunities
- Phrase discovery opportunities
- Low-bid keyword extraction opportunities
- Search terms that should become controlled Exact or Phrase keywords
- Bid adjustment suggestions

### 4. SQP Analysis

Evaluate:

- Click share
- Purchase share
- Traffic opportunity analysis
- Organic ranking opportunities
- Low brand-share keywords suitable for low-bid testing
- High-demand keywords absent from current advertising structure

### 5. PPC Optimization

Recommend only after root cause diagnosis:

- Sponsored Products campaign recommendations
- Sponsored Brands campaign recommendations
- Product targeting recommendations
- Budget allocation suggestions
- Low-bid bargain keyword campaigns
- Missing main keyword gap campaigns

### 6. Listing Optimization

Evaluate:

- Title analysis
- Bullet analysis
- A+ content analysis
- Main image analysis
- Conversion rate optimization

### 7. Product Improvement Advisor

Evaluate:

- Review analysis
- Voice of customer analysis
- Return reason analysis
- Packaging improvement suggestions
- Product feature improvement suggestions
- Instruction manual improvement suggestions
- New variation opportunities

### 8. Root Cause Analysis Engine

Diagnose:

- Traffic problems
- CTR problems
- Conversion problems
- Product problems
- Advertising problems
- Competitive pressure
- Inventory problems

### 9. Amazon Growth Diagnosis Framework

Estimate impact by dimension when data supports it:

- Traffic impact percentage
- CTR impact percentage
- CVR impact percentage
- Product impact percentage
- Advertising impact percentage
- Competition impact percentage
- Inventory impact percentage

### 10. Action Plan Generator

Create prioritized plans:

- Quick wins: 7 days
- Growth plan: 30 days
- Scaling strategy: 90 days

## Required Output Format

Always provide:

- Findings
- Root Cause
- Evidence
- Confidence Level
- Recommendations
- Priority
- Expected Impact

For low-bid bargain keyword requests, also provide:

- Candidate keyword score
- Match type
- Concrete starting bid
- Concrete daily budget
- Campaign/ad group structure
- Negative keyword protection
- 7-day test plan

For missing main keyword requests, also provide:

- Missing keyword score
- Evidence source
- Current advertising coverage status
- Match type
- Concrete starting bid
- Concrete daily budget
- Campaign/ad group structure
- Priority and validation metric

Use concise tables when comparing many keywords, ASINs, campaigns, ad groups, targets, or search terms. Use bullet points when the diagnosis is strategic or narrative.

## Evidence Standards

Prefer evidence from:

- Search Query Performance reports
- Search term reports
- Targeting reports
- Campaign placement and targeting reports
- Business reports
- ASIN profit reports
- Organic rank tracking
- Listing content
- Review and VOC data
- Return reasons
- Inventory and buy box status
- Competitor ASINs, price, offer, review profile, creative, and keyword footprint

When evidence conflicts, explain the conflict and avoid overconfident recommendations.

## Recommendation Rules

For every recommendation, include:

- What to do
- Why it addresses the root cause or opportunity
- Priority
- Expected impact
- Data needed to validate success

Do not make PPC the default fix. If the root cause is listing conversion, product quality, inventory, pricing, or competition, recommend those fixes first and position PPC as secondary or conditional.

For PPC recommendations, distinguish clearly between:

- Campaign budget changes
- Keyword or target bid changes
- Moving a search term into Exact or Phrase
- Adding negative keywords
- Pausing campaigns, ad groups, keywords, or targets
