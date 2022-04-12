# Preact Offcanvas

> Preact component for adding a hidden sidebars to your project. Simply this is a Bootstrap 5 [Offcanvas](https://getbootstrap.com/docs/5.0/components/offcanvas/) component but without installing any dependencies.


## Usage

```jsx
import React from 'react'
import { OffcanvasProvider, Trigger, Offcanvas } from 'https://deno.land/x/preact_offcanvas'

export default function App() {
  return (
    <OffcanvasProvider { /* Provider props */ }>
      <Trigger { /* Trigger props */ } />
      <Offcanvas { /* Offcanvas props */ } />
    </OffcanvasProvider>
  )
}
```

<br />

## 1. Provider Props

| Prop      |   Type   | Options  | Description                                                            | Default |
| --------- | :------: | -------- | ---------------------------------------------------------------------- | :-----: |
| `onOpen`  | Function | Optional | Callback `function` that is triggered when the Offcanvas is **opened** |   `-`   |
| `onClose` | Function | Optional | Callback `function` that is triggered when the Offcanvas is **closed** |   `-`   |

<br />

## 2. Trigger Props

| Prop        |     Type      | Options  | Description                                  |       Default       |
| ----------- | :-----------: | -------- | -------------------------------------------- | :-----------------: |
| `component` |    String     | Optional | Render Component `button` \| `div`           |      `button`       |
| `className` |    String     | Optional | CSS className applied to the `Trigger Block` | `offcanvas-trigger` |
| `styles`    | CSSProperties | Optional | Inline style                                 |        `{}`         |
| `children`  |   ReactNode   | Optional | Component children                           |         `-`         |

<br />

## 3. Offcanvas Props

| Prop             |     Type      | Options  | Description                                      |          Default           |
| ---------------- | :-----------: | -------- | ------------------------------------------------ | :------------------------: |
| `title`          |    String     | Optional | Offcanvas Title (`h5` Tag)                       |     `Offcanvas Title`      |
| `position`       |    String     | Optional | `left` \| `right` \| `top` \| `bottom`           |          `right`           |
| `backdrop`       |    boolean    | Optional | Apply a backdrop on body while offcanvas is open |           `true`           |
| `allowClickAway` |    boolean    | Optional | Closes the offcanvas when user click outside     |           `true`           |
| `allowEsc`       |    boolean    | Optional | Closes the offcanvas when escape key is pressed  |           `true`           |
| `allowScroll`    |    boolean    | Optional | Allow body scrolling while offcanvas is open     |           `true`           |
| `className`      |    String     | Optional | CSS className applied to the `Offcanvas Block`   |     `simple-offcanvas`     |
| `styles`         | CSSProperties | Optional | Inline style                                     |            `{}`            |
| `children`       |   ReactNode   | Optional | Component Children                               | `Some text as placeholder` |

---

<br />
