## Configuring Time Unit and Precision

Like SystemVerilog, Vlang has a concept of time precision and a time unit. A user may define a time precision and a time unit for each entity(hiearchical unit) in Vlang.

```d
override void doConfig() {
  timeUnit = 100.psec;
  timePrecision = 10.psec;
}
```

At the time of elaborating the design, Vlang looks hierarchically for the precision configured for each entity and uses the least of whatever values it comes across. For the timeUnit, Vlang uses the value configured for a given entity. If no value is configured for a given entity, the instances of such entity would inherit the timeUnit being used for the parent entity.


## Specifying Time in Vlang

There are two value types in Vlang, *Time* and *SimTime*. SimTime is just an integral number of simulation steps. The type *Time* stores both an integral number and a time unit to go with that number. Internally, a Vlang simultor converts all Time values to SimTime, by dividing the Time value by timePrecision.

Vlang provides a convenient syntax for specifying Time. For example a user may just say:

```d
  wait(10.nsec);
```

Alternatively, the end-user may just provide an integer to specify time. When that is done, Vlang would scale that number with the timeUnit associated with the object to which the time is being passed. For example:

```d
  alu.pipe.doneEvent.notify(4);
```

Here the doneEvent object in alu.pipe hierarchy would get notified in 4 timeUnits, and the timeUnit associated with alu.pipe would apply.

