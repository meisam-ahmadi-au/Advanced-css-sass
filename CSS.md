# CSS

## important

* responsive design
  * Fluid layouts
  * Media queries
  * responsive images
  * correct units
  * desktop-first vs mobile-first
* maintainable and scaleable code
  * clean
  * easy to understand
  * growth
  * reusable
  * how to organize files
  * how to name classes
  * how to structure HTML
* performance
  * Less HTTP requests
  * less code
  * compress code
  * use a CSS preprocessor
  * less images
  * compress images

## cascading

* is the process of combining different stylesheets from
  * author
  * user
  * browser

* importance
  * user !important
  * author !important
  * author declarations
  * user declarations
* specificity
  * inline style
  * IDs
  * classes, pseudo-classes, attribute
  * elements, pseudo-elements
* source order
  * the last declaration wins

## values

* font: x%; x% of parent's font-size
* length: x%; x% of parent's width
* font: Xem; X * parent font-size
* length: Xem; X * current element font-size
* Xrem; X * root font size for both length and fonts
* Xvw, Xvh: X percent of height and width of the parent

## Box Model

* content
* padding
* border
* margin
* fill area: content + padding + border

## Box Types

* block: block, flex, list-style, table
  * 100% parent width
  * vertically, one after another
  * box-model applies
* inline
  * content is distributed inline
  * occupies only content's space
  * no line-breaks
  * no heights and widths
  * only horizontal padding and margin
* inline-block
  * occupies only content's space
  * no line-breaks
  * box-model applies

## Positioning schemes

* Normal flow
  * default, position: relative
  * laid out according to their source order
* Floats
  * float: left or right
  * need to clear
  * removed from normal flow
  * text and inline elements will wrap around the floated element
  * the container will not adjust its height to the element
* Absolute positioning
  * position: absolute or fixed
  * removed from normal flow
  * no impact on surrounding content or elements
  * use top, bottom, left and right to offset the element

## stacking context

* z-index
* opacity
* transform

## CSS Architecture

* think - build - architect
* component design
* Block-Element-Modifier
* Block: standalone component that is meaningful on its own
* Element: part of a block that has no standalone meaning
* Modifier: a different version of a block or an element
* architect: itcss, smacss, 7-1 pattern

## Basics of Responsive Design

* use % rather than px
* responsive images
* media queries

## Useful websites

* Reset.css
* caniuse.com
* demo.agektmr.com/
* leaverou.github.io/animatable/
* cssfontstack.com
* codrops.com
* mediaqueri.es
* WebAIM, Accessibility
* bennettfeely.com/clippy/
* easing.net
* cubic-bezier.com
* statcounter
* sizzy.com => for different size

## Some CSS Reset

* box-sizing: border-box
* *, *:before, *:after { box-sizing: inheret }
* use rem for whole website;

## Floats

* .row::after { content:""; clear: both; display: table}

## Picture Tag

* art direction
* __< picture >__  & __< source >__ tage
* scottjehl.github.io/picturefill responsive image polyfill
* __< svg >__ & __< use xlink:href >__ tags

## flexbox

* align-content
* justify-items

## grid

* grid: col1 col2 ... / row1 row2 ...
* grid-area: row-start / col-start / row-end / col-end
* grid-template-column: repeate( Num, width1 width2 ...)
* fit-content(20%)
* justify-items, justify-self, align-items, align-self, justify-content, align-content

## test CSS

* percy.io

## em, rem

* em is relative to its parent
* rem is a multiplication of font-size of html
* line-height: unitless, it will multiply its own font-size

## background

* background: blue url() no-repeat 0px 0px / cover
* rgba(); color with alpha transparency
* background: linear-gradient(color, color), url() no-repeat
* background-clip: content-box, padding-box, border-box
* background blend mode

## Media Query and Retina Display

* min-resolution: 192dpi
* device-pixel-ratio

## shapes

* shapes
* shape function

## ARIA GuideLine

* Accessibility

## CSS Style Guides

* be descriptive
  * primary-header
  * secondary-header
* functional names
  * alert-button
  * submit-button

## counters

* counter-increment: myCounter increment-value
* counter(myCounter)
* counter-reset: myCounter;

## centering

* position: absolute;
* top:0; bottom:0; left:0; right:0;
* margin: auto;

## putting icons on anchor tags

* <__a data-icon="abcdxyz"__>
* a::before { content: attr(data-icon)}

## fonts

* load them seperately in HTML

## coverage

* more tools / coverage

## feature query

* @supports (display: grid) { body { display: grid; } }

* ::selection