---
layout: single
title: "Marketplace Listing & Review Data Pipeline"
permalink: /project/marketplace-data-pipeline/
author_profile: true
sitemap: false
---

{% comment %}
  TEMPORARY PAGE — Etsy Open API application evidence.
  Self-contained: nothing else in the repo links here (no nav entry, no
  listing on /project/ or /portfolio/, excluded from sitemap.xml).
  To remove: delete this single file. Nothing else needs to change.
{% endcomment %}

## Overview

Data collection and processing pipeline for an ongoing academic study of
product attributes and consumer evaluation in online marketplaces.
Engineering and data infrastructure by Hyunjong Jang; the study is a
collaborative research project.

## Etsy Open API usage

Uses the Etsy Open API v3 under a Personal Access key.

**Endpoints**

- `findAllListingsActive` — public listing metadata
- `getReviewsByListing` — public reviews for retrieved listings

**Fields collected**

listing_id, title, description, price, currency, category/taxonomy,
creation date, shop identifier, review text, review rating, review date

**Scope and limits**

- Read-only; no write operations
- Public data only — no shop management, order, receipt, or buyer data
- No personally identifiable information collected or stored
- Requests throttled below the documented rate limit
- Built and operated solely by the author; credentials are not shared

Collected data is used solely for statistical analysis in academic
research and is not redistributed.

## Status

Data collection in progress. Methods and results will be reported in a
forthcoming paper.

## Contact

Hyunjong Jang — hyunjongjang@khu.ac.kr
AIMS Lab, Kyung Hee University
