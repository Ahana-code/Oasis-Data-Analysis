FOR SUPERSTORE DATA CLEANING:
Highlights:
Cleaned and explored regional & category-wise performance
Built a summary dashboard to visualize insights

FOR CUSTOMER SEGMENTATION:
What we are doing here is creating a new column called Segment that consist of this:
| Annual Income | Spending Score | Result    |
| ------------- | -------------- | --------- |
| >70           | >60            | Premium   |
| >70           | <40            | Careful   |
| <40           | >60            | Target    |
| <40           | <40            | Low Value |
| All others    | Other values   | Mid-range |

> Formula for the above will be:
=IF(AND(D2>70, E2>60), "Premium",
 IF(AND(D2>70, E2<40), "Careful",
 IF(AND(D2<40, E2>60), "Target",
 IF(AND(D2<40, E2<40), "Low Value",
 "Mid-range"))))


> X-axis → Annual Income (k$)
> Y-axis → Spending Score (1–100)

> Colored dots for each segment:
🔴 Target
🔵 Premium
🟠 Low Value
🟢 Mid-range
🟣 Careful

FOR AUTOCORRECT AND AUTOCOMPLETE DATA ANALYSIS:-
>The main objective of this task is to:
Build and analyze Autocomplete (suggesting next word) and Autocorrect (fixing spelling mistakes) systems.
Use data analysis to evaluate the accuracy and performance of these systems.
Visualize how well your algorithms work.

>| Tool                        | Purpose                       |
| --------------------------- | ----------------------------- |
| Python                      | Programming language          |
| Jupyter Notebook or VS Code | Code writing environment      |
| pandas                      | Load and clean datasets       |
| nltk / re                   | NLP tools for preprocessing   |
| scikit-learn                | For model building (optional) |
| matplotlib/seaborn          | Visualizations                |

> Sample dataset:
text_data = [
    "I love natural language processing",
    "Natural language processing is a part of artificial intelligence",
    "Autocomplete makes typing faster",
    "Autocorrect fixes spelling mistakes automatically",
    "Machine learning helps with NLP tasks"
]







