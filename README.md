# 🔎 ShopUp Web — Exploratory QA Testing

![Testing](https://img.shields.io/badge/Testing-Exploratory%20QA-blue)
![Testing Type](https://img.shields.io/badge/Testing%20Type-Manual-orange)
![Platform](https://img.shields.io/badge/Platform-Web-green)
![Browser](https://img.shields.io/badge/Browser-Firefox-orange)
![OS](https://img.shields.io/badge/OS-macOS-lightgrey)
![Environment](https://img.shields.io/badge/Environment-Production-red)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

## 📌 Project Overview

This repository contains an independent exploratory QA review of the **ShopUp public website**, focusing on identifying reproducible user-facing issues across UI, content, accessibility, and cross-page consistency.

The objective is to document findings in a structured and professional QA format, including:

- Clear reproduction steps
- Actual vs. expected results
- Severity and priority
- User impact
- Supporting evidence
- Relevant URLs
- QA observations

---

## 🌐 Website Under Test

**ShopUp:**  
https://www.shopup.org/

**Environment:** Production

---

## 🎯 Testing Objective

The primary objectives of this testing exercise are to:

- Explore the public-facing ShopUp website.
- Identify functional and non-functional issues.
- Verify consistency of content across pages.
- Review UI and content presentation.
- Identify basic accessibility concerns.
- Validate links, navigation, and page-level information.
- Document reproducible findings using standard QA practices.

---

## 🧪 Testing Scope

The exploratory review covers the following areas:

- Homepage
- Testimonials
- Career section
- Job postings
- Blog section
- Navigation
- Content consistency
- Cross-page information consistency
- Basic accessibility
- Image alternative text
- UI/content presentation
- Domain consistency

---

## 🛠️ Test Environment

| Item | Details |
|---|---|
| Website | https://www.shopup.org/ |
| Environment | Production |
| Operating System | macOS |
| Browser | Mozilla Firefox |
| Testing Type | Exploratory / Manual |
| Primary Focus | UI, Content, Accessibility, Consistency |
| Test Period | September 2026 |

---

## 🐛 Findings

| ID | Finding | Severity | Type | Status |
|---|---|---|---|---|
| [BUG-001](bug-reports/BUG-001-testimonial-image-mismatch.md) | Testimonial image does not match testimonial attribution | Medium | Content / UI | Open |
| [BUG-002](bug-reports/BUG-002-career-domain-content.md) | Career content differs between domain variants | Medium* | Content Consistency | Open |
| [BUG-003](bug-reports/BUG-003-latest-blog-content.md) | Homepage "Latest blog" does not show the latest published post | Medium | Content / CMS | Open |
| [BUG-004](bug-reports/BUG-004-duplicate-qualification.md) | Qualification information is duplicated in Internal Audit job posting | Low–Medium | Content / CMS | Open |
| [BUG-005](bug-reports/BUG-005-image-alt-text.md) | Generic or missing image alternative text | Medium* | Accessibility | Open |

> **Note:** BUG-002 requires verification against the intended canonical domain before being classified as a confirmed production defect.
>
> **Note:** BUG-005 should be confirmed using browser/DOM inspection and supporting evidence before final classification.

---

## 📊 Testing Summary

The testing approach was primarily exploratory and risk-based.

The review focused on areas where content accuracy, consistency, accessibility, and presentation can directly affect the user experience.

### Key areas reviewed

- Homepage content
- Customer testimonials
- Career information
- Job descriptions
- Blog content
- Images and alternative text
- Cross-page consistency
- Domain variants

Detailed findings are documented individually under [`bug-reports/`](bug-reports/).

---

## 📁 Repository Structure

```text
shopup-web-exploratory-testing/
│
├── README.md
│
├── docs/
│   ├── TESTING-SCOPE.md
│   ├── TEST-ENVIRONMENT.md
│   └── TEST-SUMMARY.md
│
├── bug-reports/
│   ├── BUG-001-testimonial-image-mismatch.md
│   ├── BUG-002-career-domain-content.md
│   ├── BUG-003-latest-blog-content.md
│   ├── BUG-004-duplicate-qualification.md
│   └── BUG-005-image-alt-text.md
│
├── evidence/
│   ├── BUG-001/
│   ├── BUG-002/
│   ├── BUG-003/
│   ├── BUG-004/
│   └── BUG-005/
│
└── .gitignore
