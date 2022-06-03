# GITHUB TEST
This is a repository to test my understanding of git and **Git Hub**

***
This is an experimental MD file.

I get all my images from [Unsplash](https://unsplash.com/)

Please leave a thumbs up 🤗  if you like my repo and let's make great contributions this year :shipit:

Don't make me do this 👾

More emojis:😠⏰

And here are some of the presidents of the US:

- George Washington
- John Adams
- Thomas Jefferson
  - Hey Lab
    - Meyer

![cute kitty](https://static.boredpanda.com/blog/wp-content/uploads/2016/08/cute-kittens-4-57b30a939dff5__605.jpg)

## More Markdown Tests

Here's a quote:

>"Follow the golden rule!"

And here is a sample `code`.

And a longer code example:

```
git status
git add
git commit
```

And highligted Ruby code:
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

And an example of highlighted JS code:

```js
const $ = require("cheerio");
const request = require("request");

/**
 * @typedef {string} EmojiLiteral
 * @returns {Promise<{ [githubEmojiId: string]: EmojiLiteral | [string] }>}
 */
async function getGithubEmojiIdMap() {
  return Object.fromEntries(
    Object.entries(
      /** @type {{ [id: string]: string }} */ (await fetchJson(
        "https://api.github.com/emojis",
        {
          headers: {
            "User-Agent": "https://github.com/ikatyang/emoji-cheat-sheet"
          }
        }
      ))
    ).map(([id, url]) => [
      id,
      url.includes("/unicode/")
        ? getLast(url.split("/"))
            .split(".png")[0]
            .split("-")
            .map(codePointText =>
              String.fromCodePoint(Number.parseInt(codePointText, 16))
            )
            .join("")
        : [getLast(url.split("/")).split(".png")[0]] // github's custom emoji
    ])
  );
}

async function getUnicodeEmojiCategoryIterator() {
  return getUnicodeEmojiCategoryIteratorFromHtmlText(
    await fetch("https://unicode.org/emoji/charts/full-emoji-list.html")
  );
}
```

And here are some of the task lists:

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

## So let's get ready yo!

![transformer](https://tfwiki.net/mediawiki/images2/thumb/3/37/Optimusg1.jpg/350px-Optimusg1.jpg)