# Two complete worked learning examples

These are **original, fictional, hand-worked examples**, prepared for this Markdown guide. They are not real student outcomes, live AI runs or a claim about a provider’s model. They show what an explanation and test record can look like before a child chooses a tool.

## 1. A robot reaches a star on paper

Use a 4-column, 3-row grid. Start at (1,1), face right, and put a star at (4,3). The only commands are “move one square right” and “move one square up”.

| Step | Command | Position afterwards |
|---|---|---|
| Start | None | (1,1) |
| 1 | Right | (2,1) |
| 2 | Right | (3,1) |
| 3 | Right | (4,1) |
| 4 | Up | (4,2) |
| 5 | Up | (4,3), star reached |

The complete algorithm is **repeat Right 3 times, then repeat Up 2 times**. It uses five moves. If the star moves to (4,2), the last Up must be removed. Keeping it would move past the new target. This demonstrates sequence, repetition, prediction and a meaningful change. It is an original paper exercise inspired by general unplugged teaching, not a copied CS Unplugged lesson.

## 2. A tiny classifier can learn the wrong shortcut

Question: is an object a toy vehicle? Our fictional training set has two red toy cars labelled “vehicle” and two blue blocks labelled “not vehicle”. Imagine a learner chooses the shortcut **red → vehicle; anything else → not vehicle**. This rule is deliberately hand-written; no model was trained.

| Unseen test object | Correct label | Shortcut prediction | Correct? |
|---|---|---|---|
| Red toy bus | Vehicle | Vehicle | Yes |
| Blue toy car | Vehicle | Not vehicle | No |
| Red block | Not vehicle | Vehicle | No |
| Blue block | Not vehicle | Not vehicle | Yes |

The shortcut is correct on **2 of 4 tests (50%)**. It learned colour as a proxy for the target concept and failed on two counterexamples. Those four examples do not establish performance on all toys.

A better training set would include vehicles and non-vehicles in both colours, shapes and lighting conditions, with consistent labels. Reserve new examples for testing; do not call memorising the training items proof of generalisation. More balanced examples can help, but do not guarantee success. A child could use the same record format with a suitable provider learning activity, write down its real predictions, and compare outcomes honestly.

## Evidence a child could explain

“The paper robot needed three rights and two ups. When the target moved, I changed one command. The fictional classifier guessed from colour, so a blue car and a red block exposed its mistake. I would change the examples and test again.”

[AI resources](resources/ai.md) · [Learning paths](LEARNING-PATHS.md) · [How to recognise learning evidence](https://airbotix.ai/blog/four-pieces-of-evidence-child-learning-with-ai)
