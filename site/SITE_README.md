Aaria Dynamics — Static site scaffold

This small scaffold demonstrates the sitemap, product template, a sample product, and portal stubs described in the project brief.

How to view locally:
- Open `site/index.html` in a browser (static files). For a simple local server (recommended), run a static file server in the `site` folder, e.g., Python 3:

  python -m http.server 8000

  Then open http://localhost:8000

What is included:
- Top-level sitemap structure (pages under `/about`, `/solutions`, `/products`, `/portal`, `/contact`, `/compliance`).
- Canonical product template at `/products/aircraft/lf-13-long-fighter` with JSON-LD and datasheet CSV for ingestion.
- Portal stubs (`/portal/*`) describing gated sections.
- robots.txt and sitemap.xml (basic).

Notes and next steps:
- This is a static prototype. For full implementation use a headless CMS (Strapi/Contentful), a relational DB for products, search (Elasticsearch), secure portal with SSO, and gated content as described in the specification.
- Implement authentication, PKI/SAML/OIDC, 2FA, and network segregation for portal production.
