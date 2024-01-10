# star-rating

# Star Rating

Star Rating is a customizable React component for displaying and interacting with star ratings.

## Installation

This package is a React component, so you need to have React installed in your project. If you haven't already installed React, you can do so with the following command:

```bash
npm install react react-dom

npm install starsss
```

## API Reference

### `<StarRating />`

A React component for displaying a star rating.

#### Props

- `color` (String): The color of the stars. Default is "#fcc419".
- `size` (Number): The size of the stars. Default is 24.
- `defaultRating` (Number): The default rating. Default is 0.
- `maxRating` (Number): The maximum rating. Default is 10.
- `onSetRating` (Function): A callback function that is called when the rating is set. It receives the new rating as its argument.

#### Usage

```jsx

<StarRating />

<StarRating  maxRating = 5,
  color = "#fcc419",
  size = 48,
  className = "",
  defaultRating = 0,
  message = []
  />
```

```jsx
import { useState } from "react";
import StarRating from "starsss";

function Test() {
  const [rating, setRating] = useState(0);

  return (
    <div>
      <StarRating
        color="#fcc419"
        size={24}
        defaultRating={0}
        maxRating={10}
        onSetRating={setRating}
      />
      <p>awarded {rating}</p>
    </div>
  );
}
```

# License

This project is licensed under the MIT License
