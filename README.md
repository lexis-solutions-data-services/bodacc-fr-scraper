# Bodacc.fr French Legal Gazette Scraper

![Bodacc.fr French Legal Gazette Scraper](https://i.ibb.co/XrVbYVF0/bodacc-cover.png)

This Apify actor collects structured legal gazette announcements from **BODACC.fr**, France's official civil and commercial bulletin. Capture rich public notice data covering company events, registrations, insolvencies, and commercial activity updates — ideal for compliance workflows, risk monitoring, and market intelligence.

<p align="center">
  <img src="https://apify-image-uploads-prod.s3.us-east-1.amazonaws.com/DevbkY3adMTBuoECt-actor-4OXGCcZrCsGelkwhi-Fc0MjZxiju-Screenshot_2025-11-11_at_21.42.11.png" alt="Bodacc.fr Scraper" style="height: 60px; margin-right: 15px;" /><a href="https://apify.com/lexis-solutions/bodacc-fr-scraper" target="_blank">
    <img src="https://img.shields.io/badge/Try%20it%20on-Apify-0066FF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDA4IiBoZWlnaHQ9IjQwOCIgdmlld0JveD0iMCAwIDQwOCA0MDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMF8zNDFfNDE1NykiPgo8cGF0aCBkPSJNMjE4LjY5NSAxMDRIMzAwLjk3QzMwMi42NDMgMTA0IDMwNCAxMDUuMzU3IDMwNCAxMDcuMDNWMjMyLjc2NkMzMDQgMjM1Ljc3OCAzMDAuMDgzIDIzNi45NDUgMjk4LjQzNCAyMzQuNDI1TDIxNi4xNTkgMTA4LjY5QzIxNC44NDEgMTA2LjY3NCAyMTYuMjg3IDEwNCAyMTguNjk1IDEwNFoiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0xODkuMzA1IDEwNEgxMDcuMDNDMTA1LjM1NyAxMDQgMTA0IDEwNS4zNTcgMTA0IDEwNy4wM1YyMzIuNzY2QzEwNCAyMzUuNzc4IDEwNy45MTcgMjM2Ljk0NSAxMDkuNTY2IDIzNC40MjVMMTkxLjg0IDEwOC42OUMxOTMuMTU5IDEwNi42NzQgMTkxLjcxMyAxMDQgMTg5LjMwNSAxMDRaIiBmaWxsPSJ3aGl0ZSIvPgo8cGF0aCBkPSJNMjAyLjU5MSAyMDQuNjY4TDEwOS4xMjcgMjk4LjgzNUMxMDcuMjI5IDMwMC43NDcgMTA4LjU4MyAzMDQgMTExLjI3OCAzMDRIMjk2LjhDMjk5LjQ4MyAzMDQgMzAwLjg0MiAzMDAuNzcgMjk4Ljk2NyAyOTguODUyTDIwNi45MDggMjA0LjY4NUMyMDUuNzI2IDIwMy40NzUgMjAzLjc4MiAyMDMuNDY4IDIwMi41OTEgMjA0LjY2OFoiIGZpbGw9IndoaXRlIi8+CjwvZz4KPGRlZnM+CjxjbGlwUGF0aCBpZD0iY2xpcDBfMzQxXzQxNTciPgo8cmVjdCB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEwNCAxMDQpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==&logoColor=white" alt="Try it on Apify" style="border-radius: 12px; height: 60px;" />
  </a>
</p>


---


## 📊 Actor Stats

| Stat | Value |
|------|-------|
| **Version** | `0.1.1` |
| **Last Update** | Dec 1, 2025 |

---



## 💻 Integration Examples

This repository includes example code showing how to integrate the `bodacc-fr-scraper` actor into your projects.

You can find example implementations in the [`examples/`](./examples) folder:
- **TypeScript/JavaScript**: See [`examples/typescript/`](./examples/typescript) for a complete TypeScript example
- **Python**: See [`examples/python/`](./examples/python) for a complete Python example

Each example includes:
- Ready-to-use code templates
- Setup instructions
- Documentation links

---


## 🚀 Key Features

- 🔍 Scrape commercial announcements, legal notices, and insolvency updates from **BODACC.fr**
- 📥 Retrieve establishment, person, and act metadata in a consistent schema
- 🕒 Track publication dates, edition numbers, and court jurisdictions
- 🧭 Automatically paginate through result sets and stop at `maxItems`

---

## ❓ Why Use This Actor

- ✅ Automate monitoring of French commercial court announcements
- ✅ Enrich KYC, AML, and compliance datasets with authoritative public records
- ✅ Surface corporate events (creations, transfers, liquidations) in near real time
- ✅ Reduce manual browsing of the Bodacc portal and downloadable PDFs
- ✅ Feed structured data into case management or risk platforms
- ✅ Build historical archives for research, analytics, or investigative work

---

## 👥 Who Is This Actor Suitable For?

- ⚖️ Legal and insolvency practitioners
- 🛡️ Compliance, risk, and due diligence teams
- 🏦 Financial institutions screening French counterparties
- 📊 Corporate intelligence and market research analysts
- 🕵️ Investigative journalists and data journalists
- 🧑‍💻 Data engineers building monitoring pipelines

---

## 📥 Input Schema

The actor accepts the following input parameters:

```json
{
  "title": "Input schema for Bodacc French Legal Gazette Scraper",
  "description": "This schema defines the input for the Bodacc French Legal Gazette Scraper.",
  "type": "object",
  "schemaVersion": 1,
  "properties": {
    "startUrls": {
      "title": "Start URLs",
      "type": "array",
      "description": "URLs to scrape",
      "editor": "requestListSources",
      "prefill": [
        {
          "url": "https://www.bodacc.fr/pages/annonces-commerciales/?disjunctive.typeavis&disjunctive.familleavis&disjunctive.publicationavis&disjunctive.region_min&disjunctive.nom_dep_min&disjunctive.numerodepartement&sort=dateparution#resultarea"
        }
      ]
    },
    "maxItems": {
      "title": "Max items",
      "type": "integer",
      "description": "The maximum number of items to fetch",
      "prefill": 20,
      "default": 20
    },
    "proxyConfiguration": {
      "title": "Proxy Configuration",
      "type": "object",
      "description": "Your proxy configuration from Apify",
      "editor": "proxy",
      "default": {
        "useApifyProxy": false
      }
    }
  }
}
```

### Input Parameters

- **startUrls**: Array of Bodacc listing or detail pages to enqueue. Defaults to the commercial announcements search.
- **maxItems**: Maximum number of notices to extract (default: 20).
- **proxyConfiguration** (optional): Apify proxy settings when routing traffic through residential or datacenter pools.

### Example Start URLs

You can provide different types of URLs to target the notices you need:

**1. Commercial announcements listing** (scrapes the newest nationwide notices):

```
https://www.bodacc.fr/pages/annonces-commerciales/?sort=dateparution#resultarea
```

**2. Filtered search results** (scrapes by department, notice family, or publication type):

```
https://www.bodacc.fr/pages/annonces-commerciales/?numerodepartement=75&familleavis=creation&sort=dateparution#resultarea
```

**3. Specific notice detail page** (scrapes a single announcement record):

```
https://www.bodacc.fr/pages/annonces-commerciales-detail/?q.id=id:A202502145
```

You can mix and match listing, filtered, and detail URLs in the `startUrls` array to collect the exact notices required.

---

## 📤 Output Schema

Each scraped announcement returns the following structured data:

```json
{
  "datasetId": "annonces-commerciales",
  "recordId": "4fa94a945ad52d2ce9cf6e6d58521aabc97eb7c3",
  "establishments": {
    "etablissement": {
      "origineFonds": "Création",
      "qualiteEtablissement": "Etablissement principal",
      "activite": "Commercialisation, promotion et vente de produits cosmétiques et de soins corporels. - Effectuer des prestations sur différentes Plateformes de mise en relations entre entreprises et micro entrepreneurs",
      "enseigne": "NUZA",
      "adresse": {
        "numeroVoie": "21B",
        "typeVoie": "avenue",
        "nomVoie": "de Paris",
        "codePostal": "02400",
        "ville": "Château-Thierry"
      }
    }
  },
  "persons": {
    "personne": {
      "typePersonne": "pp",
      "numeroImmatriculation": {
        "numeroIdentification": "984 487 074",
        "codeRCS": "RCS",
        "nomGreffeImmat": "Soissons"
      },
      "nom": "ISMI",
      "prenom": "Nurcan",
      "nomCommercial": "NUZA"
    }
  },
  "url": "https://www.bodacc.fr/pages/annonces-commerciales-detail/?q.id=id:A202502145",
  "publicationType": "A",
  "id": "A202502145",
  "postalCode": "02400",
  "register": "984487074,984 487 074",
  "isPdfUnit": "oui",
  "court": "Greffe du Tribunal de Commerce de Soissons",
  "act": {
    "dateImmatriculation": "2025-10-28",
    "dateCommencementActivite": "2025-10-21",
    "creation": {
      "categorieCreation": "Immatriculation d'une personne physique suite à création d'un établissement principal"
    }
  },
  "city": "Château-Thierry",
  "publicationDate": "2025-11-06",
  "merchant": "ISMI, Nurcan",
  "pdfSubfolder": 0,
  "regionCode": 32,
  "announcementNumber": 5,
  "noticeType": "annonce",
  "edition": "20250214",
  "noticeFamily": "creation",
  "noticeTypeLabel": "Avis initial",
  "departmentNumber": "02",
  "noticeFamilyLabel": "Créations",
  "officialRegionName": "Hauts-de-France",
  "officialDepartmentName": "Aisne",
  "recordTimestamp": "2025-11-06T05:00:00Z"
}
```

### Output Fields

- **datasetId**: Name of the Bodacc collection the notice originated from.
- **recordId**: Unique identifier for the record in the dataset.
- **establishments.etablissement**: Establishment-level details such as activity, trade name, and address.
- **persons.personne**: Parties involved, registration identifiers, and legal form.
- **url**: Direct link to the Bodacc detail page for verification.
- **publicationType**: Official Bodacc series (`A`, `B`, or `C`).
- **id**: Notice identifier shown on Bodacc.
- **register**: Company registration numbers and formatting variants.
- **isPdfUnit**: Flag indicating if a PDF notice is provided.
- **court**: Commercial court or registry responsible for the filing.
- **act**: Nested fields describing the legal act, dates, and categories.
- **publicationDate**: Official Bodacc publication date.
- **merchant**: Primary merchant or company name associated with the notice.
- **location fields**: `postalCode`, `city`, `officialRegionName`, `officialDepartmentName`, `regionCode`, `departmentNumber`.
- **notice metadata**: `noticeType`, `noticeTypeLabel`, `noticeFamily`, `noticeFamilyLabel`, `edition`, `announcementNumber`.
- **recordTimestamp**: UTC timestamp recorded during scraping.

---

## Need to monitor more French records?

Exploring additional public datasets from France? Check out more Apify actors from our team:

**[Lexis Solutions on Apify](https://apify.com/lexis-solutions)** - Discover scrapers for procurement, corporate filings, and government open data feeds to complement your Bodacc pipeline.

---

👀 p.s.

Got feedback or need an extension?

Lexis Solutions is a certified Apify Partner. We can help you with custom solutions or data extraction projects.

Contact us over [Email](mailto:scraping@lexis.solutions) or [LinkedIn](https://www.linkedin.com/company/lexis-solutions)

## Support Our Work 💝

If you're happy with our work and scrapers, you're welcome to leave us a company review and leave a review for the scrapers you're subscribed to. It will take you less than a minute but it will mean a lot to us!
