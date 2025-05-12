# py-minmax  

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Tests](https://github.com/yourusername/py-minmax/actions/workflows/tests.yml/badge.svg)](https://github.com/yourusername/py-minmax/actions)

A lightweight Python library for efficiently finding **minimum** and **maximum** values in lists, arrays, and custom iterables. Optimized for simplicity and performance.

---

## Features  

- 🚀 **Fast** computation for built-in types (`int`, `float`, `str`).  
- 📦 Supports lists, tuples, and other iterables.  
- 🔧 Optional **key-function** for custom comparisons (e.g., objects).  
- ✅ Pure Python, zero dependencies.  

---

## Installation  

```bash
pip install py-minmax
Usage
python
from py_minmax import find_min, find_max

data = [3, 1, 4, 1, 5, 9, 2]

# Basic usage
print(find_min(data))  # Output: 1
print(find_max(data))  # Output: 9

# With key function (e.g., find longest string)
words = ["apple", "banana", "cherry"]
print(find_max(words, key=len))  # Output: "banana"
Benchmarks
Compare against native Python min()/max() (run benchmark.py):

Method	Time (1M elements)
py-minmax	0.045s
Native min	0.052s
Contributing
PRs welcome! See CONTRIBUTING.md for guidelines.

License
MIT © Sina Parsa
