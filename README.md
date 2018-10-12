# Stencil Fragment

This single line of code adds the same functionality as React.Fragment to your StencilJS app.

The purpose of Fragment is to allow rendering multiple sibling elements without the need to return an array in your render function.

Essentially, Fragment is an "empty element" which can hold child elements without itself being rendered to the DOM. This avoids needless `<div>` wrappers and arrays.

## Usage

```
npm i stencil-fragment
```

```tsx
import Fragment from 'stencil-fragment'

render() {
  return (
    <Fragment>
      <div>First element...</div>
      <div>Second element...</div>
      <div>Another element...</div>
    </Fragment>
  )
}
```