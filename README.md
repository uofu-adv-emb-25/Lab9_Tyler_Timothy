# Lab 9 Verification



**Update Oct 14** the `ringing` column should be something like "time elapsed" to reflect the 10-second delay. That way, it is an event related to the `alarm_on` state of the world (instead of being redundant).

| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach | south_approach | north_depart | south_depart | ringing | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|----------------|----------------|--------------|--------------|---------|---------------|
| 0      | 0         | 0        | 0                  | 0                  |                |                |              |              |         |               |
| 1      | 0         | 0        | 0                  | 1                  |                |                |              |              |         |               |
| 2      | 0         | 0        | 1                  | 0                  |                |                |              |              |         |               |
| 3      | 0         | 0        | 1                  | 1                  |                |                |              |              |         |               |
| 4      | 0         | 1        | 0                  | 0                  |                |                |              |              |         |               |
| 5      | 0         | 1        | 0                  | 1                  |                |                |              |              |         |               |
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
| 16     |           |