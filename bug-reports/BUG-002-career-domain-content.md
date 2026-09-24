#  BUG-002 — Career Content Differs Between `www` and Non-`www` Domains

![Severity](https://img.shields.io/badge/Severity-Medium-orange)
![Priority](https://img.shields.io/badge/Priority-Medium-yellow)
![Type](https://img.shields.io/badge/Type-Content%20Consistency-blue)

###  URLs

**www version**

https://www.shopup.org/career

**non-www version**

https://shopup.org/career

### 🔎 Steps to Reproduce

1. Open:

   `https://www.shopup.org/career`

2. Note the available positions.

3. Open:

   `https://shopup.org/career`

4. Compare the job listings.

###  Actual Result

The two domain variants do not display the same career content.

The current `www` version lists:

- ShopUp Fast Track (Tech)
- QA Engineer

The non-www version has different/older career content.

###  Expected Result

Both domain variants should resolve to the same canonical website and display the same current career information.

###  Impact

Users accessing the website through different domain variants may receive different information.

For a recruitment page, this could potentially result in users seeing outdated or inconsistent job opportunities.

### ⚠️ Note

This finding should be verified against ShopUp's intended canonical-domain configuration before being treated as a confirmed production defect.

### 📸 Evidence

Capture both pages side-by-side:

```text
┌─────────────────────────────┬─────────────────────────────┐
│ www.shopup.org/career       │ shopup.org/career           │
│                             │                             │
│ Current job listings        │ Different/older listings    │
│                             │                             │
└─────────────────────────────┴─────────────────────────────┘
```
