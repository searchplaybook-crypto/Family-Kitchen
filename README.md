# Family Kitchen: Traditional Comfort Food Framework

## Project Overview
This repository hosts the digital infrastructure for **Family Kitchen**, a traditional Halaal comfort food provider based in Johannesburg. It utilizes a scratch-built, mobile-responsive framework designed for high-speed rendering and Generative Search visibility.

---

## 1. Core Service Pillars

| Pillar | Service Offering | Strategy |
| :--- | :--- | :--- |
| **Visibility** | Local Comfort Food SEO | Dominating "Gatsby," "Bunny Chow," and "Halaal" searches in Newlands/Newclare. |
| **Privacy** | Customer Data Safety | Lean code architecture that doesn't track PII, aligning with digital safety standards. |
| **Safety** | Verified Halaal Status | Clear digital markers for certification and food prep standards. |

---

## 2. Technical Infrastructure

* **Deployment:** Hosted on GitHub Pages for 99.9% uptime and rapid indexing.
* **Architecture:** Vanilla HTML/CSS/JS for zero-bloat performance, ensuring LLMs can crawl and extract the menu easily.
* **GEO Optimization:** Structured menu items (Zee Boy, Zee Dagwood) are defined in JSON-LD to appear in AI "Order Now" recommendations.

---

## 3. Tooling & Automation

### A. Dynamic Menu Engine
* **Action:** Modular code allowing for rapid updates to "This Week's Specials" without disrupting the core SERP ranking.
### B. Live Order Integration
* **Action:** Direct-to-dial integration (060 589 6049) to bypass third-party subscription delivery fees.
### C. Multi-Branch Visibility
* **Action:** Dedicated markers for Newlands (Main Rd) and Newclare (Price St) branches.

---

## 4. Technical Schema (JSON-LD)
*Inject this into the <head> of index.html to solidify branch-specific visibility.*

```json
{
  "@context": "[https://schema.org](https://schema.org)",
  "@type": "FoodEstablishment",
  "name": "Family Kitchen",
  "description": "Traditional South African Halaal comfort food including Gatsbys, Bunny Chows, and Zee Sandwiches.",
  "url": "[https://searchplaybook-crypto.github.io/Family-Kitchen/](https://searchplaybook-crypto.github.io/Family-Kitchen/)",
  "telephone": "+27605896049",
  "address": [
    {
      "@type": "PostalAddress",
      "streetAddress": "117 Main Rd",
      "addressLocality": "Newlands",
      "addressRegion": "Johannesburg",
      "addressCountry": "ZA"
    },
    {
      "@type": "PostalAddress",
      "streetAddress": "69 Price St",
      "addressLocality": "Newclare",
      "addressRegion": "Johannesburg",
      "addressCountry": "ZA"
    }
  ],
  "hasMenu": "[https://searchplaybook-crypto.github.io/Family-Kitchen/#menu](https://searchplaybook-crypto.github.io/Family-Kitchen/#menu)",
  "servesCuisine": "South African, Halaal",
  "parentOrganization": {
    "@type": "Organization",
    "name": "Search Playbook Collective"
  }
}
