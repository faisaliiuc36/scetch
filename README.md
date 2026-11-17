# Pencil Sketch Reveal

**One-line description:** A single-file web app that turns any photo or cartoon character into a pencil-sketch "Guess Who?" video with sound, ready for YouTube, Facebook, Reels and Shorts.

---

## What it does

You pick a character (or upload your own photo). The app draws it stroke by stroke like a pencil sketch, builds up tension with music and sound effects, then reveals the full-colour picture and the answer name. You can record the result as a video or save the frame as a PNG.

No install, no server, no account. Everything runs in the browser.

## How to use

1. Open `sketch.html` in a modern browser (Chrome or Edge recommended).
2. Use the tabs on the right:
   - **Size**: choose the video format.
   - **Text**: set the title, the line under it, and the answer name. Pick a colour theme and a paper style.
   - **Demo**: choose a category (Players, Presidents, Actors) and a character.
   - **Photo**: upload your own image, or paste an image link.
   - **Look**: line detail, shading, drawing speed, colour pencils, colour reveal, show the pencil.
   - **Sound**: background sound, pencil sound, sound effects.
3. Press **Play it** to preview, **Record video** to save a video, or **Save PNG** to save the current frame.

## Features

**Video sizes**

| Format | Size |
|---|---|
| YouTube / Facebook video | 1920 × 1080 (16:9) |
| Reels / Shorts / TikTok | 1080 × 1920 (9:16) |
| Facebook / Instagram feed | 1080 × 1350 (4:5) |
| Square post | 1080 × 1080 (1:1) |

**Demo characters (8 per category, drawn in code)**

- **Players:** Messi, Ronaldo, Neymar, Mbappé, Haaland, Salah, Modric, Kane (cartoon footballers told apart by kit colour and number).
- **Presidents:** President 1 to 8 (generic cartoon characters in suits).
- **Actors:** Action Hero, Movie Star, Comedian, Rock Star, Heartthrob, Villain, Dancer, Superstar (generic cartoon characters).

Choosing a category sets the title automatically: `GUESS THE PLAYER`, `GUESS THE PRESIDENT` or `GUESS THE ACTOR`. You can still edit it.

**Your own image**

- Click **Choose an image**, drag an image onto the page, or press `Ctrl+V` to paste one.
- Or paste an image link (works with links that allow it, such as Wikimedia Commons).
- A thumbnail and file name show that the image is selected, and the preview shows it straight away.

**Look**

- Themes: Stadium night, Fire, Neon, Emerald.
- Paper: Cream, White, Chalkboard.
- Sliders: line detail, shading, drawing speed.
- Toggles: colour pencils, colour reveal at the end, show the pencil.

**Sound** (all of it is included in the recorded video)

- **Background sound:** Epic, Suspense, Stadium, Chill, or Off, with a volume slider and a preview button.
- **Pencil sound:** Soft rub, Soft tap, or Off, with a volume slider and a preview button.
- **Sound effects:** whoosh, riser, booms and cheer, on or off.

## Using a real name

The Presidents and Actors are generic characters, not likenesses of real people. To use a real name, type it in **Answer name** on the Text tab. It is shown big at the end of the video. For a real face, use your own photo instead.

## Optional: your own photo library

To add your own photos to the Demo tab, create a folder named `players` next to `sketch.html` and add a file `players/players.json` listing the image file names:

```json
["my-photo-1.jpg", "my-photo-2.png"]
```

Each image appears as a button in the Players category. This works when the page is served from a web server (a plain double-click on the file may block it in some browsers).

## Requirements

- A modern desktop browser. Chrome or Edge give the best video recording.
- Internet access for the Google Fonts (Bebas Neue, Inter, Poppins). Without it the page still works but uses fallback fonts.
- Video recording uses the browser's built-in recorder. It saves **MP4** where supported, otherwise **WebM**.

## Tips

- Play once before recording so you know the timing. The timer next to the status bar shows the length.
- Lower **Drawing speed** for a longer, more dramatic sketch; raise it for a shorter video.
- If the video file has no sound, check that the browser tab was not muted and that **Background volume** is above 0.
- Settings such as video size and the last open tab are remembered in the browser.

## Files

| File | What it is |
|---|---|
| `sketch.html` | The whole app (HTML, CSS and JavaScript in one file) |
| `README.md` | This file |
