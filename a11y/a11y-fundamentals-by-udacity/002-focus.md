# Focus

WebAIM WCAG 2.0 Checklist 2.1.1 Keyboard
>  All page functionality is available using the keyboard, unless the functionality cannot be accomplished in any known way using a keyboard (e.g., free hand drawing)

- Focus determines where keyboard events go in the page
- Built in HTML interactive elements are implicitly focusable meaning they're automatically in tab order + built-in keyboard event handling. For example, input, button, and select.
- Not all elements are focusable. For example, headers, div, and images.
- [Flight Booking Form](http://udacity.github.io/ud891/lesson2-focus/01-basic-form/) with disabled mouse inputs

WebAIM WCAG 2.0 Checklist 1.3.2 Meaningful Sequence
> The reading and navigation order (determined by code order) is logical and intuitive.

## tabindex

### tabindex=0

When `tabindex` is set to `0`, the element is inserted into the tab order based on its location in the source code

### tabindex=-1

When `tabindex` is set to a negative integer like `-1`, it becomes programmatically focusable but it isn’t included in the tab order

### tabindex=1+

JUST AVOID!

### Limit `tabindex` usage

Limit using `tabindex` for interactive elements only where your users need to provide some input/interaction.

### Resources on Focus
- Using the tabindex attribute https://developer.paciellogroup.com/blog/2014/08/using-the-tabindex-attribute/#content
- https://dequeuniversity.com/rules/axe/3.0/tabindex

## Skip links

Skip link is way to enable users to directly jump to the main content of your web page. This feature is really useful for disability useful.

More: https://webaim.org/techniques/skipnav/

## Focus in complex components

- Roving focus - https://www.stefanjudis.com/today-i-learned/roving-tabindex/


----------
#### [Previous](001-a11y-overview.md) |  [Table of contents](000-toc.md) | [Next](003-semantics.md)