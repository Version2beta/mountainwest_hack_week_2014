# Full stack error handling

Jamund Ferguson, was at oDesk, now PayPal, @xjamundx

Best practices:

* Catches
* Callbacks
* Custom errors
* Conventions

## try-catch

Best for JSON.parse. Other than that, not much use in node.js.

Any time I see someone throwing an error in a node app, I assume they're doing it wrong.

## callbacks

Pass in a callback that returns (err, data).

Error object gives you a stack trace.

## custom errors

```
function CustomError(message) {
    ...
}
CustomError.prototype = Object.create(Error.prototype);
```

## conventions

* Always deal in `Error` objects.
* `cb(err)` and `next(err)` and then immediately return.
* `process.on('uncaughtException')` must always `process.exit()`.
* Consider a helper function and creating a standard schema for sending errors to the client.
* log *every* error including client side error.
* Throw only if you can't do anything else.


