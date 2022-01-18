# Tailwind CSS essentials

[Tailwind CSS Tutorial for Beginners - Full Course](https://www.youtube.com/watch?v=4wGmylafgM4)

## Color

`.bg-{color}-{shade}`

|              `color`               |  `shade`  |
| ---------------------------------- | --------- |
| black, white                       | -         |
| gray, red, orange, yellow, green, | 100 - 900 |
| teal, indigo, blue, purple, pink   |           |

## Element sizing with rem

> 4 = 1 rem = 16px

1 rem = 4 in Tailwind

1 rem = document base font size = 16px in most browsers

* 1 = 0.25rem =  4px
* 2 = 0.50rem =  8px
* 3 = 0.75rem = 12px
* 4 = 1rem    = 16px
* 5 = 1.25rem = 20px
* 6 = 1.50rem = 24px

## Width & Height

`.{w|h}-{size}`

| `size` - explicit size |     |
| ---------------------- | --- |
| 0, 1, 2, 3, 4, 5, 6,   | +1  |
| 8, 10, 12,             | +2  |
| 16, 20, 24,            | +4  |
| 32, 40, 48, 56, 64     | +8  |

| `size` - fraction  |                                |
| ------------------ | ------------------------------ |
| 1/2                | Percentage of parent container |
| 1/{3, 4, 5, 6, 12} | Every number in numerator      |

| `size` - screen and full |                          |
| ------------------------ | ------------------------ |
| screen                   | 100% of screen           |
| full                     | 100% of parent container |

## Padding & Margin

`.{p|m}-{size}`
`.{p|m{l|r|t|b}}-{size}`
`.{p|m{x|y}}-{size}`

|        `size`        |     |
| -------------------- | --- |
| 0, 1, 2, 3, 4, 5, 6, | +1  |
| 8, 10, 12,           | +2  |
| 16, 20, 24,          | +4  |
| 32, 40, 48, 56, 64   | +8  |

## Text styling

### Font Family

`.font-{family}`

| `family` |                            |
| -------- | -------------------------- |
| sans     | Helvetica or similar       |
| serif    | Times New Roman or similar |
| mono     | Monospace or similar       |

> Best practice: put font family on top-most element (e.g. `<body>`)

### Text size

`.text-{size}`

| `size` |    rem    | pixels |
| ------ | --------- | ------ |
| xs     | 0.75 rem  | 12px   |
| sm     | 0.875 rem | 14px   |
| base   | 1 rem     | 16px   |
| lg     | 1.125 rem | 18px   |
| xl     | 1.25 rem  | 20px   |
| 2xl    | 1.5 rem   | 24px   |
| 3xl    | 1.875 rem | 30px   |
| 4xl    | 2.25 rem  | 36px   |
| 5xl    | 3 rem     | 48px   |
| 6xl    | 4 rem     | 64px   |

### Text align

`.text-{align}`

| `align` |     |
| ------- | --- |
| left    |     |
| center  |     |
| right   |     |
| justify |     |

### Text color

`.text-{color}-{shade}`

|              `color`               |  `shade`  |
| ---------------------------------- | --------- |
| black, white                       | -         |
| gray, red, orange, yellow, green, | 100 - 900 |
| teal, indigo, blue, purple, pink   |           |

> Best practice: put text color on top-most element (e.g. `<body class="text-gray-900">`)

### Italics

`.{italic|not-italic}`

### Font weight

`.font-{weight}`

|  `wight`  | Font Weight |
| --------- | ----------- |
| hairline  | 100         |
| thin      | 200         |
| light     | 300         |
| normal    | 400         |
| medium    | 500         |
| semibold  | 600         |
| bold      | 700         |
| extrabold | 800         |
| black     | 900         |

### Letter spacing

> Letter spacing is in em not rem:
>
> * em: parent element's font size
> * rem: base document font size

`.tracking-{spacing}`

| `spacing` | Letter spacing |
| --------- | -------------- |
| tighter   | -0.05 em       |
| tight     | -0.025 em      |
| normal    | 0              |
| wide      | 0.025 em       |
| wider     | 0.05 em        |
| widest    | 0.1 em         |

### Line height

`.leading-{height}`

| `height` | line height |
| -------- | ----------- |
| none     | 1           |
| tight    | 1.25        |
| snug     | 1.375       |
| normal   | 1.5         |
| relaxed  | 1.625       |
| loose    | 2           |

### Text decorations

`.{underline|no-underline|line-through}`

### Text transform

`.{uppercase|lowercase|capitalize|normal-case}`

`.normalcase` will undo any of the other transformations.

## Borders and Radiuses

### Border thickness

`.border-{thickness}`

| `thickness` |     |
| ----------- | --- |
| 0           | 0px |
| [empty]     | 1px |
| 2           | 2px |
| 4           | 4px |
| 8           | 8px |

### Border sides

`.border-{side}-{thickness}`

|   `side`   | `thickness` | pixels |
| ---------- | ----------- | ------ |
| t, b, l, r | 0           | 0px    |
|            | [empty]     | 1px    |
|            | 2           | 2px    |
|            | 4           | 4px    |
|            | 8           | 8px    |

#### Border color

`.border-{color}-{shade}`

|              `color`               |  `shade`  |
| ---------------------------------- | --------- |
| black, white                       | -         |
| gray, red, orange, yellow, green, | 100 - 900 |
| teal, indigo, blue, purple, pink   |           |

### Border styles

`.border-{style}`

| `style` |     |
| ------- | --- |
| solid   |     |
| dashed  |     |
| dotted  |     |
| double  |     |
| none    |     |

### Border radius

`.rounded-{radius}`

| `radius` |   rems    | pixels |
| -------- | --------- | ------ |
| sm       | 0.125 rem | 2px    |
| [empty]  | 0.25 rem  | 4px    |
| lg       | 0.5 rem   | 8px    |
| full     | -         | 9999px |
| none     | 0         | 0px    |

### Border radius sides

`.rounded-{side}-{radius}`

| `side` |                            |
| ------ | -------------------------- |
| t      | top-left & top-right       |
| r      | top-right & bottom-right   |
| b      | bottom-left & bottom-right |
| l      | top-left & bottom-left     |
| tl     | top-left                   |
| tr     | top-right                  |
| br     | bottom-right               |
| bl     | bottom-left                |

## Flex

### Flexbox alignment on the main axis

`.justify-{alignment}`

| `alignment` |         |
| ----------- | ------- |
| start       | Default |
| center      |         |
| end         |         |
| between     |         |
| around      |         |

### Flexbox alignment on the secondary axis

`.items-{alignment}`

| `alignment` |                          |
| ----------- | ------------------------ |
| stretch     | Default - fill container |
| start       |                          |
| center      |                          |
| end         |                          |
| baseline    |                          |

### Flexbox direction

`.flex-{direction}`

| `direction` |         |
| ----------- | ------- |
| row         | Default |
| row-reverse |         |
| col         |         |
| col-reverse |         |

### Flexbox wrap

`.flex-{wrap}`

| `direction`  |         |
| ------------ | ------- |
| no-wrap      | Default |
| wrap         |         |
| wrap-reverse |         |

## Responsive design

`{breakpoint}:{class}`

| `breakpoint` | Starts at |
| ------------ | --------- |
| [all]        | 0px       |
| sm           | 640px     |
| md           | 768px     |
| lg           | 1024px    |
| xl           | 1280px    |

|     Responsive Classes       |                                               |
| --------------------------   | --------------------------------------------- |
| `.sm:bg-*`                   | background color                              |
| `.sm:w-*`                    | width                                         |
| `.sm:h-*`                    | height                                        |
| `.sm:p-*`                    | padding                                       |
| `.sm:m-*`                    | margin                                        |
| `.sm:font-sans`              | font family - sans, serif, mono               |
| `.sm:text-lg`                | font size - xs, sm, base, lg, xl, {2-6}xl     |
| `.sm:text-left`              | text alignment - left, center, right, justify |
| `.sm:text-{color}-{shade}`   | text color                                    |
| `.sm:font-bold`              | font weight                                   |
| `.sm:tracking-tighter`       | letter spacing                                |
| `.sm:leading-tight`          | line spacing                                  |
| `.sm:uppercase`              | text transform                                |
| `.sm:border-{color}-{shade}` | border color                                  |
| `.sm:border-{style}`         | border style                                  |
| `.sm:border-{width}`         | border width                                  |
| `.sm:rounded-{size}`         | border radius                                 |
| `.sm:{display}`              | block, inline, flex, hidden, ...              |
| `.sm:flex`                   | display flex                                  |
| `.sm:flex-{col|row}`         | flex direction                                |

> Classes that are stackable cascade, i.e. at medium size or larger, the following apply both: `sm:font-bold md:italic`

## Other modifiers

`.hover:{class}`

`.focus:{class}`

|         Hover classes                 |                  |
| ------------------------------------- | ---------------- |
| .{hover|focus}:bg-*                   | background color |
| .{hover|focus}:text-{color}-{shade}   | text color       |
| .{hover|focus}:font-bold              | font weight      |
| .{hover|focus}:border-{color}-{shade} | border color     |

## Combination modifiers

`.md:hover:{class}`

## Other utilities

`.shadow-{size}`

| `size`  |     |
| ------- | --- |
| md      |     |
| lg      |     |
| xl      |     |
| 2xl     |     |
| inner   |     |
| outline |     |
| none    |     |

`.opacity-{percent}`

| `percent` |     |
| --------- | --- |
| 100       |     |
| 75        |     |
| 50        |     |
| 25        |     |
| 0         |     |

`.cursor-{style}`

|   `style`   |     |
| ----------- | --- |
| default     |     |
| pointer     |     |
| wait        |     |
| text        |     |
| move        |     |
| not-allowed |     |

`.select-{style}`

| `style` |     |
| ------- | --- |
| none    |     |
| text    |     |
| all     |     |
| auto    |     |

`.{sr-only|non-sr-only}`

`sr`: Screen Reader
