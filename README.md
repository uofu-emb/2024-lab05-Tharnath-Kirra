# Invariants:
1. An approach signal will always precede a depart signal
2. Trains on each track only run in one direction.
3. Barrier will always be closed when train is going by


# Prove it.

| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach | south_approach | north_depart | south_depart | time_elapsed | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|----------------|----------------|--------------|--------------|--------------|---------------|
| 0      | 0         | 0        | 0                  | 0                  |0               |0               |0             |0             |1             |               |
| 1      | 0         | 0        | 0                  | 1                  |0               |1               |0             |0             |0             | 7             |
| 2      | 0         | 0        | 1                  | 0                  |1               |0               |0             |0             |0             |7              |
| 3      | 0         | 0        | 1                  | 1                  |1               |1               |0             |0             |0             |7              |
| 4      | 0         | 1        | 0                  | 0                  |0               |0               |1             |1             |0             |               |
| 5      | 0         | 1        | 0                  | 1                  |0               |0               |0             |0             |0             |               |
| 6      | 0         | 1        | 1                  | 0                  |0               |0               |0             |0             |0             |               |
| 7      | 0         | 1        | 1                  | 1                  |0               |0               |0             |0             |0             |               |
| 8      | 1         | 0        | 0                  | 0                  |0               |0               |0             |0             |0             |8              |
| 9      | 1         | 0        | 0                  | 1                  |0               |0               |0             |0             |0             |7              |
| 10     | 1         | 0        | 1                  | 0                  |0               |0               |0             |0             |0             |7              |
| 11     | 1         | 0        | 1                  | 1                  |0               |0               |0             |0             |0             |7              |
| 12     | 1         | 1        | 0                  | 0                  |0               |0               |0             |0             |0             |8              |
| 13     | 1         | 1        | 0                  | 1                  |0               |0               |0             |0             |1             |               |
| 14     | 1         | 1        | 1                  | 0                  |0               |0               |0             |0             |1             |               |
| 15     | 1         | 1        | 1                  | 1                  |0               |0               |0             |0             |1             |               |

| number | invariant |
|--------|-----------|
| 16     | 1         |
| 17     | 2         |
| 18     | 3         |
