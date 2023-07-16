# Core Modules Assignment 2 - CSS

---

**Q1.** What’s Box Model in CSS ?

**Ans.1** The box model is a fundamental concept in CSS that describes how elements are rendered on a web page by considering them as rectangular boxes. It consists of four components: `content`, `padding`, `border`, and `margin`.

Components of the box model and the CSS properties associated with each:

**Content:** The content area is the actual space occupied by the element's content, such as text, images, or other nested elements.The content area is controlled by the following CSS properties:

`width:` Sets the width of the content area.

`height:` Sets the height of the content area.

`max-width:` Sets the maximum width the content area can have.

`max-height:` Sets the maximum height the content area can have.

**Padding:** Padding is the space between the content and the element's border. It provides extra space inside the element. The padding area is controlled by the following CSS properties:
`padding-top, padding-right, padding-bottom, padding-left`: Sets the padding on each side individually.

`padding:` Sets the padding on all sides at once (in clockwise order: top, right, bottom, left).

**Border:** The border surrounds the content and padding area, giving the element a visible boundary. The border area is controlled by the following CSS properties:

`border-width:` Sets the width of the border.

`border-color:` Sets the color of the border.

`border-style:` Sets the style of the border (e.g., solid, dashed, dotted).

**Margin:** The margin is the space outside the element, separating it from other elements. It creates space between adjacent elements. The margin area is controlled by the following CSS properties:
`margin-top, margin-right, margin-bottom, margin-left`: Sets the margin on each side individually.

`margin: `Sets the margin on all sides at once (in clockwise order: top, right, bottom, left).

---

**Q2.** What are the Different Types of Selectors in CSS & what are the advantages of them?

**Ans.2** CSS provides various types of selectors to target and apply styles to specific elements in an HTML document. The different types of selectors in CSS along with their advantages:

**Element Selectors:** These selectors target elements based on their tag name.For example, `p` targets all `<p>` elements.

**Advantages:**

- Simple and easy to use.
- Can target multiple elements of the same type at once.
- Applicable to any HTML element.

**Class Selectors:** Class selectors target elements based on their class attribute. For example, .highlight targets all elements with `class="highlight"`.

**Advantages:**

- Allows grouping and applying styles to multiple elements with the same class.
- Enables reusable styles across multiple elements.
- Allows combining with other selectors for more specific targeting.

**ID Selectors:** ID selectors target elements based on their id attribute. For example, `#header` targets the element with `id="header"`.

**Advantages:**

- Provides a unique identifier for a specific element.
- Can target and style a single element precisely.
- Useful for JavaScript interactions and bookmark linking.

**Adjacent Sibling and General Sibling Selectors:** Adjacent sibling selectors target an element that immediately follows another element, while general sibling selectors target elements that are siblings of another element.

**Advantages:**

- Allows targeting specific elements based on their relationship to other elements.
- Useful for styling specific combinations or sequences of elements.

**Pseudo-classes and Pseudo-elements:** Pseudo-classes target elements based on a specific state or condition, such as `:hover` or `:first-child`. Pseudo-elements target specific parts of an element, such as `::before` or `::after`.

**Advantages:**

- Enables targeting elements based on user interaction or specific states.
- Allows styling specific parts or elements within an element.

**Descendant Selectors:** Descendant selectors target elements that are descendants of another element. For example, div p targets all `<p>` elements inside a `<div>`.

**Advantages:**

- Provides a way to target specific elements within a parent container.
- Allows applying styles to a specific hierarchy of elements.

---

**Q3.** What is VW/VH ?

**Ans.3** In CSS, `vw (viewport width)` and `vh (viewport height)` are relative units of measurement that represent a percentage of the viewport's width and height, respectively.

**Viewport-relative Units (vw/vh):**

**vw:** 1 vw is equal to 1% of the viewport's width. For example, 50vw would be 50% of the viewport width.

**vh:** 1 vh is equal to 1% of the viewport's height. For example, 25vh would be 25% of the viewport height.

**Advantages:**

