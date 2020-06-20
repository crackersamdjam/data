Andrew has a unique way to unlock his computer. To get in, he needs a password ~P~ of length ~3 \leq N \leq 2048~. To save time, Andrew has chosen ~P~ to be a **permutation** of the numbers ~1, 2, ..., N~. Unfortunately, ~N~ numbers can be a lot to remember. In order to help him in case he forgets, Andrew's computer returns him special hints. Each time, he can enter two integers ~i~ and ~j~ (~1 \leq i, j \leq N~, ~i \neq j~) and his computer will tell him the bitwise AND value of ~p_i~ and ~p_j~ (~p_i \& p_j~). Andrew figures that no one would be able to guess his password given so little information and just to be extra safe, he sets his computer to only give up to ~5120~ hints.

Are you able to get into Andrew's computer?


## Input and Output Specification

This is an interactive problem. In the first line, you will receive the integer ~N~.

Now, you may ask queries to the computer. To ask a query, print `? i j` to ask for the bitwise AND value of ~p_i~ and ~p_j~ (~p_i \& p_j~).

The judge will respond with the answer to your query, or `-1` if you exceeded the query limit. Exit immedietly after receiving `-1` or you will receive an arbitrary verdict.

To guess the answer, print `! p_1, p_2, ... p_n` and terminate your program. Note that answering does not count as one of the ~5120~ queries.

### Subtask 1 [30%]

~3 \leq N \leq 20~

### Subtask 2 [30%]

~N~ is ~1~ less than a power of ~2~ (e.g. ~3~, ~7~, ~15~, ...) and ~3 \leq N \leq 2048~.

### Subtask 3 [40%]

~3 \leq N \leq 2048~


## Sample Interaction

`>>>` denotes your output; don't actually print this out.

```
3
>>> ? 1 2
0
>>> ? 1 3
2
>>> ? 2 3
1
>>> ! 2 1 3
```

## Explanation for the Sample

The answer is `2 1 3`. The first query asks for ~p_1 \& p_2~ = ~2 \& 1~ = ~0~. The second query asks for ~p_1 \& p_3~ = ~2 \& 3~ = ~2~. The third query asks for ~p_2 \& p_3~ = ~1 \& 3~ = ~1~.


If you have a solution that consistely uses far fewer than ~5120~ queries, please leave a comment for the writer and testers. Thanks.

