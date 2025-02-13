### What’s in the Repository?
The repository contains implementations of various **data structures** in C. Here’s what you’ll likely find:
1. **Linked Lists**: A linear data structure where each element points to the next.
2. **Stacks**: A Last-In-First-Out (LIFO) data structure.
3. **Queues**: A First-In-First-Out (FIFO) data structure.
4. **Trees**: Hierarchical data structures like binary trees.
5. **Graphs**: Data structures for representing networks.
---

### How to Run the Code:
Since the repository contains multiple files, each file likely represents a specific data structure or algorithm. Here’s how you can run the code:

#### Step 1: Clone the Repository
- Open your terminal and run:
  ```bash
  git clone https://github.com/yossef-ashraf/Data-Structures.git
  ```

#### Step 2: Navigate to the Repository Folder
- Go to the downloaded folder:
  ```bash
  cd Data-Structures
  ```

#### Step 3: Explore the Files
- List the files in the repository to see what’s available:
  ```bash
  ls
  ```
  You’ll likely see files like `linked_list.c`, `stack.c`, `queue.c`, etc.

#### Step 4: Compile and Run a Specific File
- For example, if you want to run the **Linked List** implementation:
  1. Compile the file:
     ```bash
     gcc linked_list.c -o linked_list
     ```
  2. Run the executable:
     ```bash
     ./linked_list
     ```

- Repeat the same process for other files (e.g., `stack.c`, `queue.c`, etc.).

---

### Example: Running the Linked List Code
Let’s assume the `linked_list.c` file contains the following code:

```c
#include <stdio.h>
#include <stdlib.h>

struct Node {
    int data;
    struct Node* next;
};

void printList(struct Node* node) {
    while (node != NULL) {
        printf("%d -> ", node->data);
        node = node->next;
    }
    printf("NULL\n");
}

int main() {
    struct Node* head = NULL;
    struct Node* second = NULL;
    struct Node* third = NULL;

    head = (struct Node*)malloc(sizeof(struct Node));
    second = (struct Node*)malloc(sizeof(struct Node));
    third = (struct Node*)malloc(sizeof(struct Node));

    head->data = 1;
    head->next = second;

    second->data = 2;
    second->next = third;

    third->data = 3;
    third->next = NULL;

    printList(head);

    return 0;
}
```

#### Steps to Run:
1. Compile the code:
   ```bash
   gcc linked_list.c -o linked_list
   ```
2. Run the executable:
   ```bash
   ./linked_list
   ```

#### Expected Output:
```
1 -> 2 -> 3 -> NULL
```

---

### What Each File Does:
Here’s a brief explanation of what each file in the repository might do:

1. **`list.c`**:
   - Implements a singly linked list with basic operations like insertion, deletion, and traversal.

2. **`stack.c`**:
   - Implements a stack data structure with operations like `push`, `pop`, and `peek`.

3. **`queue.c`**:
   - Implements a queue data structure with operations like `enqueue`, `dequeue`, and `peek`.

4. **`tree.c`**:
   - Implements a binary tree with operations like insertion, deletion, and traversal (e.g., in-order, pre-order, post-order).

5. **`graph.c`**:
   - Implements a graph data structure (e.g., adjacency list or matrix) with operations like adding edges and traversing (e.g., BFS, DFS).

---

### How to Understand the Code:
1. **Look for Comments**:
   - The code should have comments explaining what each function or block of code does.

2. **Check the `main` Function**:
   - The `main` function usually demonstrates how the data structure or algorithm works.

3. **Experiment**:
   - Modify the code, add new features, or test edge cases to understand it better.

---

### Example: Running the Stack Code
If you want to run the stack implementation (`stack.c`), follow these steps:

1. Compile the code:
   ```bash
   gcc stack.c -o stack
   ```
2. Run the executable:
   ```bash
   ./stack
   ```

#### Expected Output:
If the stack code is implemented correctly, it will demonstrate stack operations like `push`, `pop`, and `peek`.

