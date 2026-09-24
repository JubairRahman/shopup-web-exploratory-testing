#  BUG-003 — Homepage "Latest Blog" Does Not Show the Latest Published Post

![Severity](https://img.shields.io/badge/Severity-Medium-orange)
![Priority](https://img.shields.io/badge/Priority-Medium-yellow)
![Type](https://img.shields.io/badge/Type-Content%20%2F%20CMS-blue)

---

##  Locations

**Homepage:**  
https://www.shopup.org/

**Blog:**  
https://www.shopup.org/blog

---

##  Steps to Reproduce

### Step 1 — Check the Homepage

1. Open https://www.shopup.org/
2. Scroll down to the **Latest blog** section.
3. Observe the displayed blog posts and their publication dates.

The homepage currently displays:

- **ShopUp’s Mokam normalizing women-run groceries in Bangladesh**  
  *8 June, 2021*

- **ShopUp transforming the retail scene in Bangladesh**  
  *8 June, 2021*

---

### Step 2 — Check the Blog Page

1. Open https://www.shopup.org/blog
2. Review the published blog posts.
3. Compare the publication dates with the posts displayed in the homepage's **Latest blog** section.

The Blog page contains:

- **ShopUp’s Mokam normalizing women-run groceries in Bangladesh** — 8 June, 2021
- **ShopUp transforming the retail scene in Bangladesh** — 8 June, 2021
- **Working Capital Gap in FMCG Retail Supply Chain** — **31 August, 2021**

---

##  Actual Result

The homepage section is labelled **"Latest blog"**, but it only displays posts published on **8 June, 2021**.

The latest post available on the Blog page is:

> **Working Capital Gap in FMCG Retail Supply Chain**  
> **31 August, 2021**

However, this post is not displayed in the homepage's **Latest blog** section.

---

##  Expected Result

The **Latest blog** section should display the most recently published blog post.

Therefore, the homepage should include:

> **Working Capital Gap in FMCG Retail Supply Chain**  
> 31 August, 2021

If the homepage intentionally displays selected/featured articles rather than the latest posts, the section title should be changed from **"Latest blog"** to something more appropriate, such as **"Featured blog"**.

---

##  Impact

- Users may assume the homepage is showing the latest ShopUp blog content.
- Users may miss newer published content.
- The homepage content may appear outdated.
- It may indicate that the homepage blog section is not synchronized with the main Blog/CMS content.

---

##  Evidence

### Screenshot 1 — Homepage

**File:** `BUG-003-homepage-latest-blog.png`

Capture the **Latest blog** section showing the two June 8, 2021 posts.

### Screenshot 2 — Blog Page

**File:** `BUG-003-blog-page-latest-post.png`

Capture the Blog page showing:

> **Working Capital Gap in FMCG Retail Supply Chain**  
> **31 August, 2021**

---

## 🔗 References

- [ShopUp Homepage](https://www.shopup.org/)
- [ShopUp Blog](https://www.shopup.org/blog)

---

### 📝 QA Note

This finding is based on comparing the content displayed in the homepage's **Latest blog** section with the published content available on the ShopUp Blog page.
