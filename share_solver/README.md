## The Problem description

You get the size of two server groups and a desired target for group A in percent (`0` - `100`).
How should you choose the weights for each individual server of a group (each server of a group has to have the same weight),
that the combined weights of grooup A are the percentage of the combined weights of all groups.

* The weight have to be integers between `0` and `255`.
* You should return the solution with the lowest values if there are multiple solutions possible.
* You should return the solution with lowest error if there are no perfect solutions.

Example:

```
group_a_size = 2
group_b_size = 4
target = 50
```

Solution: `2,1`

```
server, weigth
A1      2
A2      2
B1      1
B2      1
B3      1
B4      1
---------------
total   8
```

The weight of all `A` servers is `4` which is `50` of the total way.


## How to run the tests

```bash
pipenv install --dev
pytest .
```
## How to add a new Solution

Copy the `soultion_template.py` to `<nick>_solution.py` and fill the function.
