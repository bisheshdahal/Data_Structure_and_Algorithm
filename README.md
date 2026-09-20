# Data Structures & Algorithms in Python

A collection of Jupyter notebooks where I work through the core data structures and algorithms every CS course (and every coding interview) eventually gets to. The goal isn't just to have working code sitting around — each notebook walks through the "why" behind the implementation, not just the "what," with short explanations after every code block so you can actually follow the reasoning instead of just reading syntax.

If you're learning this stuff for the first time, or just need a refresher on how a hash table actually resolves collisions, this repo is meant to be read top to bottom like a set of notes — run the cells, tweak the inputs, and see what breaks.

## What's inside

### 🔗 Linked Lists — `Linked_list.ipynb`
The building blocks of node-based data structures.
- **Singly linked list** — insertion (at the beginning, at the end, after a given node), deletion (from the beginning, from the end, by key), searching, and traversal.
- **Doubly linked list** — the same operations, but with a `prev` pointer added so the list can be walked backward as well as forward.

### 📦 Stacks & Queues — `Stacks_and_Queues.ipynb`
LIFO and FIFO structures, built from scratch and compared against Python's own tools.
- **Queues** — a naive array-backed queue (and why its `dequeue` is slower than you'd expect), a fixed-size list-backed queue, a properly O(1) circular queue, and Python's built-in `collections.deque`.
- **Stacks** — a bounded array-based stack with overflow/underflow checks.
- **Stack applications** — postfix expression evaluation, valid parenthesis checking, and infix-to-postfix conversion.

### 🌳 Trees — `Trees.ipynb`
From a plain binary tree all the way up to a self-balancing one.
- **Binary trees** — the basic node structure everything else builds on.
- **DFS traversals** — preorder, inorder, and postorder.
- **BFS traversal** — level-order traversal using a queue.
- **Expression trees** — evaluating a math expression stored as a tree.
- **Binary Search Tree (BST)** — insertion, searching, and deletion (including the tricky two-children case).
- **AVL Tree** — a self-balancing BST that uses height tracking, balance factors, and rotations to stay balanced no matter what order you insert into it.

### 🔍 Searching & Hashing — `Searching_and_Hashing.ipynb`
Finding things fast, and handling it when two things want the same spot.
- **Linear search** — finding the first occurrence, or every occurrence.
- **Binary search** — the O(log n) alternative once your data is sorted.
- **Hash tables** — three different ways to resolve collisions: linear probing, double hashing, and separate chaining.

### 🔃 Sorting — `Sortings.ipynb`
- **Bubble sort** — the classic starting point for sorting algorithms, with a look at why it runs in O(n²) time.

## How to use this repo

1. Clone it, then open any notebook in Jupyter (`jupyter notebook` or JupyterLab, or just open it in VS Code).
2. Run the cells top to bottom — each one builds on the last.
3. Read the short explanation after each code cell before moving to the next one; it's there to answer the "wait, why does this work?" question before it comes up.
4. Change the inputs and re-run things. The best way to actually understand a rotation in an AVL tree or a collision in a hash table is to break it yourself and watch what happens.

## Requirements

Just Python 3 and Jupyter. A couple of cells use `numpy`, but nothing here needs anything exotic — everything else is pure Python standard library (`collections.deque`, `typing`, etc.).

```bash
pip install jupyter numpy
```

## Why this exists

Mostly as a personal reference and a study log — a place to keep implementations I've actually typed out and understood, rather than just read about once and forgotten. If it helps you too, great. Contributions, corrections, and "hey, this explanation doesn't quite make sense" issues are welcome.
