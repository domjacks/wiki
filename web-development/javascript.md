# Javascript

## Event Loop

See ["What the heck is the event loop anyway?"](https://www.youtube.com/watch?v=8aGhZQkoFbQ) and [In the loop](https://www.youtube.com/watch?v=cCOL7MC4Pl0) for an in-depth view of the JS event loop.

## Synchronous vs Asynchronous

Javascript is _synchronous_. However, when used in a browser or Node context for example, it can use APIs available which are called asynchronous. This means, it doesn't, by default, wait for a response from those calls to the APIs.

### Browser APIs

Some examples of the APIs and Objects that a browser provides that we use in our day-to-day:

- `fetch`
- `XMLHttpRequest`
- `setTimeout`
- `Events`
- `DOM`
- `CSSOM`