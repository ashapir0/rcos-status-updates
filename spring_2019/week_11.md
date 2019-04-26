## Last Week's Accomplishments

Last week I produced a frontend demonstration showing how our library can easily be hooked into other applications.
I did this over socket.io which was fairly easy, however parsing out the data proved more challenging.

## Semester Wrap-Up
Over the course of the last semester I've learned a lot about hardware.  As a full-stack web developer I've never had the opportunity to integrate the technologies I know with low-level serial communication.  This presented a number of unique challenges that were fun to address.  In hindsight, I wish we recruited more developers to work on the project as the scope of the specifications for Whistler proved to be too large for Josh and myself.

Starting with our experimentation repository, Josh and I worked dilligently to get a proof-of-concept going in less than a month.  Choosing an underlying serial library was challenging because the benefits and drawbacks of each option are hard to quantify in terms of our unique use-case upfront.  However, I am generally confident that we made the right choice (SerialPort)[https://serialport.io/].  This library is platform agnostic and makes use of Node's event loop well (by using event-emitters).

Using an event-emitter based library - while incredibly performant - makes it tough to integrate a linear control-flow controller (outlined our goals).  My initial approach worked but caused a listener-based memory leak (these are hard to address in Node).  However a callback based implementation seems to have solved this (although the internal flow is a bit more challenging to follow).  In the future, I'd like to implement a cleaner solution.
