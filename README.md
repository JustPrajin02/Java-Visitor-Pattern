# Java-Visitor-Pattern

"Java Visitor Pattern." It tasks you with applying the open/closed principle by implementing three specific visitor classes to traverse a tree structure without modifying the tree's internal code.

Part I: Implement Three Different Visitors

You must implement visitNode, visitLeaf, and getResult for these classes:

SumInLeavesVisitor: Returns the sum of values in the tree's leaf nodes (p. 1).

ProductRedNodesVisitor: Returns the product of values of all red nodes (including leaves), computed modulo 10^9+7. The product of zero nodes is 1 (pp. 1-2).

FancyVisitor: 
Returns the absolute difference between:

The sum of values of non-leaf nodes at even depth (the root is at depth 0).

The sum of values of green leaf nodes (p. 1).

Part II: Read and Build the Tree

You must construct the tree from the input, which is rooted at node 1 (p. 2).

Input Format:

Integer n: Number of nodes.

n integers: Node values (x1,x2,x3...,xn).

n binary integers: Node colors (0 for red,1 for green).

n-1 lines: Edges defined by two space-separated integers (u and v) (p. 2).

Constraints & Sample


Nodes (n): 2<=n<=10^5 (p. 2).

Values (xi): 1<=xi<=10^3 (p. 2).

Sample Input Result:

SumInLeavesVisitor: 24

ProductRedNodesVisitor: 40

FancyVisitor: 15 (pp. 2-3)

Explanation:

<img width="203" height="191" alt="image" src="https://github.com/user-attachments/assets/7b6fe853-6200-450b-a9ec-eed1f50ef6f6" />

Locked stub code in the editor tests your three class implementations as follows:

1. Creates a SumInLeavesVisitor object whose getResult method returns the sum of the leaves in the tree, which is 7+5+12=24 . The locked stub code prints the returned value on a new line.
   
2.Creates a ProductOfRedNodesVisitor object whose getResult method returns the product of the red nodes, which is 4.2.5=40. The locked stub code prints the returned value on a new line.

3.Creates a FancyVisitor object whose getResult method returns the absolute difference between the sum of the values of non-leaf nodes at even depth and the sum of the values of green leaf nodes, which is |4-(7+12)|=15. The locked stub code prints the returned value on a new line.


