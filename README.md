# Apriori_Algorithm_for_Drivers_Errors
🧾 Project Overview

This project performs frequent itemset mining on a traffic-related dataset using two classical algorithms: Apriori and FP-Growth. The objective is to analyze the efficiency and performance of these algorithms in terms of: 1.Time complexity 2.Number of frequent patterns found 3.Support values across iterations The focus is on identifying frequent co-occurring events, such as traffic congestion signals (SGN1), traffic flow (T), and priority routes (PR1), and evaluating how well each algorithm handles large datasets.

🔍 Dataset Details

The dataset comprises transactional-style records representing traffic patterns. Each record consists of multiple items such as:

T: Traffic event
SGN1: Signal 1 active
PR1, SC3: Priority route or sensor check active
Support Thresholds:

_1.First Iteration: Minimum support = 0.4

2.Subsequent Iterations: Minimum support = 0.1_

🧠 Algorithms Used

🔶 Apriori

Classical breadth-first algorithm
Candidate generation + pruning
Runtime: ~1.0002 seconds
🔷 FP-Growth

Tree-based depth-first approach
Avoids candidate generation
Runtime: ~0.4715 seconds
📈 Top 10 Frequent Itemsets

Apriori: Found itemsets like: (T), (SGN1), (T, SGN1), (PR1), (T, SGN1, PR1) Slower due to multiple passes and candidate generation

FP-Growth: Identified same top itemsets More efficient with ~50% reduction in runtime
