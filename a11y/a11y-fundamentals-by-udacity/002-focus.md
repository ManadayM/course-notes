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

## Offscreen Content

In cases where elements are hidden from the viewport but they still fall under the tab order. For example, the list of menu items inside a collapsed hamburger menu. We can set its `visibitily` to `none` to remove them from the focus/tab order.

## Modals & Keyboard Traps

> Keyboard focus is never locked or trapped at one particular page element. The user can navigate to and from all navigable page elements using only a keyboard. [[WCAG 2.1.2](https://webaim.org/standards/wcag/checklist#sc2.1.2)]

This rule emphasis that keyboard focus should not be trapped at any one web page element.

However, there are times when the trapped keyboard focus is desirable. For example, Form opened in a modal dialog. Here the desired behviour is that focus should happen only on focusable form elements on the modal. When user submits or clicks on the overlay/grey area outside the modal surface the focus should go back to the actual active element on the web page.

_This lesson presented a very elegant way to achieve roving focus on a `modal` window and return the focus to original element when we're done. Check this video: https://www.youtube.com/watch?v=BoAsayPVogE&feature=youtu.be&t=135._

----------
#### [Previous](001-a11y-overview.md) |  [Table of contents](000-toc.md) | [Next](003-semantics.md)