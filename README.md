# minimal firefox

Changed a good bit from original repository. That was a cohesive set of CSS hacks to construct a more minimal Firefox experience, but hasn't been updated to keep up with changes in Firefox elements for some years now.

This is my personal configuration for Firefox that operates on these principles:

1. Use [sidebery](https://addons.mozilla.org/en-US/firefox/addon/sidebery/) for vertical tree-style tabs

Since the tab handing is offloaded to sidebery, the relevant CSS tweaks are actually to the sidebery extension (its theme) or the auto-hide tweak:
- https://github.com/MrOtherGuy/firefox-csshacks/blob/master/chrome/autohide_sidebar.css

2. hide the tab bar

At the time of writing (March 2025) hiding the tab bar entirely is easy:

```css
#TabsToolbar {
    display: none !important;
}
```

3. minimize the URL bar's noise, keeping as much of the full URL visible as possible

