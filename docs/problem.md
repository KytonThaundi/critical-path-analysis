# Problem Statement

## Activity Table

The project consists of the following activities and their relationships:

| Activity | Duration (days) | Preceding Activities |
|----------|----------------|---------------------|
| A | 15 | - |
| B | 5 | A |
| C | 6 | B |
| D | 3 | C |
| E | 5 | B |
| F | 10 | B |
| G | 3 | F |
| H | 2 | G, U |
| I | 1 | D, E, H |
| J | 2 | I |
| K | 10 | - |
| L | 10 | K |
| M | 5 | L, O |
| N | 2 | M, U |
| O | 5 | K |
| P | 6 | O |
| Q | 1 | O |
| R | 1 | N, P, Q |
| S | 2 | R |
| T | 10 | - |
| U | 8 | T |
| V | 5 | J, S |

## Initial Observations

1. There are three activities that can start immediately (no predecessors):
   - Activity A (15 days)
   - Activity K (10 days)
   - Activity T (10 days)

2. Complex convergence points exist at:
   - Activity H (requires completion of both G and U)
   - Activity I (requires completion of D, E, and H)
   - Activity R (requires completion of N, P, and Q)
   - Activity V (requires completion of J and S)

3. The project has multiple parallel paths that need to be analyzed to determine the critical path.