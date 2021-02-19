<h1 class="capitalize">COMD2451</h1>
<h2 class="capitalize center">Advanced CSS text Properties</h2>

---

<section class="section">
    <h2 class="sentence">CSS text effect properties</h2>
    
***Commonly*** used `CSS text effect` are:

+ text-overflow
+ word-wrap
+ word-break
+ writing-mode

</section>

---

<section class="section">
    <h2 class="sentence">CSS Text Overflow</h2>
    
The `CSS text-overflow property` ***specifies*** how ***overflowed content*** that is ***not displayed*** should be ***represented*** to the `user`. It ***can*** be `clipped`, ***display*** an `ellipsis` (...), or ***display*** a ***custom*** `string`.

The `text-overflow property` ***requires*** the ***following*** `property declarations` to ***also*** be ***present***:

```css
white-space: nowrap;
overflow: hidden;
```

**Example**:

```css
div {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
```

A ***way*** of ***achieving*** `overflow` is by ***applying*** the `value` of `nowrap` to the `white-space` *`CSS property`*. The `text` ***has*** to be `overflowing` in ***order*** for `text-overflow` ***features*** to work. ***However***, the ***default*** `white-space property` ***value*** for `text` IS `nowrap`, so ***unless*** it ***has*** to be ***explicitly applied*** for ***some reason*** (**like** that its ***default behavior*** has been ***overridden*** somewhere ***else***), it is ***not*** necessary to ***add*** it.

The `text-overflow property` ***accepts*** the ***following*** `property values`:

+ `clip`: The ***default*** value. The `text` is ***clipped*** and ***not*** accessible.

+ `ellipsis`: ***Render*** an `ellipsis` ("...") to ***represent*** the ***clipped*** `text`.

+ `string`: ***Render*** the ***given*** `string` to ***represent*** the ***clipped*** text.

+ `initial`: ***Sets*** this `property` to its ***default*** `value`.

+ `inherit`: ***Inherits*** this `property` ***from*** its `parent element`.	

