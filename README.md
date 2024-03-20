# 🤓 Potion
Make websites look like a certain popular note taking app that may or may not rhyme with the name of this repo.

## What does it do?

If you just have your HTML file and nothing else, you can put one line of code into `<head>`, and it will instantly look like it was made in that note-taking app.

## Why?

I've seen [Fruition](https://fruitionsite.com) and really like it. I find that design really simple and attractive for things like demo pages, READMEs, documentation and other such things. However, the original thing loads extremely slowly and it's inaccessible because it was never designed to be used in such a way.

This is where Potion steps in.

## Advantages over the original

- 👌 No need to go through all that complicated Cloudflare settings as with Fruition
- ⚡️ It works much faster because it's just a single small CSS file
- 😈 No trackers, no JavaScript 
- 🪄 Accessible by default
- 🌱 Works much better on narrower screens than the original

## Usage

```HTML
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/miloxeon/potion/potion.min.css">
```

Put this into `head` of a plain HTML file. Done.

## Caveats

- If you want responsive tables, you should wrap your `table` in `<div class="table-wrapper">`. It'll make it scroll horizontally on narrower screens.
- For best results, put all your content into `<body>` or `<main>`.

## Supported elements

- Basic typography: paragraphs, headings (h1–h3), `strong`, `em`, `i`, `b`, `del`
- Blockquotes
- Links and images
- Tables: `table`, `tr`, `td`, `th`, `thead`, `caption`, `tbody`
- Lists: `ul`, `ol`, `li`
- Code: inline code with `code`, blocks of code with `pre`

## Classes and special components

### Header

The `<header>` on top of the `<body>` is special. It allows you to define page title, page icon and top image:

```HTML
<body>
    <header>
        <!-- Top image (optional) -->
        <div class="background" style="background-image: url(https://source.unsplash.com/1200x400)"></div>
      
        <!-- Page icon (optional) -->
        <div class="icon">🥳</div>
      
        <!-- h1 here becomes the page title (also optional but you better have it) -->
        <h1>Potion</h1>
    </header>
    ...
</body> 
```

### Responsive tables

You should wrap your `table` in `<div class="table-wrapper">` to make it scroll horizontally on narrower screens:

```HTML
<div class="table-wrapper">
    <table>
        ...
    </table>
</div>
```

### Colors

Original colors are supported:

- Gray
- Brown
- Orange
- Yellow
- Green
- Blue
- Purple
- Pink
- Red

You can color everything from spans and paragraphs to table cells. Colors are available for both the backgrounds and the text.

```HTML

<p class="c-yellow">Yellow text</p>
<p class="b-purple">Standard text on purple background</p>
<p class="c-blue b-red">Blue text on red background</p>

```

You may always refer to the demo page HTML as a guide of how to use Potion. It's really easy.

Enjoy!
