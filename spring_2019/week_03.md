## Last Week's Accomplishments

Last week Josh and I began experimenting with different node serial-communication libraries.
We settled on using SerialPort since it makes good use of Node.js's event loop.

## This Week's Plan

I'd like to get some more concrete API implementation this week. I need to decide how to implement the commands
in a robust way that hopefully makes use of dynamic programming or polymorphism.

I think it would be most appropriate to hard-code, but I am concerned about potential future updates.
However, the way we structure our library with Lerna.js could aid in a future firmware-specific impl.

## Anything Blocking?

Josh and I need to sit down and try and wrap our head's around the documentation we've received.

## Notes

N/A