- Viewport-relative units allow you to create responsive designs that adapt to different screen sizes.
- They provide a flexible and dynamic way to size elements based on the available viewport space.
- Particularly useful for creating fluid layouts or responsive typography.

---

**Q4.** What is difference between Inline, Inline Block and block ?

**Ans.4** There are three display properties that determine how elements are rendered and flow within the document: `inline, inline-block, and block.`

**Inline:**
Inline elements do not start on a new line. They flow alongside other elements, as much as space allows.

Inline elements only take up the necessary space to contain their content, without creating line breaks or vertical gaps.

Examples of inline elements include `<span>, <a>, <strong>, <em>,` and `<img>`.

Inline elements cannot have width or height properties, and margins and paddings only affect the horizontal space, not the vertical space.

**Inline Block:**
Inline-block elements share characteristics of both inline and block elements.

They flow alongside other elements like `inline elements`, but they also respect `width, height, margin,` and `padding` properties like `block elements.`

Inline-block elements can have a specified width and height, and they create line breaks when necessary.

Examples of inline-block elements include `<input>`, `<button>,` and` <select>` by default. However, any block-level element can be turned into an inline-block using CSS.

**Block:**
Block-level elements start on a new line and occupy the full width available by default.

Block elements create vertical gaps and line breaks before and after them, creating distinct blocks of content.

They can have width, height, margin, padding, and other box model properties.

Examples of block-level elements include `<div>, <p>, <h1> to <h6>, <ul>, <li>,` and `<section>`.

---

**Q5.** How is Border-box different from Content Box?

**Ans.5** In CSS, the box-sizing property allows you to control how the total width and height of an element are calculated. There are two commonly used values for the box-sizing property: `content-box` and `border-box`.

**Content Box (Default):**

**The box-sizing:** `content-box;` value is the default behaviour for elements.

With content-box, the width and height of an element are calculated by considering only the content area and excluding the padding, border, and margin.

In other words, the specified width and height values do not include the additional space taken up by the padding and border.

**Border Box:**

**The box-sizing:** `border-box;` value alters the box model behaviour.

With border-box, the width and height of an element are calculated by including the content area, padding, and border.

In this mode, the specified width and height values represent the total space that the element will occupy, including its content, padding, and border.

The margin is still calculated outside the specified width and height, as it does not affect the element's size.

---

**Q6.** What’s z-index and How does it Function ?

**Ans.6** `z-index` is a CSS property that determines the stacking order of positioned elements on the `z-axis.` It controls the overlapping and visibility of elements when they overlap in a document. The `z-index `property accepts an integer value, and elements with higher` z-index` values are displayed in front of elements with lower `z-index `values.

Here's how `z-index` functions:

**Stacking Context:** Each positioned element (positioned with `position: relative, position: absolute,` or `position: fixed`) creates a stacking context. The stacking context defines the context in which the `z-index` property is applied.

**Default Stacking Order:** Elements have a default z-index value of auto, which means they participate in the normal stacking order based on their position in the HTML document and the order in which they appear.

**Integer Values:** The z-index property accepts integer values, both positive and negative. Elements with higher z-index values are stacked in front of elements with lower z-index values within the same stacking context.

**Parent-Child Relationship:** The z-index property is relative to the stacking context created by the nearest positioned ancestor element. A child element cannot be stacked above its parent if the parent has a higher z-index value.

**Sibling Elements:** Siblings within the same stacking context are stacked based on their z-index values and their order in the HTML document. Elements with higher z-index values appear in front of elements with lower z-index values.

---

**Q7.** What’s Grid & Flex and difference between them?

**Ans.7**

**Grid:**
CSS Grid Layout (or simply Grid) is a two-dimensional layout system that allows you to create complex grid-based layouts.

Grid provides a way to divide a container into rows and columns, creating a grid of cells where you can place elements.

It offers precise control over both the horizontal and vertical alignment of elements.

Grid allows you to define the size and placement of items within the grid cells using properties like `grid-template-columns, grid-template-rows, grid-column, grid-row,` etc.

Grid is well-suited for creating grid-based designs, such as card layouts, image galleries, and overall page structures.

