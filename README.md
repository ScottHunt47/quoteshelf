# Quote Shelf

An app for saving quotes from the books you read. It installs on your phone's home screen, works offline, and searches the Open Library catalogue for books and covers.

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
- **Import from Readwise:** on a computer, go to readwise.io/export and choose **Export to CSV**. Then in Quote Shelf tap the download icon, **Choose Readwise CSV**, and pick that file. Importing the same file again skips quotes you already have.
- **Markdown export** gives a readable file of all your quotes grouped by book, for Obsidian, Notion or Apple Notes.

## Scanning quotes
When adding a quote, tap **Scan with camera** (or **Use a photo** for one you've already taken). Take a photo of the page, then tap each line you want. The lines join into one passage, with words split across lines rejoined, and drop into the quote box for you to check before saving.

- Pick the book's language from the menu next to the scan buttons. The app remembers your choice.
- Everything is read on your phone. Photos are never uploaded anywhere.
- The first scan in each language downloads the text reader (around 5 to 15 MB), so do it on Wi-Fi.
- For best results, hold the page flat, fill the frame with the text, and avoid shadows.
- Always check the text before saving: scanning occasionally misreads a letter or punctuation mark.

## Sharing a quote as an image

Tap **Share** on any quote. Choose a size (wide, square, portrait or story), a style (Cover, Clean or Classic) and a colour, then tap **Share image** to send it to WhatsApp, Instagram, Messages and so on, or **Save image** to keep it. **Share text** sends the quote as plain text. On iPhone, the easiest way to keep an image is **Share image**, then **Save Image**


## Updating the app

If you change `index.html`, also change the `VERSION` line at the top of `sw.js` (for example `qs-v1` to `qs-v2`), then upload the folder again. Phones pick up the new version the next time the app opens with a connection.

## Files

- `index.html`: the whole app
- `sw.js`: makes it work offline
- `manifest.webmanifest`: the app's name, colours and icons for installing
- `icons/`: home-screen icons
