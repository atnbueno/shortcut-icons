# shortcut-icons

A CSS sprite to represent iOS shortcut icons.

Grab the CSS and the glyph sets you want to use, and add a shortcut icon with just an empty HTML element:

```html
<div class="shortcut-icon c4251333119 g59716 s87"></div>
```

In this example `c4251333119` is the orange color from iOS 14, `g59716` is the "color dropper" glyph and `s87` is the shortcut size.

The color and glyph values can be found both in the shortcut metadata¹ and in its _plist_.

The HTML element doesn't have to be a `<div>`.

If you want to use the colors and shortcuts from iOS 12 and/or iOS 13, grab all the glyph sets you want to use and add an additional `ios12` or `ios13` class to your HTML element.

## (¹) Accessing a shortcut's metadata

To access a shortcut's metadata add `api/records/` after `shortcuts/` in its iCloud link. Example:

<https://www.icloud.com/shortcuts/0e011689efc949a291f231333c6dd2b3> → <https://www.icloud.com/shortcuts/api/records/0e011689efc949a291f231333c6dd2b3>
