# 🚀 **The Ultimate LeetCode Cheatsheet**

## **Master Guide to Conquering Any LeetCode Problem**

*Your comprehensive reference for pattern recognition, algorithm selection, and systematic problem-solving*

---/

## **📋 Table of Contents**

1. [🎯 **Universal Problem-Solving Framework**](#-universal-problem-solving-framework)
2. [🔍 **Keyword Detection & Pattern Recognition**](#-keyword-detection--pattern-recognition)
3. [🌳 **Decision Trees for Every Pattern**](#-decision-trees-for-every-pattern)
4. [⚡ **Quick Reference Tables**](#-quick-reference-tables)
5. [🎨 **Visual Pattern Mapping**](#-visual-pattern-mapping)
6. [💡 **Implementation Templates**](#-implementation-templates)
7. [📊 **Complexity Analysis Guide**](#-complexity-analysis-guide)
8. [🎯 **Problem-Specific Cheatsheets**](#-problem-specific-cheatsheets)

---

## **🎯 Universal Problem-Solving Framework**

### **The 6-Step Process for Any LeetCode Problem**

```
1. READ → Extract keywords and data structure hints
2. MAP → Keywords → Algorithm category  
3. REFINE → Choose specific algorithm and data structure
4. IMPLEMENT → Use appropriate template
5. ANALYZE → Verify time/space complexity
6. TEST → Run through test cases
```

### **🔍 Step 1: Keyword Detection**

| **Category** | **Keywords** | **Algorithm Signal** | **Priority** |
|--------------|--------------|---------------------|--------------|
| **Data Structure** | `"array"`, `"string"`, `"linked list"`, `"tree"`, `"graph"` | **Primary Pattern** | 🔴 **HIGH** |
| **Operation** | `"sum"`, `"find"`, `"search"`, `"traverse"`, `"generate"` | **Algorithm Type** | 🔴 **HIGH** |
| **Constraint** | `"without repeating"`, `"sorted"`, `"unique"`, `"duplicate"` | **Implementation Detail** | 🟡 **MEDIUM** |
| **Optimization** | `"longest"`, `"shortest"`, `"maximum"`, `"minimum"` | **Tracking Required** | 🟡 **MEDIUM** |
| **Sequence** | `"substring"`, `"subarray"`, `"subsequence"` | **Window/Two Pointers** | 🟢 **LOW** |

---

## **🔍 Keyword Detection & Pattern Recognition**

### **🎨 Color-Coded Keyword Analysis**

| **Keyword** | **Color** | **Pattern** | **Algorithm** | **Implementation** |
|-------------|-----------|-------------|---------------|-------------------|
| **"running sum"** | 🔴 Red | **Prefix Sum** | `prefix[i] = prefix[i-1] + nums[i]` | Cumulative sum |
| **"longest substring"** | 🟢 Green | **Sliding Window** | `while right < len: expand/contract` | Two pointers + hash set |
| **"add two numbers"** | 🔵 Blue | **Linked List + Carry** | `total = val1 + val2 + carry` | Two pointers + carry |
| **"tree traversal"** | 🟡 Yellow | **BFS/DFS** | `queue = [root]` or `def dfs(node)` | Queue/Recursion |
| **"top k elements"** | 🟣 Purple | **Heap** | `heapq.heappush/pop` | Priority queue |
| **"how many ways"** | 🟠 Orange | **Dynamic Programming** | `dp[i] = dp[i-1] + dp[i-2]` | State transitions |

### **🧠 Mental Model from Keywords**

```
"running sum" → Think: "Prefix sum array"
"longest substring" → Think: "Sliding window + hash set"  
"add two numbers" → Think: "Two pointers + carry handling"
"tree" → Think: "BFS/DFS traversal"
"top k" → Think: "Heap/priority queue"
"how many ways" → Think: "Dynamic programming"
```

---

## **🌳 Decision Trees for Every Pattern**

### **📝 Master Decision Tree**

```
What is the PRIMARY data structure?
├─ Array/String → Check Array/String Patterns
├─ Linked List → Check Linked List Patterns  
├─ Tree/Graph → Check Tree/Graph Patterns
├─ Heap → Check Heap Patterns
├─ Stack/Queue → Check Stack/Queue Patterns
└─ Other → Check DP/Backtracking/Binary Search

What is the PRIMARY operation?
├─ Search → Binary Search/Two Pointers
├─ Traversal → BFS/DFS
├─ Optimization → DP/Greedy
├─ Generation → Backtracking
├─ Arithmetic → Two Pointers + Carry
└─ Window → Sliding Window
```

### **🔍 Array/String Decision Tree**

```
Is it an ARRAY/STRING problem?
├─ YES → Check operation type
│   ├─ Sum/Count operations?
│   │   ├─ "running sum", "prefix sum" → **Prefix Sum Array**
│   │   ├─ "subarray sum" → **Prefix Sum + Hash Map**
│   │   └─ "range sum queries" → **Prefix Sum Array**
│   ├─ Search operations?
│   │   ├─ "X sum" (two sum, three sum) → **Two Pointers**
│   │   ├─ "find target" → **Hash Map**
│   │   └─ "rotated sorted" → **Modified Binary Search**
│   ├─ Sequence operations?
│   │   ├─ "substring" → **Sliding Window**
│   │   ├─ "longest substring" → **Sliding Window**
│   │   └─ "palindrome" → **Two Pointers**
│   ├─ Optimization operations?
│   │   ├─ "maximum subarray" → **Kadane's Algorithm**
│   │   ├─ "top k elements" → **Heap**
│   │   └─ "minimum/maximum" → **Greedy/DP**
│   └─ Manipulation operations?
│       ├─ "reverse array" → **Two Pointers**
│       ├─ "rotate array" → **Array Reversal**
│       └─ "merge arrays" → **Two Pointers**
└─ NO → Check other data structures
```

### **🔗 Linked List Decision Tree**

```
Is it a LINKED LIST problem?
├─ YES → Check operation type
│   ├─ Arithmetic operations?
│   │   ├─ "add two numbers" → **Two Pointers + Carry**
│   │   ├─ "multiply" → **Two Pointers + Carry**
│   │   └─ "subtract" → **Two Pointers + Borrow**
│   ├─ Traversal operations?
│   │   ├─ "find middle" → **Fast & Slow Pointers**
│   │   ├─ "detect cycle" → **Fast & Slow Pointers**
│   │   └─ "reverse list" → **In-place Reversal**
│   ├─ Manipulation operations?
│   │   ├─ "merge lists" → **Two Pointers**
│   │   ├─ "remove duplicates" → **Single Pointer**
│   │   └─ "partition" → **Two Pointers**
│   └─ Position operations?
│       ├─ "remove nth from end" → **Fast & Slow Pointers**
│       ├─ "swap nodes" → **Pointer Manipulation**
│       └─ "rotate list" → **Find Tail + Connect**
└─ NO → Check other data structures
```

### **🌲 Tree/Graph Decision Tree**

```
Is it a TREE/GRAPH problem?
├─ YES → Check structure type
│   ├─ Binary Tree?
│   │   ├─ Traversal needed?
│   │   │   ├─ "level order" → **BFS (Queue)**
│   │   │   ├─ "pre/in/post order" → **DFS (Recursive)**
│   │   │   └─ "zigzag" → **BFS + Level tracking**
│   │   ├─ Path problems?
│   │   │   ├─ "path sum" → **DFS**
│   │   │   ├─ "longest path" → **DFS + Global max**
│   │   │   └─ "path to leaf" → **DFS**
│   │   └─ Structure problems?
│   │       ├─ "validate BST" → **DFS + Range**
│   │       ├─ "symmetric tree" → **DFS (Two nodes)**
│   │       └─ "balanced tree" → **DFS + Height**
│   ├─ Graph?
│   │   ├─ Traversal needed?
│   │   │   ├─ "shortest path" → **BFS**
│   │   │   ├─ "all paths" → **DFS + Backtracking**
│   │   │   └─ "connected components" → **DFS/BFS**
│   │   └─ Cycle detection?
│   │       ├─ "detect cycle" → **DFS + Visited set**
│   │       └─ "topological sort" → **DFS + Stack**
│   └─ Matrix as Graph?
│       ├─ "islands" → **DFS/BFS**
│       ├─ "word search" → **DFS + Backtracking**
│       └─ "shortest path in grid" → **BFS**
└─ NO → Check other data structures
```

---

## **⚡ Quick Reference Tables**

### **🎯 Pattern → Keywords → Algorithm Mapping**

| **Pattern** | **Keywords** | **Algorithm** | **Time** | **Space** | **Template** |
|-------------|--------------|---------------|----------|-----------|--------------|
| **Prefix Sum** | `"running sum"`, `"prefix sum"`, `"cumulative"` | Prefix Sum Array | O(n) | O(1) | `result[i] = result[i-1] + nums[i]` |
| **Two Pointers** | `"X sum"`, `"palindrome"`, `"sorted array"` | Two Pointers | O(n) | O(1) | `left = 0, right = len-1` |
| **Sliding Window** | `"substring"`, `"window"`, `"longest substring"` | Sliding Window | O(n) | O(k) | `while right < len: expand/contract` |
| **BFS/DFS** | `"tree"`, `"graph"`, `"level order"`, `"path"` | BFS/DFS | O(V + E) | O(h) | `queue = [root]` or `def dfs(node)` |
| **Heap** | `"top k"`, `"kth largest"`, `"priority"` | Heap/Priority Queue | O(n log k) | O(k) | `heapq.heappush/pop` |
| **DP** | `"how many ways"`, `"maximum"`, `"minimum"` | Dynamic Programming | O(n) to O(n²) | O(n) to O(n²) | `dp[i] = max/min(dp[i-1], ...)` |
| **Backtracking** | `"generate all"`, `"N-Queens"`, `"permutations"` | Backtracking | O(2^n) | O(n) | `def backtrack(path, choices):` |
| **Binary Search** | `"find target"`, `"rotated"`, `"peak element"` | Binary Search | O(log n) | O(1) | `while left <= right: mid = (left + right) // 2` |

### **🔍 Keyword → Implementation Quick Lookup**

| **See This** | **Think This** | **Use This** | **Example** |
|--------------|----------------|--------------|-------------|
| `"running sum"` | **Prefix Sum** | `result[i] = result[i-1] + nums[i]` | Running Sum of 1d Array |
| `"longest substring"` | **Sliding Window** | `while right < len: expand/contract` | Longest Substring Without Repeating |
| `"add two numbers"` | **Two Pointers + Carry** | `total = val1 + val2 + carry` | Add Two Numbers |
| `"tree traversal"` | **BFS/DFS** | `queue = [root]` or `def dfs(node)` | Binary Tree Level Order |
| `"top k elements"` | **Heap** | `heapq.nlargest(k, nums)` | Top K Frequent Elements |
| `"how many ways"` | **DP** | `dp[i] = dp[i-1] + dp[i-2]` | Climbing Stairs |
| `"generate all"` | **Backtracking** | `def backtrack(path, choices):` | Generate Parentheses |
| `"find target"` | **Binary Search** | `while left <= right: mid = (left + right) // 2` | Search in Rotated Array |

---

## **🎨 Visual Pattern Mapping**

### **🌈 Color-Coded Pattern Recognition**

| **Pattern** | **Color** | **Visual Cue** | **When to Use** |
|-------------|-----------|----------------|-----------------|
| **Prefix Sum** | 🔴 **Red** | `"running sum"`, `"prefix sum"` | Array cumulative operations |
| **Sliding Window** | 🟢 **Green** | `"substring"`, `"window"`, `"longest"` | Contiguous sequence problems |
| **Two Pointers** | 🔵 **Blue** | `"X sum"`, `"palindrome"`, `"sorted"` | Sorted array operations |
| **BFS/DFS** | 🟡 **Yellow** | `"tree"`, `"graph"`, `"level order"` | Tree/graph traversal |
| **Heap** | 🟣 **Purple** | `"top k"`, `"kth largest"`, `"priority"` | Priority-based operations |
| **DP** | 🟠 **Orange** | `"how many ways"`, `"maximum"`, `"minimum"` | Optimization problems |
| **Backtracking** | 🟤 **Brown** | `"generate all"`, `"N-Queens"`, `"permutations"` | Generation problems |
| **Binary Search** | ⚫ **Black** | `"find target"`, `"rotated"`, `"peak"` | Search in sorted data |

### **🔗 Keyword Chain → Complete Algorithm**

```
"running sum" → Prefix Sum Array
    ↓
"array" → Single pass iteration
    ↓
"cumulative" → result[i] = result[i-1] + nums[i]
    ↓
RESULT: O(n) time, O(1) space

"longest substring" → Sliding Window
    ↓
"without repeating" → Hash Set tracking
    ↓
"substring" → Contiguous sequence
    ↓
RESULT: Two pointers + hash set + maximum tracking

"add two numbers" → Two Pointers + Carry
    ↓
"linked lists" → Pointer manipulation
    ↓
"reverse order" → Left-to-right processing
    ↓
RESULT: Two pointers + carry + dummy head + while loop
```

---

## **💡 Implementation Templates**

### **🎯 Universal Templates for Each Pattern**

#### **Prefix Sum Template**
```python
def prefixSum(nums):
    result = [nums[0]]
    for i in range(1, len(nums)):
        result.append(result[-1] + nums[i])
    return result
```

#### **Sliding Window Template**
```python
def slidingWindow(s):
    left = 0
    char_set = set()
    max_length = 0
    
    for right in range(len(s)):
        while constraint_violated:
            char_set.remove(s[left])
            left += 1
        
        char_set.add(s[right])
        max_length = max(max_length, right - left + 1)
    
    return max_length
```

#### **Two Pointers Template**
```python
def twoPointers(nums):
    left, right = 0, len(nums) - 1
    
    while left < right:
        if condition_met:
            return result
        elif nums[left] + nums[right] < target:
            left += 1
        else:
            right -= 1
    
    return -1
```

#### **BFS Template**
```python
def bfs(root):
    if not root:
        return []
    
    queue = [root]
    result = []
    
    while queue:
        level_size = len(queue)
        level = []
        
        for _ in range(level_size):
            node = queue.pop(0)
            level.append(node.val)
            
            if node.left:
                queue.append(node.left)
            if node.right:
                queue.append(node.right)
        
        result.append(level)
    
    return result
```

#### **DFS Template**
```python
def dfs(node):
    if not node:
        return
    
    # Process current node
    process(node)
    
    # Recursively process children
    dfs(node.left)
    dfs(node.right)
```

#### **Heap Template**
```python
import heapq

def topK(nums, k):
    heap = []
    
    for num in nums:
        heapq.heappush(heap, num)
        if len(heap) > k:
            heapq.heappop(heap)
    
    return heap
```

#### **DP Template**
```python
def dp(n):
    if n <= 1:
        return n
    
    dp = [0] * (n + 1)
    dp[1] = 1
    
    for i in range(2, n + 1):
        dp[i] = dp[i-1] + dp[i-2]
    
    return dp[n]
```

#### **Backtracking Template**
```python
def backtrack(path, choices):
    if base_case:
        result.append(path[:])
        return
    
    for choice in choices:
        if is_valid(choice):
            path.append(choice)
            backtrack(path, updated_choices)
            path.pop()
```

#### **Binary Search Template**
```python
def binarySearch(nums, target):
    left, right = 0, len(nums) - 1
    
    while left <= right:
        mid = (left + right) // 2
        
        if nums[mid] == target:
            return mid
        elif nums[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    
    return -1
```

---

## **📊 Complexity Analysis Guide**

### **⏱️ Time Complexity Patterns**

| **Pattern** | **Best Case** | **Average Case** | **Worst Case** | **Notes** |
|-------------|---------------|------------------|----------------|-----------|
| **Prefix Sum** | O(n) | O(n) | O(n) | Single pass through array |
| **Two Pointers** | O(n) | O(n) | O(n) | Each element visited once |
| **Sliding Window** | O(n) | O(n) | O(n) | Each element visited at most twice |
| **BFS/DFS** | O(V + E) | O(V + E) | O(V + E) | Visit each vertex and edge once |
| **Heap** | O(n log k) | O(n log k) | O(n log k) | k operations on heap of size k |
| **DP** | O(n) | O(n²) | O(n²) | Depends on state transitions |
| **Backtracking** | O(2^n) | O(2^n) | O(2^n) | Exponential search space |
| **Binary Search** | O(log n) | O(log n) | O(log n) | Halve search space each iteration |

### **💾 Space Complexity Patterns**

| **Pattern** | **Space** | **Reasoning** |
|-------------|-----------|---------------|
| **Prefix Sum** | O(1) | In-place modification |
| **Two Pointers** | O(1) | Only pointers needed |
| **Sliding Window** | O(k) | Hash set for window characters |
| **BFS** | O(w) | Queue stores one level |
| **DFS** | O(h) | Recursion stack depth |
| **Heap** | O(k) | Heap of size k |
| **DP** | O(n) | DP table of size n |
| **Backtracking** | O(n) | Recursion depth |
| **Binary Search** | O(1) | Only pointers needed |

---

## **🎯 Problem-Specific Cheatsheets**

### **🔴 Prefix Sum Problems**

**Keywords:** `"running sum"`, `"prefix sum"`, `"cumulative"`, `"range sum"`

**Template:**
```python
def prefixSum(nums):
    for i in range(1, len(nums)):
        nums[i] += nums[i-1]
    return nums
```

**Examples:** Running Sum of 1d Array, Range Sum Query

---

### **🟢 Sliding Window Problems**

**Keywords:** `"longest substring"`, `"substring"`, `"window"`, `"without repeating"`

**Template:**
```python
def slidingWindow(s):
    left = 0
    char_set = set()
    max_length = 0
    
    for right in range(len(s)):
        while s[right] in char_set:
            char_set.remove(s[left])
            left += 1
        
        char_set.add(s[right])
        max_length = max(max_length, right - left + 1)
    
    return max_length
```

**Examples:** Longest Substring Without Repeating Characters, Minimum Window Substring

---

### **🔵 Linked List Problems**

**Keywords:** `"linked lists"`, `"add two numbers"`, `"reverse"`, `"merge"`

**Template:**
```python
def linkedListArithmetic(l1, l2):
    dummy = ListNode(0)
    current = dummy
    carry = 0
    
    while l1 or l2 or carry:
        val1 = l1.val if l1 else 0
        val2 = l2.val if l2 else 0
        
        total = val1 + val2 + carry
        digit = total % 10
        carry = total // 10
        
        current.next = ListNode(digit)
        current = current.next
        
        l1 = l1.next if l1 else None
        l2 = l2.next if l2 else None
    
    return dummy.next
```

**Examples:** Add Two Numbers, Merge Two Sorted Lists, Reverse Linked List

---

## **🚨 Critical Success Patterns**

### **⚡ Red Flag Keywords (High Priority)**

| **Keyword** | **Pattern** | **Action** |
|-------------|-------------|------------|
| 🔴 **"running sum"** | **Prefix Sum** | Use cumulative sum pattern |
| 🔴 **"longest substring"** | **Sliding Window** | Use two pointers + hash set |
| 🔴 **"add two numbers"** | **Linked List + Carry** | Use two pointers + carry handling |
| 🔴 **"tree traversal"** | **BFS/DFS** | Use queue or recursion |
| 🔴 **"top k"** | **Heap** | Use priority queue |
| 🔴 **"how many ways"** | **DP** | Use dynamic programming |

### **💡 Pattern Recognition Cheat Sheet**

```
IF you see "running sum" + "array"
THEN use: Prefix sum array pattern

IF you see "longest substring" + "without repeating"
THEN use: Sliding window + hash set

IF you see "linked lists" + "add"
THEN use: Two pointers + carry handling

IF you see "tree" + "traversal"
THEN use: BFS/DFS

IF you see "top k" + "elements"
THEN use: Heap/priority queue

IF you see "how many ways" + "optimization"
THEN use: Dynamic programming
```

---

## **🎯 Master Algorithm Selection Process**

### **The Ultimate Decision Framework**

```
1. READ the problem statement
   ↓
2. EXTRACT keywords (highlighted in color)
   ↓
3. IDENTIFY primary data structure
   ↓
4. MAP keywords to algorithm pattern
   ↓
5. SELECT appropriate template
   ↓
6. IMPLEMENT with proper complexity
   ↓
7. TEST with edge cases
```

### **🔍 Quick Pattern Scanner**

| **See This** | **Think This** | **Use This** |
|--------------|----------------|--------------|
| `"running sum"` | **Prefix Sum** | `result[i] = result[i-1] + nums[i]` |
| `"longest substring"` | **Sliding Window** | `while right < len: expand/contract` |
| `"add two numbers"` | **Two Pointers + Carry** | `total = val1 + val2 + carry` |
| `"tree traversal"` | **BFS/DFS** | `queue = [root]` or `def dfs(node)` |
| `"top k elements"` | **Heap** | `heapq.heappush/pop` |
| `"how many ways"` | **DP** | `dp[i] = dp[i-1] + dp[i-2]` |
| `"generate all"` | **Backtracking** | `def backtrack(path, choices):` |
| `"find target"` | **Binary Search** | `while left <= right: mid = (left + right) // 2` |

---

## **🎉 Final Success Formula**

**The Ultimate LeetCode Success Formula:**

1. **🔍 Scan for keywords** (use color highlighting)
2. **🌳 Follow decision trees** (systematic approach)
3. **⚡ Apply templates** (proven patterns)
4. **📊 Verify complexity** (time/space analysis)
5. **✅ Test edge cases** (comprehensive validation)

**Remember:** Every LeetCode problem follows a pattern. Master the patterns, master LeetCode! 🚀

---

*This cheatsheet combines insights from exhaustive analysis of all LeetCode preparation materials, providing you with the ultimate systematic approach to conquering any coding interview problem.*
