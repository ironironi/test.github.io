# Testing features

# A collapsible section with markdown
<details>
  <summary>Click to expand!</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

________________

external link that opens in same tab, nie dobje: [a test link](https://hebrewlion.com)

external link that opens in a new tab: <a href="http://hebrewlion.com" target="_blank">this is descriptive text</a>

Reminder: Both the <summary> and </details> tags need a blank line afterward, or Github may not cooperate.

---------------

This first cat has alt text and title, but cannot be resized
![Alt text describing image](https://1000logos.net/wp-content/uploads/2021/05/GitHub-logo.png "How do you like this image? This is additional info, beyond alt text")

Now, this is the same cat resized, but using different code. I am not sure it be alt texted, etc.
<img src="https://1000logos.net/wp-content/uploads/2021/05/GitHub-logo.png" width="100">

Further info and options at https://www.xaprb.com/blog/how-to-style-images-with-markdown/

---------------

Reusables
Reusables are long strings of reusable text.

Reusables are longer strings like paragraphs or procedural lists that can be referenced in multiple content files. Using Markdown (instead of YAML) makes it possible for our localization pipeline to split the strings into smaller translatable segments, leading to fewer translation errors and less churn when the source English content changes.

Each reusable lives in its own Markdown file.

The path and filename of each Markdown file determines what its path will be in the data object.

For example, a file named /data/reusables/foo/bar.md will be accessible as {% data reusables.foo.bar %} in pages.

Reusable files are divided generally into directories by task. For example, if you're creating a reusable string for articles about GitHub notifications, you'd add it in the directory data/reusables/notifications/ in a file named data/reusables/notifications/your-reusable-name.md. The content reference you'd add to the source would look like {% data reusables.notifications.your-reusable-name %}.

Now, let's prove it. Here's the code for a reusable: {% assets/reusable-lion.md %}
