# learn-tailwind-css
Listing **every single class in Tailwind CSS** would be **thousands of utilities**, because Tailwind generates many classes dynamically (like `p-1…p-96`, `bg-red-100…bg-red-900`, responsive variants, etc.).

Instead, the best way is a **complete categorized reference of all class types and what they mean**. This will cover essentially **everything you use in Tailwind**. 🚀

---

# 1. Layout Classes

| Class          | Meaning                          |
| -------------- | -------------------------------- |
| `container`    | Fixed width responsive container |
| `block`        | Display block                    |
| `inline-block` | Display inline-block             |
| `inline`       | Inline element                   |
| `hidden`       | Hide element                     |
| `flex`         | Enable flexbox                   |
| `inline-flex`  | Inline flexbox                   |
| `grid`         | Enable grid layout               |
| `inline-grid`  | Inline grid                      |

Example:

```html
<div class="flex">
```

---

# 2. Position

| Class      | Meaning              |
| ---------- | -------------------- |
| `static`   | Default position     |
| `relative` | Relative positioning |
| `absolute` | Absolute positioning |
| `fixed`    | Fixed to viewport    |
| `sticky`   | Sticky position      |

Position offsets:

```
top-0
top-1
right-0
bottom-0
left-0
```

---

# 3. Flexbox Utilities

| Class         | Meaning           |
| ------------- | ----------------- |
| `flex-row`    | Horizontal layout |
| `flex-col`    | Vertical layout   |
| `flex-wrap`   | Allow wrapping    |
| `flex-nowrap` | No wrap           |

Alignment:

```
justify-start
justify-center
justify-end
justify-between
justify-around
```

Vertical alignment:

```
items-start
items-center
items-end
items-baseline
items-stretch
```

Example:

```html
<div class="flex justify-center items-center">
```

---

# 4. Grid Classes

| Class          | Meaning    |
| -------------- | ---------- |
| `grid-cols-1`  | 1 column   |
| `grid-cols-2`  | 2 columns  |
| `grid-cols-3`  | 3 columns  |
| `grid-cols-12` | 12 columns |

Row classes:

```
grid-rows-1
grid-rows-2
grid-rows-6
```

Gap:

```
gap-1
gap-2
gap-4
gap-8
```

---

# 5. Spacing (Margin & Padding)

Padding:

```
p-0
p-1
p-2
p-4
p-8
p-10
```

Directional padding:

```
pt-4
pb-4
pl-4
pr-4
px-4
py-4
```

Margin:

```
m-4
mt-4
mb-4
ml-4
mr-4
mx-auto
```

Meaning example:

```
p-4 = padding 1rem
m-4 = margin 1rem
```

---

# 6. Width & Height

Width:

```
w-0
w-1
w-4
w-8
w-16
w-32
w-full
w-screen
```

Height:

```
h-4
h-8
h-16
h-32
h-screen
h-full
```

Example:

```html
<div class="w-full h-screen">
```

---

# 7. Typography

Font size:

```
text-xs
text-sm
text-base
text-lg
text-xl
text-2xl
text-3xl
text-4xl
text-5xl
```

Font weight:

```
font-thin
font-light
font-normal
font-medium
font-semibold
font-bold
font-black
```

Text alignment:

```
text-left
text-center
text-right
```

Line height:

```
leading-none
leading-tight
leading-normal
leading-loose
```

---

# 8. Colors

Background colors:

```
bg-red-500
bg-blue-500
bg-green-500
bg-gray-200
bg-black
bg-white
```

Text colors:

```
text-red-500
text-blue-500
text-green-500
```

Border colors:

```
border-red-500
border-blue-500
```

Color scale:

```
50
100
200
300
400
500
600
700
800
900
```

---

# 9. Borders

Border width:

```
border
border-2
border-4
border-8
```

Border radius:

```
rounded
rounded-sm
rounded-md
rounded-lg
rounded-xl
rounded-full
```

Example:

```html
<div class="border rounded-lg">
```

---

# 10. Shadows

```
shadow-sm
shadow
shadow-md
shadow-lg
shadow-xl
shadow-2xl
```

Example:

```html
<div class="shadow-lg">
```

---

# 11. Opacity

```
opacity-0
opacity-25
opacity-50
opacity-75
opacity-100
```

---

# 12. Hover Effects

```
hover:bg-blue-500
hover:text-white
hover:scale-110
hover:shadow-lg
```

Example:

```html
<button class="hover:bg-blue-500">
```

---

# 13. Responsive Design

Breakpoints:

| Prefix | Screen  |
| ------ | ------- |
| `sm:`  | ≥640px  |
| `md:`  | ≥768px  |
| `lg:`  | ≥1024px |
| `xl:`  | ≥1280px |
| `2xl:` | ≥1536px |

Example:

```html
<div class="text-sm md:text-lg lg:text-2xl">
```

---

# 14. Transform

```
scale-100
scale-110
rotate-45
rotate-90
translate-x-4
translate-y-4
```

Example:

```html
<div class="rotate-45">
```

---

# 15. Transition & Animation

Transition:

```
transition
duration-300
ease-in
ease-out
ease-in-out
```

Animation:

```
animate-spin
animate-ping
animate-pulse
animate-bounce
```

---

# 16. Z-index

```
z-0
z-10
z-20
z-30
z-40
z-50
```

---

# 17. Overflow

```
overflow-hidden
overflow-scroll
overflow-auto
```

---

# 18. Cursor

```
cursor-pointer
cursor-default
cursor-not-allowed
cursor-wait
```

---

# 19. Object Fit (Images)

```
object-contain
object-cover
object-fill
```

---

# 20. Dark Mode

```
dark:bg-black
dark:text-white
dark:border-gray-700
```

Example:

```html
<div class="bg-white dark:bg-black">
```

---

# Tools commonly used with Tailwind

Developers usually combine Tailwind with tools like:

* React
* Next.js
* Visual Studio Code

---

✅ **Summary**

Tailwind classes are grouped into these main categories:

1. Layout
2. Flexbox & Grid
3. Spacing
4. Typography
5. Colors
6. Borders
7. Effects
8. Transforms
9. Animations
10. Responsive design

Each category contains **scalable numeric utilities** (like `p-1` to `p-96`).

---

💡 If you want, I can also give you:

* **Complete Tailwind CSS cheat sheet (500+ classes)**
* **Tailwind full PDF guide**
* **Real project examples (Navbar + Dashboard + Landing page)**
* **Top 100 most used Tailwind classes developers use daily**.
