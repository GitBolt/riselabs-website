# RISE Lab website

The website for RISE Lab, Department of Aerospace Engineering, University of Illinois Urbana-Champaign.

It is plain HTML and CSS. There is no framework and no build step. Node.js is only used to preview the site on your computer.

For hosting, domain, accounts and launch steps, see [NOTES.md](NOTES.md).

## Files

```
index.html                    Home page
about.html                    About us
pearl.html                    PEARL
spirit.html                   SPIRIT
student-collaboration.html    Student collaboration
sponsorships.html             Sponsorships
join.html                     Join the team
styles.css                    All the styling for every page
images/                       Photos, logos and videos go here
package.json                  Tells Node how to run the preview
```

That's the whole site.

## See it on your computer

Option 1: double-click `index.html`. It opens in your browser.

Option 2: run a local server with Node.js (closer to how the live site behaves).

1. Install Node.js (the LTS version) from https://nodejs.org
2. Open a terminal in this folder and run:

   ```bash
   npm install
   npm start
   ```

3. Open the address it prints, usually http://localhost:3000

After you edit a file, save it and refresh the browser.

## How the pages are built

Every page has the same three parts:

1. **Header** at the top, with the logo text and menu
2. **Sections** in the middle, each starting with a comment like `<!-- ===== Research areas ===== -->`
3. **Footer** at the bottom, with "Contact us"

The header and footer are copied into every page. If you change the menu or the contact details, change them in all seven files.

To show which page you are on, the menu link for that page has `class="current"`.

## Common edits

### Draft text

Text that still needs to be written is wrapped in a draft span, which shows in italics:

```html
<p><span class="draft">Mission statement TBD</span></p>
```

When the real text is ready, remove the span:

```html
<p>RISE Lab builds and tests...</p>
```


### Adding a photo

Put the photo in `images/`, then replace the gray placeholder box with an `<img>`. Keep the same size class so it stays the same shape.

```html
<!-- Before -->
<div class="photo-slot photo-card"><span>Landscape photo</span></div>

<!-- After -->
<img class="photo-card" src="images/test-stand.jpg" alt="Students at the test stand">
```

Size classes:

| Class | Shape | Used for |
| --- | --- | --- |
| `photo-wide` | Very wide | Top of each inner page |
| `photo-landscape` | 16:9 | News, CAD spin |
| `photo-card` | 3:2 | Cards |
| `headshot` | Portrait | People |

The home page banner photo is set in `styles.css`. Look for the comment "To use a real photo" in the `.hero` rule.

### Adding a person

Copy one of these blocks and change the text and photo:

```html
<div class="person">
  <img class="headshot" src="images/jane-doe.jpg" alt="Headshot of Jane Doe">
  <h3>Jane Doe</h3>
  <p class="small">Team lead</p>
</div>
```

### Adding a page

1. Copy an existing page, such as `spirit.html`, and rename it.
2. Change the title and content.
3. Add a link to it in the menu and footer of every page.

### Changing colors

The colors are listed at the top of `styles.css`. Change one there and it updates everywhere.

| Name | Color | Used for |
| --- | --- | --- |
| `--blue` | `#13294b` | Illinois blue: banners, footer |
| `--orange` | `#ff5f05` | Illinois orange: buttons only |
| `--soft-blue` | `#e3edf8` | PEARL page |

Fonts are Montserrat (headings) and Source Sans 3 (text), loaded from Google Fonts in each page's `<head>`.

## Before launch

- Replace all draft text and photo placeholders
- Add the logo once the name and logo are confirmed with the university
- Delete the `<meta name="robots" content="noindex">` line from every page so search engines can find the site
