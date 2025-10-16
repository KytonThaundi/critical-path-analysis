# Critical Path Calculation

## Critical Path Identification

The critical path is determined by identifying the sequence of activities that has:
1. The longest duration through the network
2. Zero total float (slack)

### Critical Path Activities

The critical path follows the sequence:
```
A → B → F → G → H → I → J → V
```

### Duration Breakdown

1. Activity A: 15 days
2. Activity B: 5 days
3. Activity F: 10 days
4. Activity G: 3 days
5. Activity H: 2 days
6. Activity I: 1 day
7. Activity J: 2 days
8. Activity V: 5 days

Total Duration: 43 days

## Float Analysis

Activities not on the critical path have float (slack time). Some key float calculations:

1. Path through C-D:
   - Float = 7 days
   
2. Path through E:
   - Float = 10 days
   
3. Path through K-L-M:
   - Float = 16 days
   
4. Path through K-O-P:
   - Float = 17 days
   
5. Path through T-U:
   - Float = 15 days

Activities on the critical path have zero float, meaning any delay in these activities will directly impact the project completion date.