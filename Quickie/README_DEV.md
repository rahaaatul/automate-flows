# Dev Notes

- [Dev Notes](#dev-notes)
  - [Websites](#websites)
    - [Notes](#notes)
  - [Process Data](#process-data)
    - [Notes](#notes-1)
  - [Usage](#usage)
    - [Notes](#notes-2)

## Websites

List of supported websites

```json
{
  "@airbnb ": "https://www.airbnb.com/s/all?query=",
  "@aliexpress ": "https://www.aliexpress.com/wholesale?SearchText=",
  "@amazon ": "https://www.amazon.com/s?k=",
  "@anilist_anime ": "https://anilist.co/search/anime?search=",
  "@anilist_character ": "https://anilist.co/search/characters?search=",
  "@anilist_manga ": "https://anilist.co/search/manga?search=",
  "@anilist_staff ": "https://anilist.co/search/staff?search=",
  "@aol ": "https://search.aol.com/aol/search?q=",
  "@archive ": "https://archive.org/search?query=",
  "@ask ": "https://www.ask.com/web?q=",
  "@azlyrics ": "https://search.azlyrics.com/search.php?x=b7ad4ff857e7b59f99f0d0f5b3c7d2e292ea2446137b3009b6f2636b0d76aba6&q=",
  "@baidu ": "https://www.baidu.com/s?wd=",
  "@bandcamp ": "https://bandcamp.com/search?q=",
  "@bing ": "https://www.bing.com/search?q=",
  "@bitbucket ": "https://bitbucket.org/repo/all?name=",
  "@booking ": "https://www.booking.com/searchresults.html?ss=",
  "@codepen ": "https://codepen.io/search/pens?q=",
  "@conservapedia ": "https://www.conservapedia.com/index.php?search=",
  "@crunchbase ": "https://www.crunchbase.com/search?q=",
  "@dailymotion ": "https://www.dailymotion.com/search/",
  "@deviantart ": "https://www.deviantart.com/search?q=",
  "@dribbble ": "https://dribbble.com/search?q=",
  "@duckduckgo ": "https://duckduckgo.com/?q=",
  "@dumb ": "https://dumb.ducks.party/search?q=",
  "@ebay ": "https://www.ebay.com/sch/i.html?_nkw=",
  "@ecosia ": "https://www.ecosia.org/search?q=",
  "@etsy ": "https://www.etsy.com/search?q=",
  "@facebook ": "https://www.facebook.com/search/top/?q=",
  "@fandom ": "https://www.fandom.com/?s=",
  "@genius ": "https://genius.com/search?q=",
  "@giphy ": "https://giphy.com/search/",
  "@github ": "https://github.com/search?q=",
  "@goodreads ": "https://www.goodreads.com/search?q=",
  "@google ": "https://www.google.com/search?q=",
  "@imdb ": "https://www.imdb.com/find?q=",
  "@instagram ": "https://www.instagram.com/explore/tags/",
  "@itchio ": "https://itch.io/search?q=",
  "@kickstarter ": "https://www.kickstarter.com/projects/search?term=",
  "@lastfm ": "https://www.last.fm/search?q=",
  "@linkedin ": "https://www.linkedin.com/search/results/all/?keywords=",
  "@mal_anime ": "https://myanimelist.net/anime.php?cat=anime&q=",
  "@mal_character ": "https://myanimelist.net/character.php?cat=character&q=",
  "@mal_company ": "https://myanimelist.net/company?cat=company&q=",
  "@mal_manga ": "https://myanimelist.net/manga.php?cat=manga&q=",
  "@mal_people ": "https://myanimelist.net/people.php?cat=person&q=",
  "@medium ": "https://medium.com/search?q=",
  "@myanimelist ": "https://myanimelist.net/search/all?q=",
  "@myspace ": "https://myspace.com/search?q=",
  "@news ": "https://news.google.com/search?q=",
  "@npm ": "https://www.npmjs.com/search?q=",
  "@patreon ": "https://www.patreon.com/search?q=",
  "@pinterest ": "https://www.pinterest.com/search/pins/?q=",
  "@producthunt ": "https://www.producthunt.com/search?q=",
  "@quora ": "https://www.quora.com/search?q=",
  "@rationalwiki ": "https://rationalwiki.org/w/index.php?search=",
  "@reddit ": "https://www.reddit.com/search/?q=",
  "@searx ": "https://searx.org/search?q=",
  "@searx_paulgo ": "https://paulgo.io/search?q=",
  "@slack ": "https://app.slack.com/client/search/",
  "@snapchat ": "https://story.snapchat.com/search?q=",
  "@soundcloud ": "https://soundcloud.com/search?q=",
  "@spotify ": "https://open.spotify.com/search/results/",
  "@stack ": "https://stackoverflow.com/search?q=",
  "@startpage ": "https://www.startpage.com/do/search?q=",
  "@subreddit ": "https://www.reddit.com/r/",
  "@tiktok_user ": "https://www.tiktok.com/@",
  "@tmdb ": "https://www.themoviedb.org/search?query=",
  "@trakt ": "https://trakt.tv/search?query=",
  "@trakt_episode ": "https://trakt.tv/search/episodes?query=",
  "@trakt_list ": "https://trakt.tv/search/lists?query=",
  "@trakt_people ": "https://trakt.tv/search/people/?query=",
  "@trakt_user ": "https://trakt.tv/search/users/?query=",
  "@trello ": "https://trello.com/search?q=",
  "@tumblr ": "https://www.tumblr.com/search/",
  "@tvdb ": "https://www.thetvdb.com/search?query=",
  "@twitter ": "https://twitter.com/search?q=",
  "@uncyclopedia ": "https://uncyclopedia.com/index.php?search=",
  "@urban_dictionary ": "https://www.urbandictionary.com/define.php?term=",
  "@vimeo ": "https://vimeo.com/search?q=",
  "@vk ": "https://vk.com/search?q=",
  "@waybackmachine ": "https://web.archive.org/web/*/",
  "@whois ": "https://who.is/whois/",
  "@wikia ": "https://www.wikia.org/?s=",
  "@wikibooks ": "https://en.wikibooks.org/w/index.php?search=",
  "@wikihow ": "https://www.wikihow.com/wikiHowTo?search=",
  "@wikinews ": "https://en.wikinews.org/w/index.php?search=",
  "@wikipedia ": "https://en.wikipedia.org/w/index.php?search=",
  "@wikiquote ": "https://en.wikiquote.org/w/index.php?search=",
  "@wikisource ": "https://en.wikisource.org/w/index.php?search=",
  "@wikispecies ": "https://species.wikimedia.org/w/index.php?search=",
  "@wikiversity ": "https://en.wikiversity.org/w/index.php?search=",
  "@wikivoyage ": "https://en.wikivoyage.org/w/index.php?search=",
  "@wiktionary ": "https://en.wiktionary.org/w/index.php?search=",
  "@yahoo ": "https://search.yahoo.com/search?p=",
  "@yandex ": "https://yandex.com/search/?text=",
  "@youtube ": "https://www.youtube.com/results?search_query="
}
```

### Notes

1. The `SEARCH_ENGINE_LIST` variable is a dictionary containing site shortcuts.
2. Each key ends with a space. Why? Because of **_Auto Suggestions_**.
   - When you type `@`, Quickie will display suggestions that can be auto filled when selected.
   - Selecting a suggestion automatically adds an extra space after it, thanks to the hacky solution we structured with the dictionary keys.
   - This is a workaround to ensure smooth autofill functionality. Currently, there’s no better solution—_feel free to correct me if I'm wrong._

---

## Process Data

```json
{
  "custom-engine": "contains(INPUT, \"@* \")",
  "search-engine": "findAll(INPUT, \"(@\\w+)\")[1]",
  "search-query": "replaceAll(INPUT, \"(@\\w+)\\s+\")"
}
```

### Notes

- This dictionary is where 🔍**_Quickie_** processes input and stores the results in the `PROCESSED_DATA` variable.
  - `custom-engine`:
    - Checks if the user is using a shortcut by detecting an `@` symbol in the input.
    - Stores a boolean value: 0 (`false`) or 1 (`true`).
    - Determines if a shortcut or the default search engine should be used.
  - `search-engine`:
    - Identifies which shortcut (e.g., `@google`, `@bing`) is being used.
    - Stores the value of the detected shortcut key.
  - `search-query`:
    - Strips the shortcut key from the input.
    - Makes the search query ready for use with the selected search engine.

---

## Usage

```shell
PROCESSED_DATA["custom-engine"] == 1 ?

SEARCH_ENGINE_LIST[PROCESSED_DATA["search-engine"]] ++ PROCESSED_DATA["search-query"] :

SEARCH_ENGINE_LIST["@google"] ++ PROCESSED_DATA["search-query"]
```

### Notes

1. This is where the core logic is applied.
2. `PROCESSED_DATA["custom-engine"] == 1`
   - Determines if Quickie should use custom search engines.
3. If it's True:

   ```shell
   SEARCH_ENGINE_LIST[PROCESSED_DATA["search-engine"]] ++ PROCESSED_DATA["search-query"]
   ```

   - Retrieves the shortcut URL for the selected search engine (e.g., `https://www.bing.com/search?q=`).
   - Appends the cleaned search query from `PROCESSED_DATA["search-query"]` (e.g., `i'm searching on bing`).
   - The result combines the shortcut and query like this: `https://www.bing.com/search?q=i'm+searching+on+bing`.

4. If it's False:

   ```shell
   SEARCH_ENGINE_LIST["@google"] ++ PROCESSED_DATA["search-query"]
   ```

   - Uses the default search engine URL (e.g., `https://www.google.com/search?q=`).
   - Appends the search query from `PROCESSED_DATA["search-query"]` (e.g., `this is my default search engine`).
   - The result combines the default URL and query like this: `https://www.google.com/search?q=this+is+my+default+search+engine`.
