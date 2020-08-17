# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the hospital recorded the visitor trends during the week
  When the facility manager ask report
  Then report the visitor trends

Scenario: Alert when seating capacity is full

  Given the hospital as seating facility
  When seating capacity is filled
  Then alert and arrange for extra seating
