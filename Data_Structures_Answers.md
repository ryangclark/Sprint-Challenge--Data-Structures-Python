Add your answers to the questions below.

1. What is the runtime complexity of your ring buffer's `append` method?

	`O(1)` – no loops

2. What is the space complexity of your ring buffer's `append` function?

	`O(1)` – no loops

3. What is the runtime complexity of your ring buffer's `get` method?

	`O(1)` – no loops

4. What is the space complexity of your ring buffer's `get` method?

	`O(1)` – no loops

5. What is the runtime complexity of the provided code in `names.py`?

	`O(n1 * n2)` where `n1` and `n2` are the lengths of the text files, respectively. Multiple because of the nested loops. Since the provided text files are of equal length, we can say that the provided code runs in `O(n^2)`.

6. What is the space complexity of the provided code in `names.py`?

	`O(n)`. The machine must store both arrays for each text file, so that's `2n`, which simplifies to n. Looping is iterative and doesn't have recursion's space implications.

7. What is the runtime complexity of your optimized code in `names.py`?

	`O(n2 log n1)`. I am not sure how this can be further optimized. Reading the names from both text files is `O(n)` each, and they are added because they run sequentially. Creating the binary search tree is also `O(n)` because it's a loop of `n1` length and it's added because it also runs sequentially. The final loop is `O(n2 * log n1)` because it loops through `n2` and checks the BST, which runs in `O(log n1)` time. Multiply because of the loop, and it's the biggest factor, so it simplifies to the runtime complexity after removing the other, smaller additions.

8. What is the space complexity of your optimized code in `names.py`?

	`O(n)` – similar to the provided code's space complexity. The machine must store both arrays for each text file, so that's `2n`, which simplifies to n. The machine must also store the binary search tree, which is another `n`, but simplifies out. Looping is iterative and doesn't have recursion's space implications.