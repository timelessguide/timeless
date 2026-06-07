---
layout: default
title: Templates and Tools for End-of-Life Planning
subtitle: Templates to put everything important in one place.
hero_text: Structured templates for end-of-life planning, paperwork, and personal records.
hero_image: assets/images/use-hero.png
color_theme: theme-use
description: Structured templates and tools for end-of-life planning. Organize your wishes, documents, and personal records in one place.

products:
  - title: "Core Planning Kit"
    price: "$39"
    description: "The foundational guide for organizing your wishes, documents, and important details in one place."
    best_for: "anyone who wants a clear starting point."
    image: assets/images/core-kit.png
    link: "https://etsy.com/your-listing-1"
    button_text: "View details"

  - title: "Additional Guides"
    price: "$10 - $25"
    description: "Optional guides with structured templates for specific life situations and family structures."
    best_for: "people navigating different realities — including caregiving, chosen family, living abroad, business ownership, or identity-specific considerations."
    image: assets/images/addon-kit.png
    link: "https://etsy.com/your-listing-2"
    button_text: "Browse guides"

  - title: "All Planning Resources"
    price: ""
    description: "The full Timeless Tributes collection on Etsy."
    best_for: ""
    image: assets/images/all-guides.png
    link: "https://etsy.com/your-shop"
    button_text: "Visit the shop"
---

<section class="use-hero">
    <h1>{{ page.title }}</h1>
    <p class="use-main-title">{{ page.subtitle }}</p>
    <p class="use-hero-text">{{ page.hero_text }}</p>
    <div class="use-hero-image">
        <img src="{{ page.hero_image | relative_url }}" alt="">
    </div>
</section>

<div class="etsy-nudge">
    <p>These guides are <strong>hosted on Etsy</strong> for secure checkout and file delivery.<br/>These guides are designed to be completed in sections - start wherever makes sense for your situation.</p>
</div>

<div class="product-grid">
    {% for item in page.products %}
    <div class="product-card {% if forloop.last %}alt-card{% endif %}">
        <div class="product-image">
            <img src="{{ item.image | relative_url }}" alt="{{ item.title }}">
        </div>
        <div class="product-info">
            <h3>{{ item.title }}</h3>
            {% if item.price != "" %}<span class="price">{{ item.price }}</span>{% endif %}
            
            <p class="description">{{ item.description }}</p>
            
            {% if item.best_for != "" %}
            <p class="best-for"><strong>Helpful for:</strong> {{ item.best_for }}</p>
            {% endif %}
            
            <a href="{{ item.link }}" target="_blank" class="btn-product">
                {{ item.button_text }} →
            </a>
            
            
        </div>
    </div>
    {% endfor %}
</div>

<div class="support-box">
    <p>The Core Planning Kit covers what most lives have in common. Additional Guides exist for situations that need more specific care.</p>
</div>
