# hw01-intro

This is the text that I'm adding just to demo git.

My demo repo for webdev

Deployed on: https://hw01-intro.vercel.app/

## `index.html` -- the minimum you should actually write

```html
<!DOCTYPE html>
<html>
<head><meta charset="UTF-8" /><title>Hello</title></head>
<body>Hello, world!</body>
</html>
```

This includes `<meta charset="UTF-8">` even though the page would render fine
without it (the content here is plain ASCII) -- omitting it isn't just a
style nit, it's a real security anti-pattern (see `../anatomy.md`), so it's
worth including even in the minimal example.

## The literal fewest bytes a browser will still render identically

HTML5's parser auto-inserts `<html>`, `<head>`, and `<body>` even if you omit
them, so this technically works too:

```html
<!DOCTYPE html><title>Hello</title>Hello, world!
```

Not something to actually write or teach as a pattern -- it relies on
browser-implied structure instead of explicit, readable markup, which is
exactly the kind of "too clever" shortcut that makes code harder to reason
about later. Included here as a fact about how HTML5 parsing works, not a
recommendation.
