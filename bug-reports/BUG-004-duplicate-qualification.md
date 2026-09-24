#  BUG-004 — Duplicate Qualification Information in Internal Audit Job Posting

![Severity](https://img.shields.io/badge/Severity-Low--Medium-yellow)
![Priority](https://img.shields.io/badge/Priority-Low--Medium-yellow)
![Type](https://img.shields.io/badge/Type-Content%20%2F%20CMS-blue)

---

##  Location

**Job Posting:**  
https://shopup.org/job-postings/manager-senior-manager-internal-audit-2

**Section:**  
Qualification and Experience

---

## 🔎 Steps to Reproduce

1. Open the Internal Audit job posting.
2. Scroll to the **Qualification and Experience** section.
3. Review the listed qualifications and experience requirements.
4. Continue down to **Additional Information**.
5. Locate **Qualifications and Experience Required**.
6. Compare the requirements with the earlier section.

---

##  Actual Result

Qualification and experience requirements are repeated in multiple sections of the same job posting.

There is also a formatting issue in the following text:

> `...COSO).Exceptional written and verbal communication...`

There is no space between the two sentences.

---

##  Expected Result

- Qualification and experience requirements should be presented once without unnecessary duplication.
- The **Additional Information** section should contain only additional relevant information.
- A space should be added after the period:

> `...COSO). Exceptional written and verbal communication...`

---

##  Impact

- Makes the job description unnecessarily long.
- Reduces readability for applicants.
- May make the content appear incorrectly formatted or duplicated.
- Could cause applicants to interpret repeated information as separate requirements.

---

## 📸 Evidence

### Duplicate Qualification Information

![BUG-004 — Duplicate Qualification](https://github.com/user-attachments/assets/5e54657d-ce4a-46f6-b848-858571322f2e)

*The same qualification and experience information is repeated within the job posting.*

---

## 🔗 Reference

https://shopup.org/job-postings/manager-senior-manager-internal-audit-2

---

### 📝 QA Note

The issue appears to be related to duplicated job-posting content and minor text formatting.
