# 🔎 ShopUp Web — Exploratory QA Testing

![Testing](https://img.shields.io/badge/Testing-Exploratory-blue)
![Platform](https://img.shields.io/badge/Platform-Web-orange)
![Browser](https://img.shields.io/badge/Browser-Firefox-lightgrey)
![OS](https://img.shields.io/badge/OS-macOS-black)
![Environment](https://img.shields.io/badge/Environment-Production-success)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

> Exploratory QA testing of the ShopUp public website, focusing on user-facing defects, content consistency, accessibility, and cross-page behavior.

---

## 🌐 Website

**ShopUp:**  
https://www.shopup.org/

---

## 🎯 Objective

This repository documents a lightweight exploratory QA review of the ShopUp public website.

The goal is to identify and document reproducible issues from a real user's perspective, with clear:

- Reproduction steps
- Expected results
- Actual results
- Impact
- Severity / priority
- Supporting screenshots

This is an independent QA testing exercise and is not an official ShopUp QA report.

---

## 🧪 Testing Information

| Item | Details |
|---|---|
| **Website** | https://www.shopup.org/ |
| **Environment** | Production |
| **OS** | macOS |
| **Browser** | Mozilla Firefox |
| **Testing Type** | Exploratory / Manual |
| **Focus** | UI, Content, Accessibility, Consistency |
| **Test Date** | September 2026 |

---

## 🔍 Testing Areas

The exploratory review currently covers:

- Homepage
- Customer testimonials
- Careers
- Job postings
- Blog
- Navigation
- Content consistency
- Basic accessibility
- HTML / DOM inspection
- Cross-domain consistency

---

## 🐛 Findings

| ID | Finding | Severity | Area | Status |
|---|---|---|---|---|
| [BUG-001](bug-reports/BUG-001-testimonial-image-mismatch.md) | Testimonial image does not match attribution | 🟠 Medium | Content / UI | Open |
| [BUG-002](bug-reports/BUG-002-career-domain-content.md) | Career content differs between domain variants | 🟠 Medium* | Consistency | Open |
| [BUG-003](bug-reports/BUG-003-latest-blog-content.md) | "Latest blog" does not show the latest published post | 🟠 Medium | CMS / Content | Open |
| [BUG-004](bug-reports/BUG-004-duplicate-qualification.md) | Qualification information is duplicated | 🟡 Low–Medium | CMS / Content | Open |
| [BUG-005](bug-reports/BUG-005-image-alt-text.md) | Generic / missing image alternative text | 🟠 Medium | Accessibility | Open |

> **Note:** BUG-002 requires verification of the intended canonical domain configuration before being treated as a confirmed defect.

---

## 📊 Testing Summary

### Findings by Area

| Area | Findings |
|---|---:|
| Content / UI | 1 |
| Domain / Consistency | 1 |
| CMS / Content | 2 |
| Accessibility | 1 |
| **Total** | **5** |

---

## 📸 Evidence

Each finding contains supporting screenshots where applicable.

Evidence is organized by bug ID:

```text
evidence/
├── BUG-001/
├── BUG-002/
├── BUG-003/
├── BUG-004/
└── BUG-005/
