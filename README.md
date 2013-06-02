CSS Element Queries
===================

A proof-of-concept event-based CSS element dimension query with valid CSS selector syntax.

This means:

 - High-speed.
 - No interval/timeout detection. It's truly event-based.
 - No CSS modifications.
 - Valid CSS Syntax.
 - All CSS selectors available. It uses the normal attribute selector.
 - Support for webkit/gecko/internet explorer.
 - `min-width`, `min-height`, `max-width` and `max-height` are yet supported.
 - It works for almost all modification: HTML changes, inline styles, DOM mutation, CSS3 transitions.

Example
-------

```css
.widget-name {
    padding: 25px;
}
.widget-name[max-width="200px"] {
    padding: 0;
}
.widget-name[min-width="500px"] {
    padding: 55px;
}
```

Info: This is a first very experimental version! You should not use it yet.
