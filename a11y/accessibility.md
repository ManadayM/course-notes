# Accessibility (a11y)

## Notes from the podcast by Wesbos

Web is for all people regardless of their race, gender, software, language, or ability. And hence website, applications badly designed they can create barriers that can exclude people from using the web.

~ Tim Berners-Lee

### Tips & Easy wins

- Write good code
- Semantic HTML structure
- Think what is most semantic element for your purpose
- Respect hierarchy of heading tags
- Button vs Link - for action use button for navigating somewhere use anchor link
- Use more semantic element like `section`, `article`, `header`, `footer`, `aside`

### `img` element
- Use `img` tag for actual images, not `background-img`
- `alt` tag is very important for your `content` images
- Avoid adding words like `Picture of` as prefix in `alt` tags as screen reader knows already that it's a picture

### Colors

- Contrast is important aspect
- Use online contrast checker tools
- Try `Grayscale` mode on your Mac

### Custom HTML elements

- If you use custom elements to design a website then screen readers don't natively undertstand them. Here comes the ARIA into the picture.
- `Skip to content` link at very top of the page or blog post (example https://deque.com)
- aXe for Chrome Tools for auditing your website against accessibility standards.

### Screen Readers

- NVAccess - Open Source Screen Reader for Windows
- ChromeVox - Chrome extension

### Large websites

- People having slow connectivity cannot access your website smoothly. This is also a part of accessibility.

## Udacity Course Notes

### Web Content Accessibility Guidelines (WCAG) 2.0

- It's a guidelines and best practices to try and answers the questions what a11y means in a methodical way.

#### Organised around 4 core principles aka POUR
- Perceivable
- Operable
- Understandable
- Robust

### WebAIM WCAG Checklist

It is a high level checklist specifically for web content - https://webaim.org/standards/wcag/checklist ([PDF Version](https://webaim.org/standards/wcag/WCAG2Checklist.pdf))

### Focus

WebAIM WCAG 2.0 Checklist 2.1.1 Keyboard
>  All page functionality is available using the keyboard, unless the functionality cannot be accomplished in any known way using a keyboard (e.g., free hand drawing)

- Focus determines where keyboard events go in the page
- Built in HTML interactive elements are implicitly focusable meaning they're automatically in tab order + built-in keyboard event handling. For example, input, button, and select.
- Not all elements are focusable. For example, headers, div, and images.
- [Flight Booking Form](http://udacity.github.io/ud891/lesson2-focus/01-basic-form/) with disabled mouse inputs

WebAIM WCAG 2.0 Checklist 1.3.2 Meaningful Sequence
> The reading and navigation order (determined by code order) is logical and intuitive.
