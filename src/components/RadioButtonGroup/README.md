# RadioButtonGroup

RadioButtonGroup allow you to add group radiobutton

### Usage

```js
import { RadioButtonGroup } from "app-components";
```

```jsx
<RadioButtonGroup
  name="fruits"
  selected="banana"
  options={[
    { value: "apple", label: "Sweet apple" },
    { value: "banana", label: "Banana" },
    { value: "Mandarin" }
  ]}
/>
```

### Properties

| Props         |   Type    | Required |          Values          |   Default    | Description                                                                                                                                                                                                       |
| ------------- | :-------: | :------: | :----------------------: | :----------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `name`        | `string`  |    ✅    |            -             |      -       | Used as HTML `name` property for `<input>` tag. Used for identification RadioButtonGroup                                                                                                                          |
| `options`     | `arrayOf` |    ✅    |            -             |      -       | Array of objects, contains props for each `<RadioButton />` component                                                                                                                                             |
| `selected`    | `string`  |    ✅    |            -             |      -       | Value of the selected radiobutton                                                                                                                                                                                 |
| `onClick`     |  `func`   |    -     |            -             |      -       | Allow you to handle clicking events on `<RadioButton />` component                                                                                                                                                |
| `orientation` |  `oneOf`  |    -     | `vertical`, `horizontal` | `horizontal` | Position of radiobuttons                                                                                                                                                                                          |
| `disabled`    |  `bool`   |    -     |            -             |   `false`    | Disabling all radiobutton in group                                                                                                                                                                                |
| `spacing`     | `string`  |    -     |            -             |    `15px`    | Margin between radiobutton. If orientation `horizontal`, it is `margin-left`(apply for all radiobuttons, except first), if orientation `vertical`, it is `margin-bottom`(apply for all radiobuttons, except last) |
| `width`       | `string`  |    -     |            -             |    `100%`    | Width of RadioButtonGroup container                                                                                                                                                                               |
