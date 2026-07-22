# Etsy Market Research Sandbox

A personal data visualization and market analysis tool developed to evaluate product pricing distributions, category hierarchies, and keyword frequencies on the Etsy marketplace. 

This application is built exclusively for personal use and internal research purposes to assist in strategic planning before launching a dedicated Print on Demand storefront.

## Project Purpose & Scope
The goal of this project is to aggregate publicly available marketplace information to make data-driven decisions regarding product positioning, avoiding underpricing, and understanding listing taxonomy.

**Compliance & Privacy Guardrails:**
- **No Third-Party Access:** This tool is strictly for personal research and will not be commercialized as a SaaS or distributed to the general public.
- **No Data Scraping:** The application relies 100% on the official Etsy API v3. It does not use automated web scrapers or bypass Etsy's security.
- **Respect for User Data:** No private user information, buyer data, or proprietary competitor sales figures are tracked, harvested, or stored.

## Core Features
1. **Price Distribution Analysis:** Fetches active listings under specific keywords to calculate the mean and median price points, preventing pricing errors on future listings.
2. **Tag Frequency Counter:** Analyzes public tags used in active listings to identify common keyword combinations and marketplace standards within specific categories.
3. **Taxonomy Mapping:** Visualizes official Etsy category trees to ensure future product catalogs align perfectly with platform standards.

## Technical Architecture & Endpoints
The application is a lightweight dashboard built with Python (Pandas & Streamlit/Dash) that performs read-only requests to the following official Etsy API v3 endpoints:

- `GET /v3/application/listings/active`: To retrieve public price points, titles, and material tags for aggregation.
- `GET /v3/application/taxonomy/seller`: To understand official category nesting.
- `GET /v3/application/shops/{shop_id}`: To read public shop creation years and overall review scores to evaluate market maturity.

## Setup & Implementation Roadmap
- [x] Repository initialization and documentation.
- [ ] UI/UX Wireframing (Mockups for internal dashboard).
- [ ] API Integration (Pending official developer access approval).
- [ ] Local data aggregation and visualization testing.

## License
This project is for personal use only. Redistribution, commercial sale, or deployment as a public service is strictly prohibited.
