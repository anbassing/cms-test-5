# Visit Locals — CMS Test Deployment

This build keeps the existing frontend design and hard-coded Experience cards intact, while adding a read-only WordPress CMS test on the Home page.

CMS endpoint:
https://cms.visitindonesia.co.id/wp-json/wp/v2/experience?per_page=100

Behavior:
- Fetches published Experience records from WordPress.
- Injects them into the existing Experience grid using the existing `.experience-card` class.
- Existing search, category filtering, Show More, and modal behavior continue to apply.
- If the CMS request fails, existing hard-coded cards remain available.
- This does not replace production content.
