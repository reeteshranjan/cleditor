# cleditor
A version of [cleditor](http://premiumsoftware.net/cleditor/) with improvements and additional features
## Changes & Additions
- Fix for iframe `contentWindow is null` issue. This is a common issue with `iframes` added by `javascript` as seen [here](http://stackoverflow.com/a/12199913/3348386). There is a known solution where one needs to wait till the `iframe` 'loads'. The corresponding bug in cleditor got exposed when creating and destroying forms with `textarea` fields for which cleditor objects were created, while being on the same page. Modified the `reset` function as required for a fix.
- Support for `pre` tag. This is supported by others, and was a very simple addition.
- Retina-ready minimal buttons (designed 48px seen with 24px size) created from scratch. The default in this version of cleditor.
- From content box to border box based design to get rid of old-style 'accounting' for borders, paddings and margins in the dimensions of various objects
- Removed using deprecated `font` tag. Replaced the usage with font-size. Also hence moved from font sizes being 1, 2, 3 etc. to small, large, x-small, x-large etc.
