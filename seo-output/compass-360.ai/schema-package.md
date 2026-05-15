# Schema Markup Package — compass-360.ai

All blocks use JSON-LD format. Place in `<script type="application/ld+json">` in `<head>`.

---

## Block 1 — Organization + WebSite (all pages, in `<head>`)

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Organization",
      "@id": "https://compass-360.ai/#organization",
      "name": "Compass 360 AI",
      "url": "https://compass-360.ai",
      "logo": {
        "@type": "ImageObject",
        "url": "https://compass-360.ai/images/compass-360-ai-logo.png",
        "width": 300,
        "height": 60
      },
      "description": "Vendor-neutral enterprise AI advisory consultancy helping organizations in GCC/MENA and the United States navigate AI readiness, strategy, governance, and enablement.",
      "foundingDate": "2024",
      "founder": { "@id": "https://compass-360.ai/#ali-dahmash" },
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Tampa",
        "addressRegion": "FL",
        "addressCountry": "US"
      },
      "areaServed": [
        { "@type": "Place", "name": "United States" },
        { "@type": "Place", "name": "United Arab Emirates" },
        { "@type": "Place", "name": "Saudi Arabia" },
        { "@type": "Place", "name": "Qatar" },
        { "@type": "Place", "name": "Kuwait" },
        { "@type": "Place", "name": "Bahrain" },
        { "@type": "Place", "name": "Oman" }
      ],
      "knowsAbout": [
        "Enterprise AI Strategy",
        "AI Governance",
        "AI Readiness Assessment",
        "AI Advisory Consulting",
        "ISO 42001",
        "NIST AI RMF",
        "GCC Digital Transformation"
      ],
      "sameAs": [
        "https://www.linkedin.com/company/compass-360-ai"
      ],
      "contactPoint": {
        "@type": "ContactPoint",
        "contactType": "customer service",
        "url": "https://compass-360.ai/contact",
        "availableLanguage": ["English", "Arabic"]
      }
    },
    {
      "@type": "WebSite",
      "@id": "https://compass-360.ai/#website",
      "url": "https://compass-360.ai",
      "name": "Compass 360 AI",
      "description": "Enterprise AI advisory, strategy, and governance consulting for GCC/MENA and US markets.",
      "publisher": { "@id": "https://compass-360.ai/#organization" }
    }
  ]
}
```

> Update `logo` URL, `sameAs` URLs, and `foundingDate` to verified values before deploying.

---

## Block 2 — Person: Ali Dahmash (homepage + /about)

```json
{
  "@context": "https://schema.org",
  "@type": "Person",
  "@id": "https://compass-360.ai/#ali-dahmash",
  "name": "Ali Dahmash",
  "jobTitle": "Founder & AI Strategy Advisor",
  "worksFor": { "@id": "https://compass-360.ai/#organization" },
  "url": "https://compass-360.ai/about",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Tampa",
    "addressRegion": "FL",
    "addressCountry": "US"
  },
  "knowsAbout": [
    "Enterprise AI Strategy",
    "AI Governance",
    "AI Readiness Assessment",
    "Digital Transformation",
    "GCC Technology Markets",
    "MENA Enterprise Technology"
  ],
  "sameAs": [
    "https://www.linkedin.com/in/alidahmash"
  ]
}
```

---

## Block 3 — Service: AI Readiness Assessment (/ai-readiness-assessment)

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Service",
      "@id": "https://compass-360.ai/ai-readiness-assessment#service",
      "name": "AI Readiness Assessment",
      "serviceType": "AI Readiness Assessment",
      "description": "Proprietary SAiGE 5-step enterprise AI readiness assessment evaluating data infrastructure, talent capability, governance frameworks, and technology maturity. Delivers a scorecard in 48 hours.",
      "provider": { "@id": "https://compass-360.ai/#organization" },
      "areaServed": [
        { "@type": "Place", "name": "United States" },
        { "@type": "Place", "name": "Gulf Cooperation Council" },
        { "@type": "Place", "name": "Middle East and North Africa" }
      ],
      "url": "https://compass-360.ai/ai-readiness-assessment"
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://compass-360.ai" },
        { "@type": "ListItem", "position": 2, "name": "AI Readiness Assessment", "item": "https://compass-360.ai/ai-readiness-assessment" }
      ]
    }
  ]
}
```

---

