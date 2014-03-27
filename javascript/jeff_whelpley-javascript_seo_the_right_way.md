# Javascript SEO the right way

Jeff Whelpley, @jeffwhelpley, GetHuman.com

1. Inbound links: quality links from recognized sites
2. No pogosticking: Search engine users don't jump right back to search results.
3. Performance: 400 ms initial page load ideal.
4. Social proof: Users talk about your page or site.
5. On Page SEO: Content.

The problem: single page app has no content til the client renders and asks for it.

Bad solutions:

* Google Escaped Fragment Specification - gethuman.com said no. Ugly URLs are less likely to be clicked. Fragment Spec SPAs are a tiny minority of sites.
* Cloaking - Showing the search engine something different than the client sees.
* Headless browsers - Get snapshots of the pages as rendered, send them to search engines. This option sucks.

Good solution:

* Server pre-rendering

Initial page load, the server is serving a fully rendered view.


