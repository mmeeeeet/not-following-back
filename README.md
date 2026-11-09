# Not Following Back

Find out who doesn't follow you back on Instagram — **without giving anyone your password.**

🔗 **Use it here: https://mmeeeeet.github.io/not-following-back/**

## Why this exists

Instagram never shows you who doesn't follow you back, and most "unfollower checker" apps ask for your Instagram login. Handing your password to a random app is how accounts get stolen, and automated unfollow bots are how accounts get banned.

This tool takes the safe route: it reads the data export Instagram itself gives every user, and it runs **100% in your browser**. Your files are never uploaded anywhere. No login, no password, no API, no account risk — it never touches your account at all.

## How to use it

1. In Instagram: **Settings → Accounts Centre → Your information and permissions → Export your information**
2. **Create export → your account → Export to device**
3. Under **Some of your information**, tick only **Followers and following**, set the format to **JSON**
4. Download the export when it's ready, then drop the `.zip` (or the `followers_1.json` + `following.json` files inside it) onto the page

You get:
- How many people you follow / follow you / are mutuals
- The full **not following you back** list, with profile links
- The reverse list too — who follows you that you don't follow back
- Search + one-click copy of the whole list

## How it works

One static HTML page. It parses Instagram's official export files locally with JavaScript (ZIPs are unpacked in the browser with JSZip), diffs the two lists, and renders the result. There is no server and no analytics.

## License

MIT — take it, fork it, make it yours.
