From time to time I get baffled by `theirs` vs. `ours` durin the rebase conflicts. This PR is an excercise to figure it out.
https://stackoverflow.com/questions/25576415/what-is-the-precise-meaning-of-ours-and-theirs-in-git#25576672

# theirs-vs-ours

[Insert branches visualisation here]


# How their's vs. ours behave when rebasing 

1. switch to branch-b
2. `git rebase branch-a`

First conflict is unavoidable

```
$ git checkout --ours test.txt && cat test.txt 
Branch A change
git checkout --theirs test.txt && cat test.txt
Master change
```

Why is that?

(probably depending on branching strategies - explore that)
