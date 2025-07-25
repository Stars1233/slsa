---
title: SLSA specification
description: SLSA is a specification for describing and incrementally improving supply chain security, established by industry consensus. It is organized into a series of levels that describe increasing security guarantees.
---

SLSA is a specification for describing and incrementally improving supply chain
security, established by industry consensus. It is organized into a series of
levels that describe increasing security guarantees.

This is **Version 1.2 Release Candidate 1 (RC1)** of the SLSA
specification, which defines several SLSA levels and recommended attestation
formats, including provenance.

{%- for section in site.data.nav.main %}
{%- if section.url == page.url %}
{%- for subsection in section.children %}
{%- if subsection.children %}

## {{ subsection.title }}

{{ subsection.description }}

<!-- markdownlint-capture -->
<!-- markdownlint-disable MD055 MD056 -->
| Page | Description
| ---- | -----------
{%- for child in subsection.children %}
| [{{child.title}}]({{child.url | relative_url}}) | {{child.description}}
{%- endfor %}
<!-- markdownlint-restore -->

{%- endif %}
{%- endfor %}
{%- endif %}
{%- endfor %}
