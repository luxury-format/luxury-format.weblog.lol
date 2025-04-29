Type: Template
Title: Tag Listing Template
Location: /configuration/tag-listing-template.md

// Note: tag listing order can be "alphabetical", "ascending", or "descending" where alphabetical sorts by the tag name and ascending/descending sorts by the count of entries with that tag
Tag listing order: alphabetical
Tag listing format: <<[
<h2>Tags</h2>
<ul>
[tag:begin]<li><a href="$location">$tag</a> ($count)</li>[tag:end]
</ul>
]>>
