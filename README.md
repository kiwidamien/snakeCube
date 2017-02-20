# snakeCube

An implementation of the snake on a "cube net" i.e. the flattened version of a piece of paper that you fold up to get a cube.

```
    -----
    |   |
----|---|--------
|   |   |   |   |
----|---|--------
    |   |
    -----
```

Does not include a timer to automatically move the snake forward. It is intended to help users understand the geometry of the cube. In particular, visualizing how the snake head changes direction as it moves between faces is quite challenging.


Inspired by the [snakeCube CodeFights problem](https://codefights.com/challenge/93CBnFa2vWyivpdHE).

Live version available at https://kiwidamien.github.io/snakeCube/

## Files

- __index.html__

  The main page that contains the app.

- __cubeBoard.js__

  Pure javascript (no ReactJS or UI interaction). Implements the board, and how the different cells are connected as an abstract data type. No coupling to UI.

- __snake_cube.js__

  (Todo: change name of this file)

  Depends on *cubeBoard.js* and ReactJS. Implements the components, and the layout for the page.

- __snake.css__  
   Style file for the webpage. Refers to the class names in *snake_cube.js* (i.e. the css and *snake_cube.js* are very tightly coupled).
