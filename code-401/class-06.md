## Class 06

### Sources
- [How to Use Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
- [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
- [Test Coverage](https://martinfowler.com/bliki/TestCoverage.html)
- [Big O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)

### Notes

Random module can help create or shuffle random numbers and strings.

| function    | example + rules                             | tasks                                                                     |
|-------------|---------------------------------------------|---------------------------------------------------------------------------|
| randint()   | random.randint(1, 5)                        | generate random numbers within a range                                    |
| ...         | 1 = start         5 = stop, inclusive       |                                                                           |
| ...         | start < stop                                |                                                                           |
| random()    | random.random()                             | generate a random floating point number between 0 and 1                   |
| ...         | * n to get a larger number by n times       |                                                                           |
| ...         | n can be either positive or negative        |                                                                           |
| choice()    | random.choice(collection_obj)               | select a random element from a collection obj such as list, set, tuple... |
| ...         | collection obj cannot be empty              |                                                                           |
| choices()   | random.choices(coll_obj, k=3)               | select two or more elements randomly                                      |
| ...         | k = number of elements returned             |                                                                           |
| ...         | k can be greater than size  of coll_obj     |                                                                           |
| ...         | returns empty obj if input is empty & k = 0 |                                                                           |
| shuffle()   | random.shuffle()                            | shuffles the elements in place                                            |
| randrange() | random.randrange(start, stop, step)         |                                                                           |
| ...         | works as a combo of choice() and range()    |                                                                           |

Risk is defined as the probability of any unwanted incident

Steps
1. Identify
2. Assess


Risk Identification
- inherent business risks
- testing risks
- premature release risk
- software risks

Risk Assessment
- effect
- cause
- likelihood

Risk Analysis
1. Searching the risk
2. Analyzing the impact of each individual risk
3. Measures for the risk identified

Unwanted incidents include 
1. Use of new hardware
2. Use of new technology
3. Use of a new automation tool
4. Sequence of code
5. Availability of test resources for the application

Unavoidable risks
1. testing time
2. defect leakage
3. expedited timelines per client urgency requests
4. incomplete requirements

Risk magnitude (severity) indicators
- low (little or no external exposure or financial loss)
- medium (limited financial risk)
- high (non-tolerable, financial loss)

### Bookmark and Review
- [Python Random](https://docs.python.org/3/library/random.html)

### Further Reading
- [What is Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)

### Reading Questions
1. How can the random module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module? Use random.randint() to generate random numbers and random.choice() to make a selection. Other common functions include randrange(), random(), and shuffle().

2. In the context of software development, what is risk analysis, and what are the key steps involved in conducting a risk analysis for a software project? Risk analysis is the process of identifying, assessing, and creating a mitigation plan in the event of an unwanted incident prior to the actual software release. The steps as already mentioned include identification, assessment, and analysis.

3. What is test coverage and why is it an important (or potentially misleading) metric in software testing? According to the article, test coverage is a tool used to find untested parts of a codebase. The metric is important for management. The best indicator of good test coverage is bugs are a rare occurrence once released to production, and the codebase is easy to refactor and unlikely to introduce more bugs. 

4. What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity. Big O notation is way to describe the efficiency of an algorithm, like how much longer does it take to complete the task when  compared to the size of input. An everyday example of O(n) is like buying groceries. The larger the grocery list, the longer it takes to buy everything on the list. 