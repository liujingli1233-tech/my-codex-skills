# Intake Schema

Before generating listing content, normalize user input into these fields when available:

```yaml
task_mode: full_pack | single_module | optimize_existing
marketplace: US
language: en-US
product_name: ""
brand: ""
category_term: ""
audience_scenarios: []
usps: []
specs: []
compatibility:
  supported: []
  unsupported: []
package_contents: []
materials: []
certifications: []
keyword_pool:
  core: []
  secondary: []
  long_tail: []
competitor_insights: []
review_insights:
  pains: []
  expectations: []
  misuse: []
compliance_notes: []
existing_listing:
  title: ""
  bullets: []
  description: ""
  search_terms: ""
```

## Rules

- User-provided facts have highest priority.
- Do not invent dimensions, quantities, materials, compatibility, certifications, warranty, or safety claims.
- If a missing fact blocks accurate output, ask only for that fact.
- For Amazon US, output front-end copy in English unless the user asks otherwise.
