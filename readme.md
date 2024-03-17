<h1>Bootstrap5</h1> 

- is the newest version of Bootstrap, which is the most popular HTML, CSS, and JavaScript framework for creating responsive, mobile-first websites.

- Responsive web design is about creating web sites which automatically adjust themselves to look good on all devices, from small phones to large desktops.

---

Bootstrap5 Containers Class->

```
Class Extrasmall<576px  Small≥576px  Medium≥768px Large≥992px Extra large≥1200px XXL≥1400px
.container-sm  100% 540px 720px 960px 1140px 1320px
.container-md   100% 100% 720px 960px 1140px 1320px
.container-lg   100% 100% 100% 960px 1140px 1320px
.container-xl   100% 100% 100% 100% 1140px 1320px
.container-xxl  100% 100% 100% 100% 100% 1320px
```
---

The grid system is responsive, and the columns will re-arrange automatically depending on the screen size.

---

### The Bootstrap 5 grid system has six classes:
-  ```.col-*-*``` The first star (*) represents the responsiveness: sm, md, lg, xl or xxl, while the second star represents a number, which should add up to 12 for each row.
(if last * is not given it take as auto-column width, or used when we can't determine the number of columns)

```

.col- (extra small devices - screen width less than 576px)
.col-sm- (small devices - screen width equal to or greater than 576px)
.col-md- (medium devices - screen width equal to or greater than 768px)
.col-lg- (large devices - screen width equal to or greater than 992px)
.col-xl- (xlarge devices - screen width equal to or greater than 1200px)
.col-xxl- (xxlarge devices - screen width equal to or greater than 1400px)

```

### Row columns
- Use the responsive ```.row-cols-*``` classes to quickly set the number of columns that best render your content and layout.

- ```.row-cols-4``` means the number of columns in a row are set to 4. This class can be added to any .row divider to specify that there should be four equally space must be placed within a .row container. Here must be placed within a .row container.

- Whereas normal ```.col-*``` classes apply to the individual columns (e.g., .col-md-4), the row columns classes are set on the parent .row as a default for contained columns. With .row-cols-auto you can give the columns their natural width.

---

### Gutters
- are the padding between your columns, used to responsively space and align content in the Bootstrap grid system.

- Gutters are the gaps between column content, created by horizontal padding. We set padding-right and padding-left on each column, and use negative margin to offset that at the start and end of each row to align content.

- Gutters start at 1.5rem (24px) wide. This allows us to match our grid to the padding and margin spacers scale.

- Gutters can be responsively adjusted. Use breakpoint-specific gutter classes to modify horizontal gutters, vertical gutters, and all gutters.
```
1 rem= 16px;
$grid-gutter-width: 1.5rem;
$gutters: (
0: 0,
1: $spacer * .25,
  2: $spacer _ .5,
3: $spacer,
  4: $spacer _ 1.5,
5: \$spacer \* 3,
);
```

### Horizontal gutters
- ```.gx-*``` classes can be used to control the horizontal gutter widths. The .container or .container-fluid parent may need to be adjusted if larger gutters are used too to avoid unwanted overflow, using a matching padding utility. For example, in the following example we’ve increased the padding with ```.px-4```:

---

### Vertical gutters
```.gy-*``` classes can be used to control the vertical gutter widths. Like the horizontal gutters, the vertical gutters can cause some overflow below the .row at the end of a page. If this occurs, you add a wrapper around .row with the .overflow-hidden class:

---

### Text Alignment Class

``` text-*-* ```classes can be used to control the text alignment within a column.The first star * represents the responsiveness: ```sm, md, lg, xl or xxl```.

```
text-start
text-center
text-end

text-break

text-transform
text-uppertaste
text-captalize

- Font size:
fs-1 2.5 rem
fs-2 2 rem
fs-3 1.75 rem
fs-4 1.5 rem
fs-5 1 rem

- Font weight and italics:
fw-bold
fw-bolder
fw-normal
fw-lighter
fst-italic
fst-normal

```
--------------------

### Utility Classes (Spacing)
Margin and Padding
Where property is one of:

m - for classes that set margin
p - for classes that set padding
Where sides is one of:

t - for classes that set margin-top or padding-top
b - for classes that set margin-bottom or padding-bottom
s - (start) for classes that set margin-left or padding-left in LTR, margin-right or padding-right in RTL
e - (end) for classes that set margin-right or padding-right in LTR, margin-left or padding-left in RTL

x - for classes that set both _-left and _-right
y - for classes that set both _-top and _-bottom
blank - for classes that set a margin or padding on all 4 sides of the element

0 - for classes that eliminate the margin or padding by setting it to 0

1 - (by default) for classes that set the margin or padding to $spacer * .25
2 - (by default) for classes that set the margin or padding to $spacer _ .5
3 - (by default) for classes that set the margin or padding to $spacer
4 - (by default) for classes that set the margin or padding to $spacer _ 1.5
5 - (by default) for classes that set the margin or padding to \$spacer \* 3
auto - for classes that set the margin to auto

---

### Background Colors
The classes for background colors are:
```
.bg-primary,  
.bg-success,
.bg-info,
.bg-warning,
.bg-danger,
.bg-secondary,
.bg-dark
.bg-light.
```
---

Border & Border-radius
Use border utilities to quickly style the border and border-radius of an element. Great for images, buttons, or any other element.
```
<span class="border"></span>
<span class="border-top"></span>
<span class="border-end"></span>
<span class="border-bottom"></span>
<span class="border-start"></span>
```

Border color-
Change the border color using utilities built on our theme colors.
```
<span class="border border-primary"></span>
<span class="border border-secondary"></span>
<span class="border border-success"></span>
<span class="border border-danger"></span>
<span class="border border-warning"></span>
<span class="border border-info"></span>
<span class="border border-light"></span>
<span class="border border-dark"></span>
<span class="border border-white"></span>
```
Border-width-
```
<span class="border border-1"></span>
<span class="border border-2"></span>
<span class="border border-3"></span>
<span class="border border-4"></span>
<span class="border border-5"></span>
```
Border-radius-
```
<img src="..." class="rounded" alt="...">
<img src="..." class="rounded-top" alt="...">
<img src="..." class="rounded-end" alt="...">
<img src="..." class="rounded-bottom" alt="...">
<img src="..." class="rounded-start" alt="...">
<img src="..." class="rounded-circle" alt="...">
<img src="..." class="rounded-pill" alt="...">
```
Sizes-
```
<img src="..." class="rounded-0" alt="...">
<img src="..." class="rounded-1" alt="...">
<img src="..." class="rounded-2" alt="...">
<img src="..." class="rounded-3" alt="...">
```
---

### Text Color-
```
text-primary
text-secondary
text-success
text-danger
text-warning bg-dark
text-info bg-dark
text-light bg-dark
text-dark
text-body
text-muted
text-white bg-dark
text-black-50
text-white-50 bg-dark
```

---

### Responsive images-

1.  Images in Bootstrap are made responsive with ```.img-fluid```. This applies ```max-width: 100%```; and ```height: auto```; to the image so that it scales with the parent element.
2.  you can use ```.img-thumbnail``` to give an image a rounded 1px border appearance.
3.  Align images with the helper float classes or text alignment classes. block-level images can be centered using the .mx-auto margin utility class.

---

### Float and Clear Classes

1.  Toggle floats on any element, across any breakpoint, using our responsive float utilities.
2.  These utility classes float an element to the left or right, or disable floating, based on the current viewport size using the CSS float property. !important is included to avoid specificity issues. These use the same viewport breakpoints as our grid system. Please be aware float utilities have no effect on flex items.
3.  Quickly and easily clear floated content within a container by adding a clearfix utility.
4.  Easily clear floats by adding .clearfix to the parent element. Can also be used as a mixin.
    Here are all the support classes:
  ```
    .float-start
    .float-end
    .float-none
    .float-sm-start
    .float-sm-end
    .float-sm-none
    .float-md-start
    .float-md-end
    .float-md-none
    .float-lg-start
    .float-lg-end
    .float-lg-none
    .float-xl-start
    .float-xl-end
    .float-xl-none
    .float-xxl-start
    .float-xxl-end
    .float-xxl-none
  ```
---

Buttons
Use Bootstrap’s custom button styles for actions in forms, dialogs, and more with support for multiple sizes, states, and more.
```
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>
```
The .btn classes are designed to be used with the ```<button>``` element. However, you can also use these classes on ```<a> or <input>``` elements (though some browsers may apply a slightly different rendering).

Fancy larger or smaller buttons? Add .btn-lg or .btn-sm for additional sizes.

---

### Card Layout-
- A card is a flexible and extensible content container.
- It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options.
- If you’re familiar with Bootstrap 3, cards replace our old panels,
wells, and thumbnails
- Similar functionality to those components is available as modifier classes for cards.

Hiding elements in Bootstrap->

Screen size Class
```
Hidden on all .d-none
Hidden only on xs .d-none .d-sm-block
Hidden only on sm .d-sm-none .d-md-block
Hidden only on md .d-md-none .d-lg-block
Hidden only on lg .d-lg-none .d-xl-block
Hidden only on xl .d-xl-none .d-xxl-block
Hidden only on xxl .d-xxl-none
Visible on all .d-block
Visible only on xs .d-block .d-sm-none
Visible only on sm .d-none .d-sm-block .d-md-none
Visible only on md .d-none .d-md-block .d-lg-none
Visible only on lg .d-none .d-lg-block .d-xl-none
Visible only on xl .d-none .d-xl-block .d-xxl-none
Visible only on xxl .d-none .d-xxl-block
```