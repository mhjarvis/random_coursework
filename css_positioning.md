<h1 align=center>----- CSS Positioning -----</h1>

### The ```position:``` element.

There are five different types of positioning: ```:static | :relative | :sticky | :absolute | :fixed | :inherit```.

```:static``` is the normal layout, the default. Block-level elements generate a rectangular box that is part of the document's flow; inline-level boxes cuase the creation of one or more line boxes that are followed within their parent element.

```:relative``` has the element's box offset by some distance. The element retains the shape it would have had were it not positioned, and the space that the element would ordinarily have occupied is preserved.

```:absolute``` has the element's box completely removed from the flow of the document and positioned with respect to its containing block, which may be another element in the document or the initial containing block (described in the next section). Whatever space the element might have occupied in the normal document flow is closed up, as though the element did not exist. The positioned element generates a block-level box, regardless of the type of box it would have generated if it were in the normal flow.

```:fixed``` has the element's box behave as though it was set to ```:absolute```, but its containing block is the viewport itself.

```:sticky``` has the element left in the normal flow until the conditions that trigger its stickiness come to pass, at which point it is removed from the normal flow but its original space in the normal flow is preserved. It will then act as if absolutely positioned with respect to its containing block. Once the conditions to enforce stickiness are no longer met, the element is returned to the normal flow in its original space.

### The containing block.

Generally, the box that contains another element (as ```html``` is the containing block for the ```body``` element). The containing block depends entirely on the type of positioning.

### Notes

#### The ```static``` Property
```static``` is not affected by top, bottom, left, right properties / values.

#### The ```relative``` Property
```relative``` top, bottom, left, right properties / values cause the element to be moved from its normal position.

#### The ```absolute``` Property
```absolute``` positioned relative to its parent element that is positioned ```relative```.

#### The ```fixed``` Property
```fixed``` positioned relative to the viewport (whole browser window, will stay put).

#### The ```sticky``` Property
```sticky``` positioned based on scroll position.