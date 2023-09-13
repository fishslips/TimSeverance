## Day 2

| Argument |
| --- |
| ¬q <br> p → q  |
| ∴ ¬p |

The Conjunction of the hypothesis implies the conclusion

In other words ((p -> q) ^ !q) -> !p

When we talked about conditional operations, we discussed the fact that p -> q has p as the hypothesis, and q as the conclusion.

In an argument, we have a few hypotheses, and then a conclusion. So in other words, an argument is the conjunction of a few hypotheses or propositions followed by a final proposition or conclusion.

Whenever there are rows where all of the arguments in a truth table are true, the argument is valid when the conclusion is also true for those rows, and invalid if the conclusion is false for those rows.

| Argument |
| --- |
| p V q <br> p|
| ∴ ¬q |

| p | q | p V q | ¬q |
| --- | --- | --- | --- |
| T | T | T | F |
| T | F | T | T |
| F | T | T | F |
| F | F | F | T |

Rows 1 and 2 of the truth table for the hypotheses in the argument yield true. However, row 1 has a false conclusion. Since there is an instance where the hypotheses are true, but the conclusion is false, the entire argument is false, despite there being an instance where the hypotheses are true with a true conclusion.

When p and q are true, the argument is false.

In order to prove that an argument is invalid, you HAVE to have an instance where the hypotheses are all true. There are a few questions that ask about whether or not the propositions show that an argument is invalid, but in order to prove whether or not an argument is invalid, you have to show that the hypotheses can first be true, but that the resulting conclusion is false. When we're talking about validity, we're talking about arguments with grounds for reason. Arguments that have baseless or truth-less hypotheses are not even considered to be arguments basically.

