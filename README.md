# adaptation-problem-list-in-mobile-browser

### 1.  remove the blue background of click area
```css
-webkit-tap-highlight-color: transparent;
```

### 2. "Smooth" scroll on mobile device
```css
-webkit-overflow-scrolling: touch;
```
PS：this property conflicts with `-webkit-appearance: none;`

### 3. centering items with flexbox and overflow
```css
.parent {
  margin: auto;
  display: flex;
  // ....
}
```

### 4. prevent pull to refresh
```css
html,
body {
    overscroll-behavior-y: contain;
}
```

### 5. `overflow:hidden` applied to `body` not working on iPhone Safari
```css
html, body {
  overflow-y: hidden;
  height: 100%;
}
```
but scrollTop becomes 0
