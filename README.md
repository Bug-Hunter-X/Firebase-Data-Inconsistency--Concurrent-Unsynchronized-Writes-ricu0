# Firebase Data Inconsistency Bug
This repository demonstrates a bug related to data inconsistency in Firebase when multiple clients write to the same data concurrently without proper synchronization. The bug involves a simple counter application where multiple users incrementing the counter simultaneously can lead to inaccurate counter values.

## Bug Description
The `counterBug.js` file shows how unsynchronized writes cause the counter to update inconsistently, resulting in an incorrect final value. 

## Solution
The `counterSolution.js` file illustrates a solution using Firebase transactions to ensure atomic updates, thereby resolving the inconsistency issue.

## How to Reproduce
1.  Clone the repository.
2.  Install Firebase dependencies: `npm install firebase`
3.  Configure Firebase (replace placeholders with your project details) in both `counterBug.js` and `counterSolution.js`.
4.  Run `counterBug.js` to observe the inconsistent behavior.
5.  Run `counterSolution.js` to observe the consistent behavior using transactions.