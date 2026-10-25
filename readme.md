# LeetCode Blind

LeetCode Blind is a small Chrome extension that hides problem difficulty labels on LeetCode, helping you choose and solve problems without seeing their difficulty first.

## What it does

- Hides the difficulty badge on individual problem pages.
- Hides difficulty labels in problem listings.
- Runs on `https://leetcode.com/*`.

The labels are hidden with CSS, so the page layout remains in place. The extension does not change problem data or submit solutions.

## Install in Chrome

1. Download or clone this project.
2. Open `chrome://extensions` in Chrome.
3. Turn on **Developer mode**.
4. Select **Load unpacked** and choose the project folder containing `manifest.json`.
5. Open or refresh a LeetCode page.

To apply changes after editing the extension files, select **Reload** on its card in `chrome://extensions`, then refresh the LeetCode page.

## Project files

- `manifest.json` — extension metadata and content-script configuration.
- `content.js` — runs on LeetCode pages and logs that the extension is active.
- `styles.css` — hides difficulty labels.

## Limitations

The extension targets the current difficulty-label selectors used by LeetCode. If LeetCode changes its page markup, some labels may become visible until the selectors are updated.
