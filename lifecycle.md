# Lifycycle

```mermaid
stateDiagram-v2
  Initial: Initial Stage
  Growth: Growth Event
  Evolution: Stable Evolution
  Stale: Reduced Activity
  Challenge: Challenge Event
  Initial --> Growth
  Initial --> Complete
  Initial --> Challenge
  Growth --> Evolution: New Resoruces
  Growth --> Challenge
  Evolution --> Complete
  Evolution --> Challenge
  Challenge --> Evolution
  Challenge --> Stale
  state Stale {
    Maintenance
    Fallow
    Abandoned
  }
  Stale --> Complete: Sunset
  Stale --> Growth: Reactivation
```