Grid is generally used for creating layouts at a higher level, managing the overall structure of the page.

**Flexbox:**
CSS Flexible Box Layout (or Flexbox) is a one-dimensional layout system that focuses on distributing and aligning elements along a single axis (either horizontally or vertically).

Flexbox allows for flexible and dynamic layouts, adjusting the size and positioning of elements to fit different screen sizes.

It provides a container (flex container) and its child elements (flex items) that can flexibly grow, shrink, and be aligned.

Flexbox offers properties like `flex-direction, justify-content, align-items,` and `align-self` to control the behavior and positioning of `flex items`.

Flexbox is particularly useful for creating responsive designs, aligning elements within a container, and creating flexible navigation menus, equal-height columns, or centered content.

Flexbox is generally used for creating smaller components or sections within a layout, rather than managing the overall structure of the page.

---

**Q8.** Difference between absolute and relative and sticky and fixed position explain with example.

**Ans.8** The CSS positioning properties `absolute, relative, sticky, and fixed` are used to control the position of elements on a web page.

**Absolute Positioning:**
When an element is positioned as absolute, it is removed from the normal document flow and positioned relative to its nearest positioned ancestor or the initial containing block if no positioned ancestor exists.

The position of the element is specified using the `top, right, bottom, and left` properties.

Absolute positioned elements are not affected by other elements and can overlap with other content.

**Example:**

```css
.container {
	position: relative;
}
.absolute-element {
	position: absolute;
	top: 10px;
	left: 20px;
}
```

In this example, the `.absolute-element` will be positioned 10 pixels from the top and 20 pixels from the left of its nearest positioned ancestor (`.container`).

**Relative Positioning:**
When an element is positioned as `relative`, it remains in the normal document flow, but its position can be adjusted using the `top, right, bottom, and left `properties.

Relative positioning does not remove the element from the document flow, so it still affects the layout of surrounding elements.

**Example:**

```css
.relative-element {
	position: relative;
	top: 10px;
	left: 20px;
}
```

In this example, the .relative-element will be moved 10 pixels down and 20 pixels to the right, without affecting the position of other elements.

**Sticky Positioning:**
When an element is positioned as `sticky`, it acts as a hybrid between `relative` and `fixed` positioning.

The element behaves as `relative` until a specified scroll threshold is reached, after which it becomes fixed and remains in a `fixed` position.

The position of the element can be controlled using` top, right, bottom, and left`, similar to other positioning methods.

Sticky positioning is useful for creating elements that stick to a specific position as the user scrolls, such as sticky navigation bars.

```css
example: .sticky-element {
	position: sticky;
	top: 20px;
}
```

In this example, the `.sticky-element` will behave as relative until it reaches a scroll position of 20 pixels from the top, after which it becomes `fixed` and stays at that position.

**Fixed Positioning:**
When an element is positioned as `fixed`, it is removed from the normal document flow and remains fixed relative to the browser viewport, regardless of scrolling.

The position of the element is specified using `top, right, bottom, and left` properties.

Fixed positioned elements are not affected by scrolling and are always visible in the same position, creating a `"fixed"` effect.

**Example:**

```css
.fixed-element {
	position: fixed;
	top: 10px;
	right: 20px;
}
```

In this example, the .fixed-element will be positioned 10 pixels from the top and 20 pixels from the right of the viewport.

---

**Q9.** Build Periodic Table as shown in the below image:

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F41470e09-2a72-448e-b080-ed9ede4b3c76%2Fperiodic_table.png?id=769a10d4-c2ba-4af0-8de5-28bee2644c3f&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [Periodic Table Code](https://github.com/yashPundhir/Periodic_Table_Assignment)

---

**Q10.** Build Responsive Layout both desktop and mobile and Tablet, see below image for reference:

![img](https://pwskills.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fa884c074-bb09-4827-a38f-290726e97f64%2Fresponsive.jpg?id=1174eb35-8bb2-41cf-aee6-376b8890092c&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=2000&userId=&cache=v2)

## [Responsive Layout Code](https://github.com/yashPundhir/Mobile_Responsiveness_Practice_Assignment)

---
