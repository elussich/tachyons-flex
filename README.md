# TACHYONS-FLEX

This is an "unofficial" Tachyons module that provides a set of classes to construct flex box layouts.

## IMPORTANT NOTE:
**This module is deprecated and will no longer be maintained. [Latest Tachyons release](https://www.npmjs.com/package/tachyons) now provides flexbox capabilities, both inside the main package, and through the official flexbox module: (https://www.npmjs.com/package/tachyons-flexbox).**

### Why Flex Box?
Flex Box Layouts could easily be achieved by mixing & matching flex-related properties, stablishing a behavioral relationship between the flex container, and its inner flex items.

While flex box layout implementations are limitless, there are still some regularly common use cases from where to start. The classes enlisted here should provide enough flexibility to tackle down most of those scenarios, while keeping a simple and clear nomenclature.

Visit the official Tachyons site here: [http://tachyons.io](http://tachyons.io)

## Install
```
npm install --save-dev tachyons-flex
```
or download the css on github and include in your project.

## Usage

Just set a `df` class onto your desired _flex container_ element and a `flx-i` class onto a _flex item_ element, inside. For different results, mix & match the provided classes, and be sure to check `index.html` file for more thorough examples.

## The Code
```
/*

   ## FLEX BOX LAYOUT

   Mix & match container-level flex properties with item-level ones to achieve
   desired flex box layouts.

   More complex flex layout system may need more fine-tuned values for different
   flex properties, but in most cases, simple layouts can easily be achieved by
   a combination of the classes enlisted here.

   For further reference:
   https://developer.mozilla.org/en-US/docs/Web/CSS/flex

   ### To note:
   The `df` class defines a flex container, from where all flex layouts start.
   This class was defined following the syntax found on the __Display__ module:
   https://github.com/tachyons-css/tachyons-display

   Base:
    flx = Base for all flex-related properties

   Modifiers:
    dr = sets flex direction to row (default value)
    dc = sets flex direction to column
    drr = sets flex direction to reversed row
    dcr = sets flex direction to reversed column

    i = sets a flex item, standing for `flex: 1`; property value, which is a
    shorthand for `flex-grow: 1;`, `flex-shrink: 1;` and `flex-basis: 0%;`.
    This is the most likely usage for a flex item: to grow so as to take all
    white space available.

    g0 = sets flex grow to 0
    s0 = sets flex shrink to 0
    b0 = sets flex basis to 0%
    g1 = sets flex grow to 1
    s1 = sets flex shrink to 1
    b1 = sets flex basis to 100%

    ais = align items to stretch (default)
    aifs = align items to start (flex-start)
    aife = align items to end (flex-end)
    aic = align items to center
    aib = align items to baseline

    acs = align content to stretch (default)
    acfs = align content to start (flex-start)
    acfe = align content to end (flex-end)
    acc = align content to center
    acsb = align content with space between
    acsa = align content with space around

    ass = align self to stretch (default)
    asfs = align self to start (flex-start)
    asfe = align self to end (flex-end)
    asc = align self to center
    asb = align self to baseline

    jcfs = justify content to start (flex-start, default)
    jcfe = justify content to end (flex-end)
    jcc = justify content to center
    jcsb = justify content to space between
    jcsa = justify content to space around

    w = flex wrap
    wr = flex wrap reverse
    wn = flex no wrap (default)

    o0 = order 0
    o1 = order 1
    o2 = order 2
    o3 = order 3
    o4 = order 4
    o5 = order 5

*/

/*
  FLEX CONTAINER
 */
.df {
  display: flex;
}

/*
  FLEX DIRECTION
 */
.flx-dc {
  flex-direction: column;
}
.flx-dr {
  flex-direction: row;
}
.flx-dcr {
  flex-direction: column-reverse;
}
.flx-drr {
  flex-direction: row-reverse;
}

/*
  FLEX
 */
.flx-i {
  flex: 1;
}
.flx-g0 {
  flex-grow: 0;
}
.flx-s0 {
  flex-shrink: 0;
}
.flx-b0 {
  flex-basis: 0%;
}
.flx-g1 {
  flex-grow: 1;
}
.flx-s1 {
  flex-shrink: 1;
}
.flx-b1 {
  flex-basis: 100%;
}

/*
  ALIGN ITEMS
 */
.flx-ais {
  align-items: stretch;
}
.flx-aifs {
  align-items: flex-start;
}
.flx-aife {
  align-items: flex-end;
}
.flx-aic {
  align-items: center;
}
.flx-aib {
  align-items: baseline;
}

/*
  ALIGN CONTENT
 */
.flx-acs {
  align-content: stretch;
}
.flx-acfs {
  align-content: flex-start;
}
.flx-acfe {
  align-content: flex-end;
}
.flx-acc {
  align-content: center;
}
.flx-acsb {
  align-content: space-between;
}
.flx-acsa {
  align-content: space-around;
}

/*
  ALIGN SELF
 */
.flx-ass {
  align-self: stretch;
}
.flx-asfs {
  align-self: flex-start;
}
.flx-asfe {
  align-self: flex-end;
}
.flx-asc {
  align-self: center;
}
.flx-asb {
  align-self: baseline;
}

/*
  JUSTIFY CONTENT
 */
.flx-jcfs {
  justify-content: flex-start;
}
.flx-jcfe {
  justify-content: flex-end;
}
.flx-jcc {
  justify-content: center;
}
.flx-jcsb {
  justify-content: space-between;
}
.flx-jcsa {
  justify-content: space-around;
}

/*
  WRAP
 */
.flx-w {
  flex-wrap: wrap;
}
.flx-wr {
  flex-wrap: wrap-reverse;
}
.flx-wn {
  flex-wrap: nowrap;
}

/*
  ORDER
 */
.flx-o0 {
  order: 0;
}
.flx-o1 {
  order: 1;
}
.flx-o2 {
  order: 2;
}
.flx-o3 {
  order: 3;
}
.flx-o4 {
  order: 4;
}
.flx-o5 {
  order: 5;
}

```

## A Note on Class Names

First of all, I took the dare to add a `df` class, that follows the syntax presented on the [Display](https://github.com/tachyons-css/tachyons-display) module. This was a necessary decision, since HTML elements rely on the `display` property set to `flex` to be converted into "flex containers".

Unfortunately, Flex Box definitions don't necessarily have a "namespace" of their own, and are actually hard to wrap on a common syntax. For this effect, I set a `flx` base namespace, so then all flex-related properties are appended as modifiers, keeping them as short and less verbose as possible.

## Author

[elussich](https://github.com/elussich)

## License

The MIT License (MIT)

Copyright (c) 2015 Esteban Lussich

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
