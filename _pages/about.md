---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a bioinformatician with a background in molecular biology and genetics, specialized in computational biology. Since 2018, I have been a CNRS researcher, focusing on tumor heterogeneity through the integration of experimental and computational approaches. My research spans both the development of novel methodological frameworks and the study of cancer biology. 

In 2025, I joined the [LIG](https://www.liglab.fr/fr) to establish a bioinformatics group within the [APTIKAL](https://lig-aptikal.imag.fr/) team : [Bioinfo@APTIKAL](https://bioinfo-lig.github.io/)

I am involved in the network BiGre (Computational Biology in Grenoble)

I am also actively engaged in promoting collaborative science by organizing data challenges


Research projects 
======


**On going projects:**

<!-- Project cards: generate automatically from pages whose permalink contains "/projects/" -->
<style>
.project-card-top{
  display:flex;
  flex-direction:column;
  gap:0.75rem;
  align-items:flex-start;
  margin:1rem 0 1.5rem;
  padding:14px;
  border:1px solid #e6e6e6;
  border-radius:8px;
  background:#fff;
  box-shadow:0 4px 10px rgba(0,0,0,0.03);
}
.project-card-top img{
  width:100%;
  max-width:920px;
  height:auto;
  border-radius:6px;
  object-fit:cover;
  box-shadow:0 6px 18px rgba(0,0,0,0.06);
}
.project-card-top .meta{ width:100%; }
.project-card-top h3{ margin:0 0 6px; font-size:1.05rem; }
.project-card-top p{ margin:0 0 8px; color:#444; }
.project-card-top .summary{ color:#666; font-size:0.95rem; line-height:1.5; }
.project-card-top .actions{ margin-top:10px; }
@media(min-width:960px){
  .project-card-top{ max-width:920px; }
}
</style>

{%- for p in site.pages -%}
  {%- if p.permalink and p.permalink contains '/projects/' -%}
    <div class="project-card-top">
      {%- if p.image -%}
        <img src="{{ p.image }}" alt="{{ p.title | escape }}" />
      {%- endif -%}
      <div class="meta">
        <h3>{{ p.title }}</h3>
         {%- if p.subtitle -%}
          <p style="margin:4px 0 8px;color:#666;font-style:italic;">{{ p.subtitle }}</p>
        {%- endif -%}
        <p>
          {%- if p.coordinator -%}<strong>Coordinator:</strong> {{ p.coordinator }}{%- elsif p.authors -%}<strong>Coordinator:</strong> {{ p.authors }}{%- endif -%}
          {%- if p.agency -%} &nbsp; • &nbsp; <strong>Funding:</strong> {{ p.agency }}{%- endif -%}
        </p>
         {%- if p.partners -%}
        <p><strong>Partners:</strong> {{ p.partners }}</p>
        {%- endif -%}
        {%- if p.period -%}
        <p><strong>Period:</strong> {{ p.period }}</p>
        {%- endif -%}
        <p class="summary">
          {%- if p.excerpt -%}
            {{ p.excerpt | strip_html }}
          {%- elsif p.summary -%}
            {{ p.summary | strip_html }}
          {%- else -%}
            {{ p.content | strip_html | truncate: 280 }}
          {%- endif -%}
        </p>
              <p class="actions">
        {%- if p.external_url -%}
          <a href="{{ p.permalink }}" style="display:inline-block;padding:8px 12px;background:#0b6cff;color:#fff;border-radius:5px;text-decoration:none;font-weight:600;">Project page</a>
          <a href="{{ p.external_url }}" target="_blank" rel="noopener" style="display:inline-block;margin-left:8px;padding:8px 12px;border-radius:5px;border:1px solid:#ddd;text-decoration:none;color:#0b6cff;background:#fff;font-weight:600;">External link</a>
        {%- elsif p.url -%}
          <a href="{{ p.permalink }}" style="display:inline-block;padding:8px 12px;background:#0b6cff;color:#fff;border-radius:5px;text-decoration:none;font-weight:600;">Project page</a>
          <a href="{{ p.url }}" target="_blank" rel="noopener" style="display:inline-block;margin-left:8px;padding:8px 12px;border-radius:5px;border:1px solid:#ddd;text-decoration:none;color:#0b6cff;background:#fff;font-weight:600;">External link</a>
        {%- elsif p.paperurl -%}
          <a href="{{ p.permalink }}" style="display:inline-block;padding:8px 12px;background:#0b6cff;color:#fff;border-radius:5px;text-decoration:none;font-weight:600;">Project page</a>
          <a href="{{ p.paperurl }}" target="_blank" rel="noopener" style="display:inline-block;margin-left:8px;padding:8px 12px;border-radius:5px;border:1px solid:#ddd;text-decoration:none;color:#0b6cff;background:#fff;font-weight:600;">External link</a>
        {%- else -%}
          <a href="{{ p.permalink }}" style="display:inline-block;padding:8px 12px;background:#0b6cff;color:#fff;border-radius:5px;text-decoration:none;font-weight:600;">Project page</a>
        {%- endif -%}
      </p>
      </div>
    </div>
  {%- endif -%}
{%- endfor -%}



**Past projects:**

- **ACACIA** 2021-2025 ITMO Cancer AVIESAN
- **THEMA** 2022-2015 IRS-IDEX UGA
- **ARTICAH** 2021 UGA MIAI
- **COMETH** 2019 EIT Health
- **HADACA** 2018 EIT Health
- **LuCaH** 2019 IRS-IDEX UGA
- **Epi-Cancer** 2018 PEPS - CNRS INS2I