<aside class="notes">
    Note: Go to the [CSS text-overflow Property](https://www.w3schools.com/cssref/css3_pr_text-overflow.asp) to show live examples.
</aside>

</section>

---

<section class="section">
    <h2 class="sentence">The CSS word-wrap property</h2>
    
The `CSS word-wrap property` ***allows*** `long words` to be able to be ***broken*** and ***wrap*** onto the ***next line***.

If a **word** is ***too long*** to ***fit*** within an **area**, it ***expands outside***. That's ***because*** of the `text`'s ***default*** `white-space: nowrap` ***property declaration*** `applied` to it.

This ***especially happens*** when ***long*** `URLs` are ***included*** in the `text content` in **normal flow**.

The `word-wrap property` ***accepts*** the ***following*** `values`:

+ `normal`: `Break words` ***only*** at ***allowed*** `break points`. This is the ***default*** `value`.
+ `break-word`: ***Allows*** `unbreakable words` to be ***broken***.
+ `initial`: ***sets*** the `word-wrap property` to its ***default*** `value`.
+ `inherit`: ***inherits*** the `word-wrap property` ***from*** its `parent element`.

`Example` ***not using*** the `word-wrap property`, so the ***implicit*** `value` of `normal` is ***applied***:

The **HTML**:

```html
<article>
    <h2>CSS word-wrap</h2>
    <p class="para">This is some text with a very long URL: https://www.geeksforgeeks.org/what-is-the-difference-between-word-break-break-all-versus-word-wrap-break-word-in-css/
    </p>
</article>
```

The **CSS**:

```css
article {
    background: blue;
    width: 175px;
}
```

`Example` ***using*** the `word-wrap property` ***with*** the `value` of `break-word`:

The **HTML**:

```html
<article>
    <h2>CSS word-wrap property</h2>
    <p class="para">This is some text with a very long URL: https://www.geeksforgeeks.org/what-is-the-difference-between-word-break-break-all-versus-word-wrap-break-word-in-css/
    </p>
</article>
```

The **CSS**:

```css
article {
    background: blue;
    width: 175px;
    word-wrap: break-word;
}
```

<aside class="notes">
    Note: I'll take the students into the browser and make sure that I also have each example code applied to the index.html and the styles.css in each instance.
</aside>

</section>

---

<section class="section">
    <h2 class="sentence">The CSS word-break property</h2>
    
The `CSS word-break property` ***specifies*** `how words` ***should*** `break` ***when reaching*** the ***end*** of a `line`.

The `CSS word-break property` ***accepts*** the ***following*** `values`:

+ `normal`: ***Default*** `value`. Uses ***default*** `line break` ***rules***.
+ `break-all`: To ***prevent*** `overflow`, `word` may be ***broken*** at ***any character***.
+ `keep-all`: `Word breaks` ***should not*** be ***used*** for `Chinese/Japanese/Korean` (`CJK`) `text`. ***Non-CJK*** `text` ***behavior*** is the ***same*** as value `"normal"`.
+ `break-word`: To ***prevent*** `overflow`, `word` ***may be** `broken` at ***arbitrary points***.
+ `initial`: ***Sets*** the `word-break property` to its ***default*** `value`.
+ `inherit`: ***Inherits*** the `word-break property` ***from*** its `parent element`.

<aside class="notes">
    Show the students examples on the [CSS word-break Property](https://www.w3schools.com/cssref/css3_pr_word-break.asp) page on w3schools.
</aside>

</section>

---

<section class="section">
    <h2 class="sentence">The CSS writing-mode property</h2>
    
The `CSS writing-mode property` ***specifies*** whether `lines` of `text` are ***laid out*** `horizontally` or `vertically`.

The `CSS writing-mode property` ***accepts*** the ***following*** `values`:

+ `horizontal-tb`: ***Let*** the `content` ***flow horizontally*** from `left` to `right`, ***vertically*** from `top` to `bottom`.
+ `vertical-rl`: ***Let*** the `content` ***flow vertically*** from `top` to `bottom`, ***horizontally*** from `right` to `left`.
+ `vertical-lr`: ***Let*** the `content` ***flow vertically*** from `top` to `bottom`, ***horizontally*** from `left` to `right`.

<aside class="notes">
    Show the students examples on the [CSS writing-mode Property](https://www.w3schools.com/cssref/css3_pr_writing-mode.asp) page on w3schools.
</aside>

</section>

---

<section class="section">
    <h2 class="sentence">CSS text Affect Properties</h2>
    
The ***following*** is a ***list*** of the `CSS text effect` ***properties***:

+ [text-align-last](https://www.w3schools.com/cssref/css3_pr_text-align-last.asp): ***Specifies*** how to ***align*** the `last line` of a ***block*** of `text`.
+ [text-justify](https://www.w3schools.com/cssref/css3_pr_text-justify.asp): ***Specifies*** how `justified text` ***should be*** `aligned` and `spaced`.
+ [text-overflow](https://www.w3schools.com/cssref/css3_pr_text-overflow.asp): ***Specifies*** how ***overflowed*** `content` that is ***not displayed*** should be ***signaled*** to the `user`.
+ [word-break](https://www.w3schools.com/cssref/css3_pr_word-break.asp): ***Specifies*** `line breaking` ***rules*** for ***non-CJK*** (Chinese, Japanese, Korean) `scripts`.
+ [word-wrap](https://www.w3schools.com/cssref/css3_pr_word-wrap.asp): ***Allows*** `long words` to be ***able*** to be ***broken*** and ***wrap*** onto the ***next line***.
+ [writing-mode](https://www.w3schools.com/cssref/css3_pr_writing-mode.asp): ***Specifies*** whether `lines` of `text` are ***laid out*** `horizontally` or `vertically`.

<aside class="notes">
    Show the students examples on the [CSS Text Effects](https://www.w3schools.com/css/css3_text_effects.asp) page on w3schools.
</aside>

</section>

---

<section class="section">
    <h2 class="sentence">Related Resources</h2>
    
+ [CSS white-space Property: Digital Ocean](https://www.digitalocean.com/community/tutorials/css-white-space-property)
</section>



