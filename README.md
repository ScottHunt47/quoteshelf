# Quote Shelf

A Readwise-style app for saving quotes from the books you read. It installs on your phone's home screen, works offline, and searches the Open Library catalogue for books and covers.

## Put it online (free, about 5 minutes)

The app has to be on the web once so your phone can install it. The easiest way:

1. Unzip `quote-shelf.zip` on your computer. You'll get a folder called `quote-shelf`.
2. Go to **app.netlify.com/drop** and create a free account.
3. Drag the `quote-shelf` folder onto the page.
4. Netlify gives you a web address like `something-random.netlify.app`. You can rename it in **Site settings → Change site name**, for example `scott-quotes.netlify.app`.

GitHub Pages and Cloudflare Pages work too. Upload the folder's contents, with `index.html` at the top level.

## Install it on your phone

Open your web address on your phone, then:

- **iPhone:** open it in **Safari**, tap **Share**, then **Add to Home Screen**.
- **Android:** open it in **Chrome**, tap the **⋮** menu, then **Install app** or **Add to Home screen**.

It now opens full screen from its own icon, like any other app, and works without a connection. Book search is the only part that needs the internet.

## Your data

Your books and quotes are saved **only on that phone**, inside the app. Nothing is sent anywhere except your book searches to Open Library.

That means:

- **Back up regularly.** Tap the download icon at the top, then **Save backup file**, and save it to iCloud Drive, Google Drive, or email it to yourself. The app reminds you once you have 10 or more quotes and no recent backup.
- **Moving to a new phone:** install the app there, then choose **Restore from a backup**.
- **Deleting the app from your home screen deletes your quotes** on most phones. Back up first.
- **iPhone:** if you don't open the app for several weeks, Safari can clear its data. Opening it now and then, and keeping backups, protects you.
- **Markdown export** gives a readable file of all your quotes grouped by book, for Obsidian, Notion or Apple Notes.

## Updating the app

If you change `index.html`, also change the `VERSION` line at the top of `sw.js` (for example `qs-v1` to `qs-v2`), then upload the folder again. Phones pick up the new version the next time the app opens with a connection.

## Files

- `index.html`: the whole app
- `sw.js`: makes it work offline
- `manifest.webmanifest`: the app's name, colours and icons for installing
- `icons/`: home-screen icons
