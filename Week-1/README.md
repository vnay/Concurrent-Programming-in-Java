**Week 1 project submission

Project Instructions

Your modifications should be made entirely inside of CoarseLists.java. You should not change the signatures of any public or protected methods inside of CoarseLists.java, but you can edit the method bodies and add any new methods that you choose. We will use our copy of ListSetTest.java in the final grading process, so do not change that file or any other file except CoarseLists .java.

Your main goals for this assignment are as follows:

Inside CoarseLists.java, implement the CoarseList class using a ReentrantLock object to protect the add, remove, and contains methods from concurrent accesses. You should refer to SyncList.java as a guide for placing synchronization and understanding the list management logic.
Inside CoarseLists.java, implement the RWCoarseList class using a ReentrantReadWriteLock object to protect the add, remove, and contains methods from concurrent accesses. You should refer to SyncList.java as a guide for placing synchronization and understanding the list management logic.
