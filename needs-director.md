# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the hospital allows visitor
  When visitor enter the hospital
  Then count the number of visitors

Scenario: Compute parking slots to reserve for visiting specialists

  Given the hospital as parking facility
  When parking slots are going to filled up
  Then reserve the slots for visiting specialists
