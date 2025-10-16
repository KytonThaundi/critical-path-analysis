# Network Analysis

## Network Diagram

![Project Network Diagram](assets/network-diagram.svg)

*Project Network Diagram showing activities, dependencies, and critical path*

### Diagram Key Elements

1. **Nodes**: Each node represents an activity
   - Activity identifier (A, B, C, etc.)
   - Duration in days
   - Early Start (ES) and Early Finish (EF) times
   - Late Start (LS) and Late Finish (LF) times

2. **Arrows**: Show dependencies between activities
   - Direction indicates the flow of the project
   - No duration associated with dependencies (finish-to-start relationships)

3. **Critical Path** (highlighted in red):
   - A → B → F → G → H → I → J → V
   - Total duration: 43 days
   - Zero float activities

### Key Features

1. **Starting Activities** (no predecessors):
   - Activity A (15 days)
   - Activity K (10 days)
   - Activity T (10 days)

2. **Major Convergence Points**:
   - Node H: Requires completion of both paths through G and U
   - Node I: Merges paths from D, E, and H
   - Node R: Combines paths from N, P, and Q
   - Node V: Final activity, requiring both J and S

3. **Parallel Paths**:
   - Path through C-D: Parallel to E and F
   - Path through K-L-M: Parallel to K-O
   - Path T-U: Independent path feeding into H

## Network Structure

The network diagram can be broken down into several main paths:

### Path 1 (Starting with A)
```
A(15) → B(5) → splits into:
- C(6) → D(3)
- E(5)
- F(10) → G(3)
```

### Path 2 (Starting with K)
```
K(10) → splits into:
- L(10) → M(5)
- O(5) → splits into:
  - P(6)
  - Q(1)
```

### Path 3 (Starting with T)
```
T(10) → U(8)
```

## Early Start/Finish Calculations

### Starting Activities (ES = 0)
- A: ES=0, EF=15
- K: ES=0, EF=10
- T: ES=0, EF=10

### Following A
- B: ES=15, EF=20
- C: ES=20, EF=26
- D: ES=26, EF=29
- E: ES=20, EF=25
- F: ES=20, EF=30
- G: ES=30, EF=33

### Following K
- L: ES=10, EF=20
- O: ES=10, EF=15
- P: ES=15, EF=21
- Q: ES=15, EF=16

### Following T
- U: ES=10, EF=18

### Convergence Points
- H: ES=33, EF=35 (needs both G and U)
- I: ES=35, EF=36 (needs D, E, and H)
- J: ES=36, EF=38
- M: ES=20, EF=25 (needs L and O)
- N: ES=25, EF=27 (needs M and U)
- R: ES=27, EF=28 (needs N, P, Q)
- S: ES=28, EF=30
- V: ES=38, EF=43 (needs J and S)
