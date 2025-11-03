# Lab 9 Verification



**Update Oct 14** the `ringing` column should be something like "time elapsed" to reflect the 10-second delay. That way, it is an event related to the `alarm_on` state of the world (instead of being redundant).

| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach | south_approach | north_depart | south_depart | timer_elasped | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|----------------|----------------|--------------|--------------|---------|---------------|
| 0      | 0         | 0        | 0                  | 0                  | 6               | 5               | 17             | 17             | 0        |               |
| 1      | 0         | 0        | 0                  | 1                  |                |                |              |              |         | 20              |
| 2      | 0         | 0        | 1                  | 0                  |                |                |              |              |         | 20              |
| 3      | 0         | 0        | 1                  | 1                  |                |                |              |              |         | 20              |
| 4      | 0         | 1        | 0                  | 0                  |                |                |              |              |         | 20              |
| 5      | 0         | 1        | 0                  | 1                  | 7               | 23               | 17             | 0             | 5        |               |
| 6      | 0         | 1        | 1                  | 0                  |                |                |              |              |         |               |
| 7      | 0         | 1        | 1                  | 1                  |                |                |              |              |         |               |
| 8      | 1         | 0        | 0                  | 0                  |                |                |              |              |         |               |
| 9      | 1         | 0        | 0                  | 1                  |                |                |              |              |         |               |
| 10     | 1         | 0        | 1                  | 0                  |                |                |              |              |         |               |
| 11     | 1         | 0        | 1                  | 1                  |                |                |              |              |         |               |
| 12     | 1         | 1        | 0                  | 0                  |                |                |              |              |         |               |
| 13     | 1         | 1        | 0                  | 1                  |                |                |              |              |         |               |
| 14     | 1         | 1        | 1                  | 0                  |                |                |              |              |         |               |
| 15     | 1         | 1        | 1                  | 1                  |                |                |              |              |         |               |

| number | invariant |
|--------|-----------|
| 16     | Alarm always preceeds the arms lowering          |
| 17     | The approach signal always activates before the departure signal (for a single direction)         |
| 18     | Arms always lower before the train passes         |
| 19     | Arms lowering time is consistent         |
| 20     | Alarm is always on when the train is present         |
| 21     | Power is never interrupted         |
| 22     | Weather will never damage the equipment         |
| 23     | Only one train can be present at a time (for a single direction)         |
