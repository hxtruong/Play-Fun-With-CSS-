# Play fun with CSS
Note some fun things

## Natour project prebuild 
- Animation: aniName time typeAction
- animation-fill-mode: use to specifies a style for the element when animation start (after, backwards, both)
- The **box-sizing** property can be used to adjust this behavior:

  * **content-box** gives you the default CSS box-sizing behavior. If you set an element's width to 100 pixels, then the element's content box will be 100 pixels wide, and the width of any border or padding will be added to the final rendered width.
  * **border-box** tells the browser to account for any border and padding in the values you specify for an element's width and height. If you set an element's width to 100 pixels, that 100 pixels will include any border or padding you added, and the content box will shrink to absorb that extra width. This typically makes it much easier to size elements.

## Behind the CSS
### Three pillars of CSS and HTML
1. Responsive design
  - Fluid layouts
  - Media queries
  - Responsive images
  - Correct units
  - Desktop-first and mobile-first

2. Maintainable and scalable code
  - Clean
  - Esay-to-understand
  - Growth
  - Reusable
  - Orgainze/Name classes/structure HTML
3. Web performance
  - Less HTTP request
  - Less code
  - Compress code
  - Use a CSS Preprocessor
  - Less images
  - Compress images

### Overview
When user to to a website
  * Load HTML
  * Parser HTML - Load CSS -> Parse CSS => CSS object model (CSSOM)
    - Line by line
    - Parse CSS: Resolve conflicting CSS declearations (cascade), Process final CSS values
  * =>> Document Object Model (DOM)

### CSS structure
- Two part: *Selector* and *Declaration block*
- The priority CSS will be appied:
  * Importance
    User->Author *important*
    Author->User declarations
    Default browser declarations
  * Specificty
    Inline: css is written in HTML code
    IDS
    Classes
    Elements: like button {color: 'white'}
    =>>> Example:
    #nav a.button:hover {} -> (0 inline, 1 ID, 2 class (include :hover pesuduo class), 1 element)
    =>>> Select the CSS has best specific
  * Source order: the last declaration in code will override all other declarations and will be applied

#### Size
- root font-size = 16px
- Percentages and relative values -> pixels
- *em*,*emm* and *rems*: font-size relate to prarent/current/document's root
- *vh, vw*: wiew height/width

#### Inheritance
- The *initial* keyword resets a property to its initial value
