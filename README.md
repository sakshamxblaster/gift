# Our One Month Anniversary Website

A romantic one-page website for Saksham & Tanu: song + photo slideshow, story timeline, the first rose, "79 times", cards and a letter (Hinglish / English).

## Files
- `index.html`: page structure
- `style.css`: colours and layout
- `script.js`: **all the text lives at the top (the `C` object)**: names, start date, story, cards, note, letter
- `assets/`: song (`song.mp3`, `song.m4a`, and `song-data.js` which is a built-in backup copy of the song), photos and Discord screenshots

## Preview in VS Code
1. Open this folder in VS Code (File > Open Folder).
2. Install the extension **Live Server** (Ritwick Dey).
3. Right-click `index.html` > **Open with Live Server**.
(Opening `index.html` by double-click also works, but Live Server is better.)

## Put it online with GitHub Pages
1. Create a free account at github.com and click **New repository**. Name it e.g. `our-month` and keep it **Public** (free GitHub Pages needs public).
2. Upload everything in this folder (keep the `assets` folder as it is):
   - easiest: on the new repo page click **uploading an existing file**, drag all files and the `assets` folder in, then **Commit changes**.
   - or with git:
     ```
     git init
     git add .
     git commit -m "anniversary site"
     git branch -M main
     git remote add origin https://github.com/YOUR_USERNAME/our-month.git
     git push -u origin main
     ```
3. In the repo go to **Settings > Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After about a minute your link is: `https://YOUR_USERNAME.github.io/our-month/`

## Things to know
- A public repo means anyone who finds it can see the photos, screenshots and song file. Use a hard-to-guess repo name and share the link only with Tanu.
- The song needs one tap on **Play our song** (phones block automatic sound).
- To change a name, date or any text, edit the top of `script.js`, then commit/upload the changed file again.

## If the song does not play
- Under the Play button you will see the song time, like `0:00 / 3:29`. The page first tries `assets/song.mp3`, then `assets/song.m4a`, and if both fail it switches to the built-in backup in `assets/song-data.js` by itself (this can take up to 5 seconds after the page opens).
- Upload/keep the whole `assets` folder (all files in it) next to `index.html`.
- Check the file: `song.mp3` should be about 3.2 MB. If it is 0 KB or tiny, unzip again.
- Play and Pause: tap the button, or tap the photo. On a computer, Space also works.
- Open the page through Live Server or your GitHub link, in Chrome or Safari (not inside WhatsApp or the Files app).
