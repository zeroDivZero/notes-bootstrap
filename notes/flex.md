# FLEX

Display behavior utilities to create flexbox container and transform children into flex items. Manages layout, grid column sizing, navigation, and components.

## Direction

Horizontal (`flex-row`, default) or vertical (`flex-column`):

```html
<div class="d-flex flex-row">
  <div class="p-2">Flex item 1</div>
  <div class="p-2">Flex item 2</div>
  <div class="p-2">Flex item 3</div>
</div>

<div class="d-flex flex-column">
  <div class="p-2">Flex item 1</div>
  <div class="p-2">Flex item 2</div>
  <div class="p-2">Flex item 3</div>
</div>
```

Use `.flex-row-reverse` or `.flex-column-reverse` to reverse child order.

Responsive variations: `.flex-sm-row`, `.flex-md-column-reverse`, `.flex-lg-row-reverse`, `.flex-xl-column`, etc.

## Justify Content

Specifies alignment of flex items on main axis:

```html
<div class="d-flex justify-content-start">...</div>
<div class="d-flex justify-content-end">...</div>
<div class="d-flex justify-content-center">...</div>
<div class="d-flex justify-content-between">...</div>
<div class="d-flex justify-content-around">...</div>
<div class="d-flex justify-content-evenly">...</div>
```

Responsive variations are available.

## Align Items

Specifies alignment of flex items on cross axis:

```html
<div class="d-flex align-items-start">...</div>
<div class="d-flex align-items-end">...</div>
<div class="d-flex align-items-center">...</div>
<div class="d-flex align-items-baseline">...</div>
<div class="d-flex align-items-stretch">...</div>
```

Responsive variations are available.

## Align Self

Specifies alignment of individual flex item on cross axis. Same options and responsive variations as align-items. Examples:

```html
<div class="align-self-end">...</div>
<div class="align-self-lg-center">...</div>
<div class="align-self-xxl-stretch">...</div>
```

## Fill

Use `.flex-fill` class (and responsive variations like `.flex-md-fill`) on siblings to fill up available space relative to their content.

```html
<div class="d-flex">
  <div class="p-2 flex-fill">Flex item with a lot of content</div>
  <div class="p-2 flex-fill">Flex item</div>
  <div class="p-2">Flex item</div>
</div>
```

## Grow and Shrink

Grow first one and give other two necessary space:

```html
<div class="d-flex">
  <div class="p-2 flex-grow-1">Flex item</div>
  <div class="p-2">Flex item</div>
  <div class="p-2">Another flex item</div>
</div>
```

Shrink second one by force wrapping content to new line:

```html
<div class="d-flex">
  <div class="p-2 w-100">Flex item</div>
  <div class="p-2 flex-shrink-1">Flex item</div>
</div>
```
