Flexbox (Flexible Box Layout) is a CSS layout system used to **align, distribute, and control space between items inside a container**. It is very powerful for building responsive layouts.

---

# 1. Basic Flex Syntax

To use Flexbox you must first set the container to `display: flex`.

```css
.container {
  display: flex;
}
```

In **Tailwind CSS**:

```html
<div class="flex"></div>
```

This makes all **direct children** become **flex items**.

---

# 2. Main Axis vs Cross Axis

Flexbox works with two axes:

| Axis           | Meaning                 |
| -------------- | ----------------------- |
| **Main axis**  | Direction items flow    |
| **Cross axis** | Perpendicular direction |

Default:

```
Main Axis → Horizontal
Cross Axis ↓ Vertical
```

Example:

```
[ Item ] [ Item ] [ Item ]
```

---

# 3. flex-direction

Controls the **direction of items**.

### CSS

```css
.container {
  display: flex;
  flex-direction: row;
}
```

### Values

| Value            | Meaning                |
| ---------------- | ---------------------- |
| `row`            | left → right (default) |
| `row-reverse`    | right → left           |
| `column`         | top → bottom           |
| `column-reverse` | bottom → top           |

### Tailwind

| Tailwind           | CSS            |
| ------------------ | -------------- |
| `flex-row`         | row            |
| `flex-row-reverse` | row-reverse    |
| `flex-col`         | column         |
| `flex-col-reverse` | column-reverse |

Example:

```html
<div class="flex flex-col">
```

---

# 4. justify-content

Controls **alignment on the main axis**.

### CSS

```css
justify-content: center;
```

### Values

| Value           | Result                    |
| --------------- | ------------------------- |
| `flex-start`    | start                     |
| `flex-end`      | end                       |
| `center`        | center                    |
| `space-between` | equal space between items |
| `space-around`  | equal space around items  |
| `space-evenly`  | equal space everywhere    |

### Tailwind

| Tailwind          | CSS           |
| ----------------- | ------------- |
| `justify-start`   | flex-start    |
| `justify-end`     | flex-end      |
| `justify-center`  | center        |
| `justify-between` | space-between |
| `justify-around`  | space-around  |
| `justify-evenly`  | space-evenly  |

Example:

```html
<div class="flex justify-center">
```

---

# 5. align-items

Controls **alignment on the cross axis**.

### CSS

```css
align-items: center;
```

### Values

| Value        | Meaning       |
| ------------ | ------------- |
| `stretch`    | default       |
| `flex-start` | top           |
| `flex-end`   | bottom        |
| `center`     | middle        |
| `baseline`   | align by text |

### Tailwind

| Tailwind        | CSS        |
| --------------- | ---------- |
| `items-start`   | flex-start |
| `items-end`     | flex-end   |
| `items-center`  | center     |
| `items-stretch` | stretch    |

Example:

```html
<div class="flex items-center">
```

---

# 6. flex-wrap

Controls whether items **wrap to next line**.

### CSS

```css
flex-wrap: wrap;
```

### Values

| Value          | Meaning           |
| -------------- | ----------------- |
| `nowrap`       | default           |
| `wrap`         | wrap to next line |
| `wrap-reverse` | reverse wrap      |

### Tailwind

| Tailwind      | CSS    |
| ------------- | ------ |
| `flex-wrap`   | wrap   |
| `flex-nowrap` | nowrap |

Example:

```html
<div class="flex flex-wrap">
```

---

# 7. gap

Controls space **between items**.

### CSS

```css
gap: 20px;
```

### Tailwind

```
gap-2
gap-4
gap-8
```

Example:

```html
<div class="flex gap-4">
```

---

# 8. flex item properties

These apply to **child elements**.

### flex-grow

Allows items to grow.

```css
flex-grow: 1;
```

Tailwind:

```
grow
```

---

### flex-shrink

Controls shrinking.

```css
flex-shrink: 1;
```

Tailwind:

```
shrink
```

---

### flex-basis

Initial size.

```css
flex-basis: 200px;
```

Tailwind:

```
basis-1/2
basis-1/3
basis-full
```

---

# 9. Example Layout

### CSS Example

```css
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
```

### Tailwind Version

```html
<div class="flex flex-col justify-center items-center h-screen">
```

This means:

```
flex           → enable flexbox
flex-col       → vertical layout
justify-center → vertical center
items-center   → horizontal center
h-screen       → full screen height
```

---

# 10. Visual Example

Center a component in the screen:

```html
<div class="h-screen flex justify-center items-center">
  <button>Click</button>
</div>
```

Result:

```
        [ Button ]
     perfectly centered
```

---

# 11. Common Real-World Patterns

### Navbar

```html
<div class="flex justify-between items-center">
```

### Centered card

```html
<div class="flex justify-center items-center h-screen">
```

### Column layout

```html
<div class="flex flex-col gap-4">
```

---

✅ **Simple rule to remember**

```
flex → enable flexbox
flex-direction → layout direction
justify-content → main axis alignment
align-items → cross axis alignment
```

---

If you want, I can also explain **10 real flexbox patterns every React/Tailwind developer should know (with diagrams)**. It's extremely useful for frontend interviews.
