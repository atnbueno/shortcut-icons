# shortcut-icons

A CSS sprite to represent iOS shortcut icons.

Grab the [stylesheet](https://github.com/atnbueno/shortcut-icons/blob/main/shortcut-icons.css) and the [default (iOS 14) glyph set](https://github.com/atnbueno/shortcut-icons/blob/main/ios14-glyphs.png), and add a shortcut icon to your HTML with just an empty `div` element:

```html
<div class="shortcut-icon c4251333119 g59793 s86"></div>
```

In this example `shortcut-icon` is the base CSS class. The secondary `c4251333119` class is the orange **color** from iOS 14, the `g59793` class is the "paintbrush" **glyph** and the `s86` class is the desired **icon size**. See the [demo.html](https://github.com/atnbueno/shortcut-icons/blob/main/demo.html) file for more examples.

The color and glyph **numeric values** can be found both in the shortcut metadata (see below) and in its _plist_ (the shortcut "source code").

The HTML element doesn't have to be a `<div>`, although using other elements may require additional CSS to reset their appearance.

If you want to use the colors and glyphs from iOS 12 and/or iOS 13, grab the glyph sets you want to use and add an additional `ios12` or `ios13` class to each HTML element.

And if you need a size not in the CSS, it's easy to define your own. For example, to get 58×58 icons:

```css
.s58  { --icon-size:  58px }
```

## Accessing a shortcut's metadata

To access a shortcut's metadata add `api/records/` after `shortcuts/` in its iCloud link. Example:

https://www.icloud.com/shortcuts/0e011689efc949a291f231333c6dd2b3 \
↓\
https://www.icloud.com/shortcuts/api/records/0e011689efc949a291f231333c6dd2b3

## Sites that use this

- [RoutineHub](https://routinehub.co/)
- My (non-public yet 😅) website

## License

As the [LICENSE](https://github.com/atnbueno/shortcut-icons/blob/main/LICENSE) explains, I don't claim authorship of the glyphs. Those are Apple's and I'm using them to show what can be seen in publicly published iCloud links. The limited resolution of the assets is intentional.
