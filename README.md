# Rowboat Music

Rowboat Music is a [Hugo](https://gohuho.io) theme for music sites.

## Example Site

An [example site](https://github.com/jack126guy/rowboat-music-example) is available which demonstrates all of the different features.

## Features

### Recent Releases

Although Rowboat Music does not require a particular organization of music, you should place normal musical releases in the "releases" section. This way, a list of the most recent releases will appear on the homepage.

By default, up to five releases are listed. Set the `recentReleaseCount` site parameter to a different number to change how many are listed.

### Cover Art

You can add cover art as a [page resource](https://gohugo.io/content-management/page-resources/) named `cover.xyz` where `.xyz` is any file extension such as `.png` or `.jpg`.

Adding a page resource is perhaps the simplest way to add cover art, but there are a few different ways to do it. These are listed in order of priority (higher-priority items override lower-priority ones).

1. Add a `customcover` parameter to the [front matter](https://gohugo.io/content-management/front-matter). This should be the path to an image file, relative to the base of the site (refer to the [relURL](https://gohugo.io/functions/relurl/) function).
2. Add a `coverof` parameter to the front matter. This should be the path to another page ([cross reference](https://gohugo.io/content-management/cross-references/)) to use the same cover art as that page. (Be careful when using this option because it is possible to create an infinite loop.)
3. Add a [page resource](https://gohugo.io/content-management/page-resources/) named `cover.xyz` where `.xyz` is any file extension. (This is the method mentioned previously.)
4. Add cover art to the parent page using one of the methods mentioned. Subpages will inherit the cover art unless it is overridden.

### References

References are lists of links to other pages, such as a track list for an album. Different reference types can be defined, such as tracks, parts, works in progress, and so on.

(More detailed documentation is needed. For now, refer to the example site for information on using the reference system.)

## License

Rowboat Music is available under the MIT License. Refer to `LICENSE.txt` for details.

Files under the `static` directory are dedicated to the public domain under [Creative Common CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). (A copy is available in `LICENSE-STATIC.txt`.) The intent of this dedication is to allow users to create a site using this theme without having to provide a copy of the license: These files are copied, not output from a program, so the license would apply if not for this dedication.