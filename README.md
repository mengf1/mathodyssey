# A Dataset for MathOdyssey


The [anonymous] Math 2024 presents a collection of 387 meticulously crafted math problems, meticulously curated by professional math problem writers from both universities and high schools. The compilation includes high school competition questions with 148 problems, followed by a series of 138 high school mathematics questions, and concluding with 101 university-level mathematics questions. 

The [anonymous] Math 2024 problem setters are composed of mathematics professors hailing from esteemed institutions such as [anonymous]. These professors were formally invited by [anonymous] to contribute their expertise to the competition. The problem setter committee aligned with the mission of [anonymous], which aims to advance innovative research in artificial general intelligence (AGI) and foster interdisciplinary collaboration, and ensure that AGI development benefits humanity as a whole. To maintain the integrity and fairness of the competition, the problem setter committee ensured that all problems were original and kept confidential. Responsibilities of the problem setter committee included problem generation, review, formatting, testing, and revisions for GAIC Math 2024.


A new dataset of 387 questions and solutions from high school competition questions, high school mathematics questions, and university-level mathematics questions.


| ID |  Level                                     | Label                                              | Number   | 
|----|-------------------------------------------|----------------------------------------------------|----------|
| 1  | high school competition                   | Algebra                                            | 82       | 
| 2  | high school competition                   | NumberTheory                                       | 4        | 
| 3  | high school competition                   | Geometry                                           | 25       | 
| 4  | high school competition                   | Combinatorics                                      | 37       | 
| 5  | high school mathematics questions         | Algebra                                            | 69       | 
| 6  | high school mathematics questions         | Geometry                                           | 14       | 
| 7  | high school mathematics questions         | PreCalculus                                        | 47       | 
| 8  | high school mathematics questions         | Trigonometry                                       | 2        | 
| 9  | high school mathematics questions         | Calculus                                           | 5        | 
| 10 | high school mathematics questions         | Series                                             | 1        | 
| 11 | university-level                          | Linear Algebra and Abstract Algebra                | 25       | 
| 12 | university-level                          | Calculus and Analysis                              | 24       | 
| 13 | university-level                          | Differential Equations                             | 14       | 
| 14 | university-level                          | Probability                                        | 21       | 
| 15 | university-level                          | Statistics                                         | 17       | 

## Evaluation Baseline

Evaluation Results of Odyssey-Math dataset across different models.
![table_from_paper](./docs/benchmark-new.webp)

## Quick Tour

To duplicate the baseline evaluation result, we provide the tutorials.

To generate the response using gpt4.
```python
python generate_response.py
```

To generate the response using llama or dbrx.
```python
python generate_with_llama.py
python generate_with_dbrx.py
```
Please note that the api_url may be subject to change over time, you can find the newest on [power.netmind.ai](https://power.netmind.ai/inference).

To clean the generated answer.
```python
cd jsonl
python process.py
```

To compare with the ground-truth data:
```python
python evaluate_response.py
```

Finally, in the visualize.ipynb, you can check the final accuracy.

## 📜 License

The new contributions to our dataset are distributed under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license, including

- The creation of the dataset;
- The filtering and cleaning of source datasets;
- The standard formalization of instances for evaluation purposes;
- The annotations of metadata.

The copyright of the images and the questions belongs to the original authors. Alongside this license, the following conditions apply:

- **Purpose:** The dataset was primarily designed for use as a test set.
- **Commercial Use:** The dataset can be used commercially as a test set, but using it as a training set is prohibited. By accessing or using this dataset, you acknowledge and agree to abide by these terms in conjunction with the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.
