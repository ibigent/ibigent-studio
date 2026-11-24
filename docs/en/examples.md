# Examples — IBIGENT Studio

**[Docs home](../../README.md)**

With the IBIGENT Studio MCP connected in your AI tool, you drive the editor by asking the AI to build HTML.

## Basic flow
1. In IBIGENT Studio, open the editor.
2. In your AI tool, ask for a section as HTML and to send it to your IBIGENT Studio editor.
3. In the editor, pick the insertion point — the HTML appears there.

## Example prompt
```
Build a responsive "our services" section as HTML with four cards,
then send it to my IBIGENT Studio editor.
```

The AI generates the HTML and, through the MCP connection, delivers it to your editor; you choose where it goes.

## Edit by just asking — no code (IBIGENT AI Hosting & Builder Hosting)
Keep the editor open and describe the change. The AI reads the page and edits only that part. No code is needed.

```
Change the main headline to "A warm place to grow"
```

```
Make the selected text red
```

The change appears in the editor within 2–3 seconds with an **Undo** notice. Save in the editor when you are happy (your live site does not change until you save).

## Build a new homepage or content page from material
Prepare your company profile, menu structure and page text with the AI, then say:

```
Build a new homepage from our company profile
```

```
Make a CEO greeting page from this material
```

The material fills the editor's "New homepage" (Builder) or "Add content page" window. Review it and click [Next]; IBIGENT builds it with its own design. Existing boards and posts stay as they are. For a content page, keep a content-page editor open.

## Add a submenu (IBIGENT AI Hosting, sites with sub-pages)
```
Add an Implants page under the Treatments menu
```

## Upload a site you built yourself (IBIGENT AI Hosting)
1. Ask your AI tool (Claude Code, Codex, Cursor, etc.) to build the site in a folder, then zip the whole folder. The zip must contain `index.html`, up to 100MB. Executable files such as PHP are left out for security.
2. In the editor, drop the zip onto **Site deploy** (bottom right) and click **Upload and deploy**. Zip files cannot be sent through MCP — upload them yourself.
3. When the progress bar finishes, the site is live at your address and shown in the editor. Deploying replaces the previous site. For boards or a database, use Builder Hosting.

After uploading you can edit the site in the editor or by asking your AI, as above. Your site's scripts are kept when you save, and the uploaded original is kept in **Restore saved version** the first time you save. The editor does not run your site's scripts, so parts drawn by scripts (language switchers, sliders) may look different there — check them with **Live preview** next to the save button.

For exact editor steps and the on-screen send flow, see the official docs: https://www.ibigent.com/docs/ibigent-studio/

---
**Keywords:** IBIGENT Studio examples, AI HTML to editor, MCP usage
