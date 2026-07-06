# Module Prompts

## Output Order

For a full Amazon listing package, output in this order:

1. Title
2. Bullet Points
3. Search Terms
4. Product Description in Amazon-compatible HTML format
5. Main and secondary image brief
6. A+ content brief
7. Video script
8. Rufus Q&A validation
9. Listing self-check

## Global Visual Fidelity Rule

- Product appearance, structure, color, texture, accessories, package, storage case, labels, logo, size markings, and quantity must stay 100% consistent with the user's provided product photos or confirmed product facts.
- Do not redesign the product, change its structure, change colors, add missing parts, remove real parts, invent packaging, change the storage case, or create a different product style.
- You may improve composition, lighting direction, clarity, background, callout hierarchy, and information layout, but the physical product and packaging must remain exactly the same.
- If any visual detail is unclear, mark it as needing user confirmation instead of guessing.
- Any image, A+, or video brief for designers or AI image tools must include: `Use the provided product photo as the source of truth; keep product appearance, structure, color, accessories, packaging, and quantity exactly the same; do not redesign the product.`

## Title

- Put the main category keyword near the beginning.
- Include 1-2 high-value keywords, 1-2 clear differentiators, and key specs when useful.
- Keep it readable on mobile.
- Avoid exaggerated claims, medical claims, competitor brands, ASINs, and unsupported promises.
- For US listings, write in English.

## Bullet Points

- Output exactly 5 bullet points unless the user asks otherwise.
- Put the strongest conversion points in bullets 1-2.
- Put specs, compatibility, material, package contents, use cases, and Rufus-supporting facts in bullets 3-5.
- Each bullet should focus on one main idea.
- Include confirmed sizes, quantities, drive types, materials, and compatibility when provided.
- Do not invent specs, certifications, warranty, safety conclusions, or compatibility.

## Search Terms

- Output one line only.
- Use spaces only. Do not use commas, punctuation, brand names, competitor names, ASINs, promotional claims, or subjective words.
- Keep under Amazon backend byte limits, normally under 249 bytes for US listings.
- Avoid repeated words, repeated roots, and repeated meanings as much as possible.
- Remove words already used in the title and bullet points unless essential.
- Prioritize uncovered buyer search intents, synonyms, use cases, misspellings, and problem words.
- Good style example: `stripped wheel nut socket locking remover twist extractor rounded bolt rusted frozen tire repair impact tool`
- Bad style example: `lug nut extractor lug nut remover lug nut removal wheel nut remover damaged lug nut socket`

## Product Description HTML

- Output Product Description in Amazon-compatible HTML format by default.
- Use `<p>...</p>` for paragraphs and `<b>...</b>` for bold section headings.
- Allowed default tags: `<p>`, `<b>`, and `<br>`.
- Do not use tables, scripts, styles, unsupported layout HTML, links, or decorative markup.
- Keep text concise and suitable for Seller Central.
- For US listings, write the visible description text in English.

Example:
```html
<p><b>Professional Extraction for Real Repair Situations</b></p>
<p>Stripped, rusted, or broken fasteners can stop your work instantly. This extractor set is engineered to solve those problems efficiently, even in deep, narrow, and hard-to-reach spaces.</p>
<p>✓ Slim design reaches tight and recessed areas</p>
<p>✓ CR-MO steel delivers strength under high torque</p>
<p>✓ Compatible with multiple tool systems</p>
<p>From automotive repair to home maintenance and industrial applications, this kit gives you the control, flexibility, and confidence to remove damaged fasteners quickly and effectively.</p>
```

## Image Brief

- Main image: pure white background, no text, no logo overlays, no watermark.
- Product and packaging must match the provided real product photos exactly.
- Image 2-3: focus on the strongest conversion points without changing the product's actual appearance or structure.
- Image 4-6: show use cases, specs, compatibility, material, and trust-building details while keeping the real product unchanged.
- Image 7: package contents, storage, size chart, or variant comparison using the real accessories and package contents only.
- Do not ask designers or AI tools to create a new product model, new packaging, new colorway, or invented accessory.

## A+ Brief

- Structure modules around value proposition, key function, user scenario, material/quality, comparison, and package contents.
- Product visuals, diagrams, package contents, and comparison images must be based on the actual product photos and confirmed facts.
- Keep copy direct and factual.
- Do not include promotional claims, unsupported superiority, medical claims, or competitor names.
- Do not redesign product appearance, packaging, accessories, or storage layout for A+ visuals.

## Video Script

- Default length: 30 seconds.
- Use 3-5 second scenes.
- Show the problem, product solution, key specs, how it works, and package contents.
- Product appearance, structure, accessories, packaging, and quantity shown in the video must match the user's provided product photos and facts.
- Do not make claims not supported by the listing facts.
- Do not script a redesigned product, new packaging, or invented use configuration.

## Rufus Q&A Validation

- Generate buyer-style questions based only on the title, bullets, description, search terms, and confirmed specs.
- Answers must only use explicit listing information.
- If the listing does not provide enough information, write that the answer cannot be confirmed.

## Listing Self-Check

Check these areas:

- Title readability and keyword placement
- Bullet clarity and factual support
- Description consistency
- Search Terms duplication and backend compliance
- Image/A+ consistency
- Product visual fidelity: appearance, structure, colors, accessories, package, labels, logo, size markings, and quantity must match the source photos and confirmed facts
- Rufus answerability
- Missing specs or compatibility risks
