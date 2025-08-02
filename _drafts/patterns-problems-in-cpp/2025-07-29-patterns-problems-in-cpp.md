---
layout: post
title:  "Pattern problems in Cpp"
date:   2025-07-23
categories: Cpp loops patterns dsa
author: insane
permalink: /posts/pattern-problems-in-cpp
---
Patterns problems in C++ archive here. I will probably keep on updating it as I solve more similar problems.

These are mostly solved just using for loops. Their are many ways to so solve one pattern, for example some will start i from 1 some from 0, some will use <= to end the loop while some <. These will mostly change the loop calculations a bit. I have just used one of the ways which I felt OK when writing the programs.

---

Pattern 1 -

```
* * * *
* * * *
* * * *
* * * *
```

```cpp
void print1(int n) {
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            cout << "* ";
        }
        cout << endl;
    }
}
```

---

Pattern 2 -

```
*
* *
* * *
* * * *
* * * * *
```

```cpp
void print2(int n) {
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < i + 1; j++) {
            cout << "* ";
        }
        cout << endl;
    }
}
```

---

Pattern 3 -

```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

```cpp
void print3(int n) {
    for (int i = 0; i < n; i++) {
        for (int j = 1; j < i + 1; j++) {
            cout << j << " ";
        }
        cout << endl;
    }
}
```

---

Pattern 4 -

```
1
2 2
3 3 3
4 4 4 4
5 5 5 5 5
```

```cpp
void print4(int n) {
    for (int i = 0; i < n; i++) {
        for (int j = 1; j < i + 1; j++) {
            cout << i + 1  << " ";
        }
        cout << endl;
    }
}
```

---

Pattern 5 -

```
* * * *
* * *
* *
*
```

```cpp
void print5(int n) {
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n - i; j++) {
            cout << "* ";
        }
        cout << endl;
    }
}
```