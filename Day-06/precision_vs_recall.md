# Precision vs Recall

| Precision                                    | Recall                                    |
| -------------------------------------------- | ----------------------------------------- |
| Measures correctness of positive predictions | Measures ability to find positive cases   |
| Formula: TP / (TP + FP)                      | Formula: TP / (TP + FN)                   |
| Focuses on False Positives                   | Focuses on False Negatives                |
| High Precision means fewer false alarms      | High Recall means fewer missed cases      |
| Important when false positives are costly    | Important when false negatives are costly |
| Used in Spam Detection                       | Used in Disease Detection                 |
| Improves quality of positive predictions     | Improves detection coverage               |
| May miss some actual positives               | May generate more false positives         |
| Precision increases when FP decreases        | Recall increases when FN decreases        |
| Often balanced using F1-Score                | Often balanced using F1-Score             |

## Trade-Off

Increasing Precision may decrease Recall.

Increasing Recall may decrease Precision.

The choice depends on the problem being solved.
