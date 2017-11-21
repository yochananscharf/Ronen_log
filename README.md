# Ronen_log

## Assumptions

1. The first line of each event is relevant for understanding event type. Subsequent line that can go on for scores of lines are irrelevant. This assumption can be completely wrong. Please update me if this is the case.
2. I understood the project name and branch name to be int the format of  " [ project_name] - Branch-name". Found less then 1000 lines containing this format.
3. The group-by output  reflects my understanding of  "number of events per day per project per branch". Please correct me if I misunderstood.

## Fixed the parsing to split on time-stamp.
the lines containing the following pattern

+++++++++++++++
+Application started.....
+++++++++++++

are appended to the last event (except for the first occurrence).
