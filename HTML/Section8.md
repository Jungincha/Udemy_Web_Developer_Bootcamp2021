# Section 8: The CSS box model

#### box-sizing
It sets how the total width and height of an element i calculated
- content-box
<br>: The default CSS box-sizing behavior
- border-box
<br>: It tells the brower to account for any border and padding in the values you specify for an element's width and height

#### Display property
- block
<br>The element generates a block element box, generating line breaks both before and after the element when in the normal flow
- inline
<br>The element generates one or more inline element boxes that do not generate line breaks before or after themselves. It ignores width and height.
- inline-block 
<br>The element generates a block element box that will be flowed with surrounding content as if it were a single inline box

#### CSS Units
- px (absolute)
- % (relative)
<br>Percentages are always relative to some other value
- em
<br>Font size of the parent, in the case of typographical properties like `font-size`, and font size of the element itself, in the case of other properties like `width`
- rem
<br>Relative font size of the root element
