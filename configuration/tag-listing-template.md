---
Type: Template
Title: Tag Listing Template
---

// Note: tag listing order can be "alphabetical", "ascending", or "descending" where alphabetical sorts by the tag name and ascending/descending sorts by the count of entries with that tag
Tag listing order: ascending
Tag listing format: <<[
<h2>TAGS</h2>
<ul>
[tag:begin]<li><a href="$location">$tag</a> ($count)</li>[tag:end]
</ul>
]>>
