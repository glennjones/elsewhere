---
heading: How does it work?
category: overview
---
Whether you use Elsewhere as a server or as part of your own node project, it works by you first providing it with a url.

Elsewhere searches the page at this url for links, marked up with `rel=me`, linking to other pages. It then searches these subsequent pages for more links and so on.

Any link found on any of these subsequent pages that links back to the original url, verifies the page. Any page that links to a verified page is then also marked as verified and so on.

Any pages with these reciprical links to other pages in the graph can be reliably thought of belonging to the owner of the url you initially provided Elsewhere.

Many profile pages do lack `rel=me` markup however and thus the reciprical links cannot be reliably established. As a result many legitimate profiles cannot be reliably marked as verified. When using the server you can choose to include these unverified links or not.

Once Elsewhere has run out of links it returns with a graph representing the owner of your initial url, which you can then do what you like with.