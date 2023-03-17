# Table Challenge

A client-side javascript game for practicing multiplication tables. You can checkout the current default version at [https://cagedev.github.io/table-challenge/](https://cagedev.github.io/table-challenge/).

## Configuration

### Assignments

The assignments may be configured either as an array of arrays containing the assignment instructions and the results as a pair

```javascript
const assignments = [
    ['1 x 3 =', 1 * 3],
    ['2 x 3 =', 2 * 3],
    ['3 x 3 =', 3 * 3],
    ['4 x 3 =', 4 * 3],
    ['5 x 3 =', 5 * 3],
    ['6 x 3 =', 6 * 3],
    ['7 x 3 =', 7 * 3],
]
```

or as a number of parameters

```javascript
    const tables = [1, 2, 3, 4, 5, 6, 10]; // available tables
    const min = 0; // minimum multiple in the table
    const max = 10; // maximum multiple in the table
```

in which case the assignments are generated randomly.

### Difficulty

Difficulty can be adjusted by editing the following settings

```javascript
    const maxLives = 5; // Maxumim lives available (integer)
    const winCondition = 10; // Number of points required to win (Number)
    const timerDelta = 5000; // Time (in ms) per question (integer)
    const pointsDelta = 1; // Number of points gained per correct answer (Number)
    const livesDelta = -1; // Number of lives lost per incorrect answer (integer)
```

## Notes

Currently the games starts as soon as the page loads and data is not saved.