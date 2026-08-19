# Plagiarism-__project
 A code plagiarism detection system that analyzes source-code similarity using preprocessing, tokenization, identifier normalization, similarity algorithms, and structural/AST analysis to identify potentially copied programming submissions.
# 🔍 Code Plagiarism Detector

> An intelligent source-code similarity detection system designed to identify potential plagiarism in programming assignments by analyzing lexical, token-level, sequential, and structural similarities.

---

## 📌 Overview

The **Code Plagiarism Detector** is a software system that analyzes programming submissions and identifies potentially copied or highly similar code.

Unlike simple text comparison, the system attempts to detect plagiarism even when the source code has been modified through:

- Variable renaming
- Function renaming
- Comment modification/removal
- Whitespace and formatting changes
- Minor code modifications
- Structural similarities

The system generates a **similarity score** and provides an explainable comparison between submissions.

> ⚠️ A high similarity score indicates potentially suspicious similarity; it does not by itself prove plagiarism. Final evaluation should be performed by a teacher, examiner, or authorized evaluator.

---

## 🎯 Problem Statement

Traditional code plagiarism detection systems based primarily on text matching can be bypassed by making simple changes to source code.

For example:

### Original Code

```cpp
int sum(int a, int b)
{
    return a + b;
}
