---
Type: Page
Title: Archive
Location: /archive
---

# Archive

<article>
        <h1><i class="fa-solid fa-archive"></i> {post-title}</h1>
        {post-list}
    </article>
    <hr>
    <div class="weblog-info">
        <div class="container background-orange">
            <h2><i class="fa-solid fa-clock"></i> Recent posts</h2>
            {recent-posts}
        </div>
            <h2><i class="fa-solid fa-fw fa-magnifying-glass"></i> Search</h2>
            <form class="weblog-search" action="?" method="get">
                <input placeholder="What are you looking for?" type="text" name="search">
                <div class="weblog-search--submit-wrap">
                    <button type="submit">Let's take a look!</button>
                </div>
            </form>
        </div>
    </div>
