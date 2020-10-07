**Week-4 Project Submission

Project Instructions

Your modifications should be made entirely inside of ParBoruvka.java. You should not change the signatures of any public or protected methods inside of ParBoruvka.java, but you can edit the method bodies and add any new methods that you choose. We will use our copy of BoruvkaPerformanceTest.java in the final grading process, so do not change that file or any other file except ParBoruvka.java.

Your main goal for this assignment is to complete the computeBoruvka method at the top of ParBoruvka. The testing infrastructure will call computeBoruvka from a certain number of Java threads. You do not need to create any additional threads if you do not wish to (indeed, it is recommended that you do not). computeBoruvka is passed two objects:

nodesLoaded: A ConcurrentLinkedQueue object containing a list of all nodes in the input graph for which you are to compute a minimum spanning tree using Boruvka's algorithm. Because this Queue<ParComponent> object is a ConcurrentLinkedQueue, it is safe to access nodesLoaded from multiple threads concurrently without additional synchronization.
solution: A BoruvkaSolution object on which you will call BoruvkaSolution.setSolution once your parallel Boruvka implementation has collapsed the input graph down to a single component. You must only call setSolution once, and the testing infrastructure will use the provided result to verify your output.
Inside of ParBoruvka, there are two additional inner classes: ParComponent and ParEdge. ParComponent represents a single component in the graph. A component may be a singleton node, or it may be formed from collapsing multiple nodes into each other. A ParEdge represents an edge between two ParComponents. You may not change the signatures for the existing methods in ParComponent or ParEdge. However, you are free to modify their method bodies, to add new methods, or to add new fields. An efficient implementation will likely require modifications to ParComponent and/or ParEdge.
