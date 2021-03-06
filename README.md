# Single Updates on a Virtualized Grid

To run the project:

```sh
yarn dev
```

Then navigate to `http://localhost:3000`.

## Cortex

Cortex is a messaging queue that passes updated cell values to each cell.

This implementation uses Context and `useRef`.
Another implementation might use the event emitter API.

## PlainGrid

Regular implementation of a virtualized grid and updates on it's data.
Every time data updates, the entire table must re-render.

## MyGrid

Virtualized grid implementation using Cortex to do single updates on individual cells without re-rendering the entire table.
