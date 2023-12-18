# Classifying-Bug-Types
## Abstract
### Context 
In software engineering, classifying bugs can be a
matter of great significance. It not only helps developers better
manage projects and analyze the maintenance process, but today,
many Automated Program Repair tools rely on bug classification.

### Objective
Performing an Abstract Syntax Tree (AST) algorithm
to classify bugs has drawbacks. AST algorithms are expensive and
sometimes fail to determine bug types even in low granularities
in terms of computation. By training Deep Learning models that
can alternatively perform the same task, we aim to considerably
decrease this cost in the long term.

### Method
Our aim is to classify bug fix patterns based on
their repair diff files and corresponding commit messages. To
solve this problem, we employed a pre-trained Bidirectional
Encoder Representations from Transformers (BERT) model for
natural language processing for commit messages and source
code processing for diff files. The taxonomy used is based on
single-statement bug fixes (SStuBs).

### Results After conducting experiments with BERT model, the
final evaluations demonstrate that the model has succeeded in
classifying 67% of single statement bugs (TSSB-3M dataset [13]).

### Conclusion 
The results show that the model trained solely
on Diffs can be a noble alternative to costly AST algorithms
when classifying vast datasets of bug fixes. However, it needs
adjustments to be useful in practice. The models trained on
Commit messages also showed promising potential for our goals.
The work introduces a thriving baseline, indicating significant
potential for future applications.

### Index Terms
Bug Classification, Bug Characterization, Fix
Patterns Taxonomy, Bug Reports, Deep Learning

## Code Notebooks Used
### Diff Only Model
https://colab.research.google.com/drive/15xfE9fUjuHG91VUiQoL60afztOGdjNHR?usp=sharing

### Commit Only Model
https://colab.research.google.com/drive/1Q422oau7DlvMkT243Gld0Fw6OBNN7ttD?usp=sharing

### Diff & Commit Model
https://colab.research.google.com/drive/1VhFG735y6Y809H5u9FhrqAxS_0FcqpWQ?usp=sharing