## Block 4 — Service: AI Enablement & Governance (/ai-enablement-governance)

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Service",
      "@id": "https://compass-360.ai/ai-enablement-governance#service",
      "name": "AI Enablement & Governance",
      "serviceType": "AI Governance Consulting",
      "description": "Enterprise AI governance frameworks aligned to ISO 42001 and NIST AI RMF. Policy design, risk management protocols, and responsible AI adoption programs for GCC/MENA and US enterprises.",
      "provider": { "@id": "https://compass-360.ai/#organization" },
      "areaServed": [
        { "@type": "Place", "name": "United States" },
        { "@type": "Place", "name": "Gulf Cooperation Council" },
        { "@type": "Place", "name": "Middle East and North Africa" }
      ],
      "url": "https://compass-360.ai/ai-enablement-governance"
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://compass-360.ai" },
        { "@type": "ListItem", "position": 2, "name": "AI Governance Consulting", "item": "https://compass-360.ai/ai-enablement-governance" }
      ]
    }
  ]
}
```

---

## Block 5 — Service: AI Advisory & Consulting (/ai-advisory-consulting)

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Service",
      "@id": "https://compass-360.ai/ai-advisory-consulting#service",
      "name": "AI Advisory & Consulting",
      "serviceType": "AI Advisory Consulting",
      "description": "Ongoing vendor-neutral AI advisory for C-suite and executive leadership teams. Helps CIOs, CDOs, and CEOs navigate AI investment decisions, vendor selection, and enterprise AI program design.",
      "provider": { "@id": "https://compass-360.ai/#organization" },
      "areaServed": [
        { "@type": "Place", "name": "United States" },
        { "@type": "Place", "name": "Gulf Cooperation Council" },
        { "@type": "Place", "name": "Middle East and North Africa" }
      ],
      "url": "https://compass-360.ai/ai-advisory-consulting"
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://compass-360.ai" },
        { "@type": "ListItem", "position": 2, "name": "AI Advisory & Consulting", "item": "https://compass-360.ai/ai-advisory-consulting" }
      ]
    }
  ]
}
```

---

## Block 6 — Service: AI Strategy & Roadmap (/ai-strategy-roadmap)

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Service",
      "@id": "https://compass-360.ai/ai-strategy-roadmap#service",
      "name": "AI Strategy & Roadmap",
      "serviceType": "AI Strategy Development",
      "description": "End-to-end AI strategy development and 12–18 month roadmap design for enterprise organizations, aligning AI investment with business objectives and competitive positioning.",
      "provider": { "@id": "https://compass-360.ai/#organization" },
      "areaServed": [
        { "@type": "Place", "name": "United States" },
        { "@type": "Place", "name": "Gulf Cooperation Council" },
        { "@type": "Place", "name": "Middle East and North Africa" }
      ],
      "url": "https://compass-360.ai/ai-strategy-roadmap"
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://compass-360.ai" },
        { "@type": "ListItem", "position": 2, "name": "AI Strategy & Roadmap", "item": "https://compass-360.ai/ai-strategy-roadmap" }
      ]
    }
  ]
}
```

---

## Block 7 — Service: Enterprise AI Training (/enterprise-ai-training)

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Service",
      "@id": "https://compass-360.ai/enterprise-ai-training#service",
      "name": "Enterprise AI Training",
      "serviceType": "AI Training and Upskilling",
      "description": "Customized role-based AI literacy and upskilling programs for enterprise teams. Covers AI strategy, governance, responsible AI adoption, and practical AI tool application.",
      "provider": { "@id": "https://compass-360.ai/#organization" },
      "areaServed": [
        { "@type": "Place", "name": "United States" },
        { "@type": "Place", "name": "Gulf Cooperation Council" },
        { "@type": "Place", "name": "Middle East and North Africa" }
      ],
      "url": "https://compass-360.ai/enterprise-ai-training"
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://compass-360.ai" },
        { "@type": "ListItem", "position": 2, "name": "Enterprise AI Training", "item": "https://compass-360.ai/enterprise-ai-training" }
      ]
    }
  ]
}
```

> Do NOT use `Course` schema — retired from Google rich results June 2025. `Service` is correct for consulting-delivered training.

---

## Block 8 — ContactPage (/contact)

```json
{
  "@context": "https://schema.org",
  "@type": "ContactPage",
  "url": "https://compass-360.ai/contact",
  "name": "Contact Compass 360 AI",
  "description": "Get in touch with the Compass 360 AI team to discuss AI readiness assessments, strategy engagements, or advisory services.",
  "isPartOf": { "@id": "https://compass-360.ai/#website" },
  "about": { "@id": "https://compass-360.ai/#organization" }
}
```

---

## Validation

After deploying all blocks:
1. Google Rich Results Test: https://search.google.com/test/rich-results
2. Schema Markup Validator: https://validator.schema.org
3. GSC Enhancements panel: breadcrumbs and sitelinks searchbox appear 1–4 weeks after Google recrawls
