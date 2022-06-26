# CSS FLEXBOX

Flexbox is a unidimensional layout model, supported by most web browsers – Chrome, Firefox, Safari, Opera, Microsoft Edge, iOS and Android.

## Flex Container

The container's function is to wrap other items and with the `display: flex` property transform the child items into **flex items**.

![](C:\Users\isysa\AppData\Roaming\marktext\images\2022-06-19-12-02-00-image.png)

> Containers can be used with div, span, links, h1, h2...

```css
container {
    display: flex; //initializer
    flex-direction:; //line,column
    flex-wrap:;    //next line
    flex-flow:;    //applies the same value for both flex-direction and flex-wrap
    justify-content:;
    align-items:;    //adjusts axis
    align-content:;  //adjusts line
}
```

## Flex Item

```css
flex-item {
    flex-grow:; //how it grows
    flex-basis:; //initial size
    flex-shrink: //shrink capacity
    flex:; //applies the same value for the 3 above
    flex-order:; //list order
    align-self:; //alignment of the item individually
```

> Flex items can also be flex containers!

# FLEX CONTAINER - Fundamentals

### -display: flex

Turns all this tag's children into **flex items**. 

In spite of this, as the items' quantity grows, they may surpass the container's limit!

![](C:\Users\isysa\AppData\Roaming\marktext\images\2022-06-20-10-04-30-image.png)

### -flex-direction

Establishes the main axis on which all items will be placed. The axis options are:

- **row:** left to right

- **row-reverse:** right to left

- **column:** top to bottom

- **column-reverse:** bottom to top

![](C:\Users\isysa\AppData\Roaming\marktext\images\2022-06-20-10-47-11-image.png)

### -flex-wrap

This property is responsible for allowing whether the items should break line once they reache the box's limit or not.

- **nowrap:** it the default value for any container. It forbids the line break.
  
  While there's still space, the container compresses all items to the limit of their content's size — the items may also have min-width. When it's no longer possible to do so, the items will surpass the container's limit and fill the page.

- **wrap:** allows the items which surpass the container's limit to break line, starting a new row or column inside the container.

- **wrap-reverse:** stacks the rows or columns in such a way that the order is "bottom-up"
  
  > ![](C:\Users\isysa\AppData\Roaming\marktext\images\2022-06-20-10-57-15-image.png)

> The spacing ends up as a problem with all these properties when the container has a `max-width`!

### -flex-flow

Shortcut for flex-direction and flex-wrap.

### -justify-content

- **flex-start:** justifies to the container's beginning

- **flex-end:** container's end

- **center**

- **space-between:** creates an even spacing between the elements

- **space-around:** the spacing between the center items is two times bigger than the first and last.

> Different from align-items, justify-content depends on the container's height and width.

### -align-items

Takes care of the **flex items** alignment according to the container's axis. 

> *Changes according to whether the items are placed inside a column or row.

- **center**

- **stretch:** (default) stretches the item so it fills the container in its entirety.

- **flex-start**

- **flex-end**

- **baseline:** aligns according to the typography's base line. If the letter is immense, it won't overflow the container.

![](C:\Users\isysa\AppData\Roaming\marktext\images\2022-06-22-16-50-00-image.png)

### -align-content

Row orientation. For `align-content` to work, we have to have:

- a **container** that allows line breaks

- the container's **height** to be bigger than the sum of the row's items.

The available alignment types are

- **center**

- **stretch**

- **flex-start**

- **flex-end**

- **space-between**

- **space-around**

# Flex Item

### -flex-grow

Determines the item's growth proportion, respecting item's contents.

> Flex-grow won't work if the flex container has justify-content active!

### -flex-basis

Gives the item a **starting size**.

- **auto**

- you can also set the value in **px**, **%**, **em** and so on.

- **0** relates to the flex-grow in a way that it attempts to make all items the same size, according to the items' content.
