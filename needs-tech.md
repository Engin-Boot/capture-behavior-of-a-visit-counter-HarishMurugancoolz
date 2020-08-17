# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the server as checkpoints on visit counter facility
  When server restarts
  Then recover the data from the checkpoint

Scenario: Reconcile counts if the sensor is offline for a while

  Given the facility as a sensor for visit counter
  When sensor is offline
  Then reconcile the counts when it is online
