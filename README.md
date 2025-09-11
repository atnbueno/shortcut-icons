# Shortcut Icons  

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/atnbueno/shortcut-icons?style=social)](https://github.com/atnbueno/shortcut-icons/stargazers)
[![Demo](https://img.shields.io/badge/demo-online-green)](https://atnbueno.com/shortcut-icons/demo.html)

A lightweight CSS sprite library for displaying **iOS shortcut icons** in your web projects.

## Quick Start  

Grab the [stylesheet](https://github.com/atnbueno/shortcut-icons/blob/main/shortcut-icons.css) and the [default (iOS 26) glyph set](https://github.com/atnbueno/shortcut-icons/blob/main/ios26-glyphs.png), and add a shortcut icon to your HTML with just an empty `div` element:

```html
<div class="shortcut-icon c4251333119 g59793 s86"></div>
```

In this example `shortcut-icon` is the base CSS class. The secondary `c4251333119` class is the orange **color** from iOS 26, the `g59793` class is the "paintbrush" **glyph** and the `s86` class is the desired **icon size**.

See the [live demo](https://atnbueno.com/shortcut-icons/demo.html) and [its source](https://github.com/atnbueno/shortcut-icons/blob/main/demo.html) file for more examples.

The color and glyph **numeric values** can be found both in the shortcut metadata (see below) and in its _plist_ (the shortcut "source code"). See below for how to get them using a shortcut.

The HTML element doesn't have to be a `<div>`, although using other elements may require additional CSS to reset their appearance.

If you want to use the colors and glyphs from iOS 12-18, grab the glyph sets you want to use and add an additional `ios12`, `ios13`, `ios14`, `ios15`, `ios16`, `ios17`, or `ios18` class to each HTML element.

And if you need a size not in the CSS, it's easy to define your own. For example, to get 58×58 icons:

```css
.s58  { --icon-size:  58px }
```

## Accessing a shortcut's metadata

To access a shortcut's metadata add `api/records/` after `shortcuts/` in its iCloud link. Example:

<https://www.icloud.com/shortcuts/3c00aa9f2c57462e81f78007efca59d2> \
↓\
<https://www.icloud.com/shortcuts/api/records/3c00aa9f2c57462e81f78007efca59d2>

## Accessing a shortcut's own icon

This shortcut shows how to get the image, the color code and the glyph code of a shortcut icon. It does it with itself, but it would be easy to modify it to let the user pick another shortcut from their library.

**Get Shortcut Icon Info**
<https://www.icloud.com/shortcuts/3c00aa9f2c57462e81f78007efca59d2>


## Sites that use this

- [RoutineHub](https://routinehub.co/)
- Cherri's [Shortcuts Glyph Search](https://glyphs.cherrilang.org/)
- [Live demo in my site](https://atnbueno.com/shortcut-icons/demo.html)
- [Shortcut repository](https://atajos.wiki/repo) from [@shortcuts_es](https://t.me/shortcuts_es)

## License

As the [LICENSE](https://github.com/atnbueno/shortcut-icons/blob/main/LICENSE) explains, I don't claim authorship of the glyphs. Those are Apple's and I'm using them to show what can be seen in publicly published iCloud links. The limited resolution of the assets is intentional.

## Credits

Thanks to [@ActuallyTaylor](https://github.com/ActuallyTaylor/) for her help in getting the hi-res versions of the glyphs for the first versions. Without her I don't think I'd have the patience to do this.

Thanks also to the members of [r/Shortcuts'](https://discord.gg/HrzAhUu) and [RoutineHub's](https://discord.gg/2prYfrSUmc) Discords for their feedback.
