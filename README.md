# 🚀 Prefix Common Array Problem: MAANG-Level Interview Question

This repository contains the solution to the **Prefix Common Array Problem**, a **MAANG-level coding question** commonly seen in top tech company interviews. The solution is implemented in **Java** with an efficient **O(n)** approach using a **Frequency Array**.

---

## 📌 Problem Statement

You are given two integer arrays, `A` and `B`, of the same length `n`.  
Your task is to compute the **prefix common array** `result`, where:

- `result[i]` is the count of numbers that are common in both arrays from index `0` to `i`.

---

## 💡 Intuition

The key idea is to efficiently count how many elements are common between the two arrays at each prefix. By using a **frequency array**, we can track occurrences of elements as we iterate through the arrays. When an element is encountered in both arrays (frequency becomes 2), it is considered "common."

---

## ⚙️ Approach

1. Initialize:
   - `result` array to store the prefix common counts.
   - `freq` array to track occurrences of each number.
   - `commonCount` variable to track the count of common elements.

2. Iterate through both arrays:
   - Increment the frequency of the current number in `A`. If its frequency becomes 2, it is common.
   - Increment the frequency of the current number in `B`. If its frequency becomes 2, it is common.

3. Store the current count of common elements in the `result` array for each prefix.

4. Return the `result` array.

---

## 🕒 Complexity Analysis
1. Time Complexity:
  $$O(n)$$ – We iterate through the arrays once, performing constant-time operations for each index.

2. Space Complexity:
  $$O(n)$$ – The freq array requires space proportional to the input size.

---

## 🧠 Example Walkthrough
Input:
A = [1, 3, 2, 4]
B = [3, 1, 2, 4]

Output:
result = [0, 2, 3, 4]

Explanation:

For i = 0: No common numbers → result[0] = 0
For i = 1: Common numbers are [1, 3] → result[1] = 2
For i = 2: Common numbers are [1, 2, 3] → result[2] = 3
For i = 3: All numbers are common → result[3] = 4

---

## 🎥 YouTube Explanation
For a detailed explanation with visuals and examples, check out my YouTube video:
📺 Prefix Common Array | MAANG-Level Coding Question - https://youtu.be/STatMh7TW0M

