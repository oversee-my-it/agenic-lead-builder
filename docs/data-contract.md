
# Agenic Lead Builder – Data Contract

## Top-level JSON
```json
{
  "sales_summary": { ... },
  "report_text": "string",
  "sections": { ... },
  "contacts": [ ... ],
  "compliance": { ... },
  "memberships": [ ... ],
  "sources": [ "url1", "url2", "..." ]
}
```

## sales_summary
- icp_match: string (High|Medium|Low)
- best_sales_contact_title: string
- regulation_status: string
- lead_type: string
- services_fit: [string]

## contacts[]
- name: string
- title: string
- profile_url: string
- role_class: string (Economic Buyer|Technical Buyer|Influencer)

## compliance
- status: string (Regulated|Likely Regulated|Inconclusive|Not Regulated)
- evidence: [ { "phrase": string, "page_section": string } ]
- confidence: string (High|Medium|Low)

## memberships[]
- org_name: string
- proof_text: string
- page_section: string

## sources[]
- url: string
```
