# 9-Week Comprehensive Study Plan: Algorithms & System Design

**Total Duration**: 8 weeks (~88 hours)  
**Schedule**: 2 hours/weekday, 4 hours/weekend  
**Goal**: Build deep foundational knowledge + interview readiness

---

## Week 1: Trees - Fundamentals to Advanced

### Topics to Cover
1. **Binary Trees**: Traversals (inorder, preorder, postorder, level-order)
2. **Binary Search Trees**: Search, insert, delete, validation
3. **Balanced Trees**: AVL trees concept, Red-Black trees overview
4. **Advanced**: Segment Trees, Fenwick Trees (Binary Indexed Trees)

### Resources
- **Book**: *Introduction to Algorithms* (CLRS) - Chapter 12 (BST), Chapter 13 (Red-Black Trees)
- **Video**: MIT OCW 6.006 - Lecture 5 (Binary Search Trees), Lecture 6 (AVL Trees)
  - Link: https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/
- **Practice Platform**: LeetCode Trees section
- **Segment Trees Tutorial**: CP-Algorithms (https://cp-algorithms.com/data_structures/segment_tree.html)

### Practice Problems (Pick 8-10)
- LeetCode Easy: 94, 144, 145 (traversals), 104, 111, 226
- LeetCode Medium: 98, 102, 103, 105, 230, 236
- Segment Tree: Range Sum Query problems (307, 308)

### Implementation Exercise
**Weekend Project** (4 hours): Implement a self-balancing BST (AVL) in Python or Rust with insert/delete/search operations. Write unit tests.

### Milestone Checkpoint
- [ ] Can explain when to use BST vs balanced trees vs segment trees
- [ ] Can implement tree traversals without looking up
- [ ] Solved at least 8 problems independently
- [ ] Completed AVL tree implementation with tests

**If checkpoint fails**: Spend 2 extra days reviewing weak areas before moving to Week 2

---

## Week 2: Graphs - Traversal to Advanced Algorithms

### Topics to Cover
1. **Graph Representations**: Adjacency matrix, adjacency list, edge list
2. **Traversal**: BFS, DFS, topological sort
3. **Shortest Paths**: Dijkstra's, Bellman-Ford, Floyd-Warshall
4. **Advanced**: Union-Find (Disjoint Set), Minimum Spanning Trees (Kruskal's, Prim's)
5. **Special**: Tries (Prefix Trees) - for string algorithms

### Resources
- **Book**: CLRS - Chapter 22 (Elementary Graph Algorithms), Chapter 23 (MST), Chapter 24 (Shortest Paths)
- **Video**: MIT OCW 6.006 - Lectures 13-16 (Graphs, BFS/DFS, Dijkstra)
- **Tries**: https://www.youtube.com/watch?v=AXjmTQ8LEoI (Back to Back SWE)
- **Interactive Visualization**: VisuAlgo (https://visualgo.net/en/graphds)

### Practice Problems (Pick 10-12)
- BFS/DFS: 200, 133, 207, 210, 417
- Shortest Path: 743, 787, 1334
- Union-Find: 547, 684, 721, 990
- Tries: 208, 211, 212, 677

### Implementation Exercise
**Weekend Project**: Build a graph library in Go with:
- BFS/DFS traversal
- Dijkstra's shortest path
- Cycle detection
Include visualization output (text-based is fine)

### Milestone Checkpoint
- [ ] Can choose appropriate graph algorithm for a given problem
- [ ] Understands time/space complexity of each algorithm
- [ ] Solved at least 10 problems independently
- [ ] Implemented graph library with 3+ algorithms
- [ ] Can explain when to use Tries vs HashMaps

---

## Week 3: Dynamic Programming - From Zero to Hero

### Topics to Cover
1. **Fundamentals**: Memoization vs Tabulation, identifying subproblems
2. **1D DP**: Fibonacci, climbing stairs, house robber, coin change
3. **2D DP**: Unique paths, longest common subsequence, edit distance
4. **Advanced Patterns**: Knapsack (0/1, unbounded), longest increasing subsequence
5. **DP on Trees/Graphs**: Diameter of tree, path sum problems

### Resources
- **Book**: *Dynamic Programming for Coding Interviews* by Meenakshi & Kamal Rawat
- **Video Course**: Abdul Bari's DP Playlist (YouTube) - Start with basics
  - Link: https://www.youtube.com/watch?v=nqowUJzG-iM&list=PL_z_8CaSLPWekqhdCPmFohncHwz8TY2Go
- **Interactive**: Educative.io "Grokking Dynamic Programming" (if accessible)
- **Article**: "Demystifying Dynamic Programming" (freeCodeCamp)

### Practice Problems (Pick 12-15, DP needs volume)
- **1D DP**: 70, 198, 213, 322, 300, 152
- **2D DP**: 62, 63, 64, 72, 97, 115, 1143
- **Knapsack**: 416, 494, 518
- **Advanced**: 124, 543, 337

### Implementation Exercise
**Weekend Project**: Create a DP pattern recognition tool (Python):
- Input: Problem description
- Output: Suggests DP pattern (1D, 2D, Knapsack, etc.)
- Document 5 DP patterns with examples

### Milestone Checkpoint
- [ ] Can identify if a problem requires DP (optimal substructure + overlapping subproblems)
- [ ] Comfortable with both top-down and bottom-up approaches
- [ ] Solved at least 12 problems across different patterns
- [ ] Created pattern recognition documentation
- [ ] Can explain time/space optimization techniques (space-optimized DP)

**Critical**: DP is hard. If checkpoint fails, extend by 3 days and re-solve problems.

---

## Week 4: System Design Fundamentals - Scalability Basics

### Topics to Cover
1. **Scalability Principles**: Vertical vs horizontal scaling
2. **Load Balancing**: Algorithms (round-robin, least connections, consistent hashing)
3. **Caching Strategies**: 
   - Cache-aside, write-through, write-back, write-around
   - Eviction policies: LRU, LFU, FIFO
   - Cache invalidation patterns
4. **Database Fundamentals**: 
   - Indexing strategies (B-tree, hash, composite)
   - Query optimization basics
   - Connection pooling

### Resources
- **Book**: *Designing Data-Intensive Applications* by Martin Kleppmann - Chapters 1-3
- **Video**: Gaurav Sen's System Design Playlist (YouTube) - First 10 videos
  - Link: https://www.youtube.com/watch?v=xpDnVSmNFX0&list=PLMCXHnjXnTnvo6alSjVkgxV-VH6EPyvoX
- **Paper**: "Web Caching and Zipf-like Distributions: Evidence and Implications"
- **Interactive**: Redis University - RU101 (free, hands-on caching)
  - Link: https://university.redis.com/

### Practice Exercises
1. **Implement LRU Cache** (LeetCode 146) - Use in Python, Go, and Rust
2. **Design a URL Shortener** - Focus on caching strategy
3. **Query Optimization Challenge**:
   - Set up PostgreSQL locally
   - Load a dataset (1M+ rows)
   - Optimize 5 slow queries using EXPLAIN ANALYZE
   - Document before/after metrics
4. **Load Balancer Simulation** (Go):
   - Implement round-robin, least connections, weighted algorithms
   - Simulate 1000 requests, compare performance

### Reading Assignments
- "Scaling Memcache at Facebook" paper
- "Instagram Architecture" blog post
- Martin Fowler's "Cache-Aside" pattern article

### Milestone Checkpoint
- [ ] Can explain cache eviction policies and when to use each
- [ ] Completed LRU cache implementation in 2+ languages
- [ ] Successfully optimized 5 database queries with measurable improvements
- [ ] Can design a caching layer for a given system
- [ ] Understands trade-offs between different load balancing algorithms

---

## Week 5: Distributed Systems Concepts

### Topics to Cover
1. **CAP Theorem**: Consistency, Availability, Partition Tolerance
2. **Consistency Models**: Strong, eventual, causal consistency
3. **Consensus Algorithms**: Raft (focus), Paxos (overview)
4. **Data Partitioning**: Sharding strategies, consistent hashing
5. **Replication**: Leader-follower, multi-leader, leaderless
6. **Distributed Transactions**: 2PC, Saga pattern

### Resources
- **Book**: *Designing Data-Intensive Applications* - Chapters 5, 7, 8, 9
- **Paper**: "In Search of an Understandable Consensus Algorithm" (Raft paper)
  - Link: https://raft.github.io/raft.pdf
- **Interactive**: Raft Visualization - http://thesecretlivesofdata.com/raft/
- **Video**: MIT 6.824 Distributed Systems - Lectures 4-7
  - Link: https://www.youtube.com/channel/UC_7WrbZTCODu1o_kfUMq88g
- **Course**: Martin Kleppmann's Distributed Systems lectures (Cambridge)

### Practice Exercises
1. **Implement Consistent Hashing** (Python/Go):
   - Virtual nodes support
   - Add/remove nodes dynamically
   - Visualize key distribution
2. **Raft Consensus Simulation** (Rust):
   - Implement leader election
   - Log replication (basic version)
   - Use existing libraries for reference
3. **Design Exercise**: Design a distributed key-value store
   - Document: replication strategy, consistency model, partition handling
4. **Read Case Studies**:
   - Cassandra architecture
   - DynamoDB paper
   - Google Spanner paper (overview)

### Milestone Checkpoint
- [ ] Can explain CAP theorem with real-world examples
- [ ] Understands trade-offs between consistency models
- [ ] Completed consistent hashing implementation
- [ ] Can design a basic distributed system on whiteboard
- [ ] Read and understood at least 2 distributed systems papers

---

## Week 6: Advanced Caching & Database Design

### Topics to Cover
1. **Advanced Caching**:
   - Multi-level caching (CDN, application, database)
   - Cache warming strategies
   - Thundering herd problem & solutions
   - Geo-distributed caching
2. **Database Deep Dive**:
   - Normalization vs denormalization trade-offs
   - Indexing strategies for different query patterns
   - Database sharding: range-based, hash-based, directory-based
   - Read replicas and write scaling
3. **NoSQL Patterns**:
   - When to use document stores (MongoDB)
   - Column-family stores (Cassandra)
   - Key-value stores (Redis, DynamoDB)
   - Graph databases (Neo4j)

### Resources
- **Book**: 
  - *Database Internals* by Alex Petrov - Chapters 1-4
  - *Seven Databases in Seven Weeks* by Eric Redmond
- **Video**: 
  - CMU Database Systems (15-445) - Lectures on indexing and query optimization
  - Link: https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi
- **Articles**:
  - "Scaling Redis at Twitter"
  - "Sharding & IDs at Instagram"
  - "How Discord Stores Billions of Messages"

### Practice Exercises
1. **Database Schema Design Challenge**:
   - Design schemas for: Social media app, E-commerce platform, Analytics system
   - Include indexing strategy and sharding approach
2. **Caching Layer Implementation** (Go/Python):
   - Multi-level cache (in-memory + Redis)
   - Cache-aside pattern with database
   - Implement cache warming
   - Handle thundering herd with locks
3. **Query Optimization Project**:
   - Set up MongoDB and PostgreSQL
   - Same dataset in both
   - Compare query performance for different patterns
   - Document when to use which database

### Milestone Checkpoint
- [ ] Can design caching strategy for complex applications
- [ ] Understands database sharding strategies and trade-offs
- [ ] Completed multi-level cache implementation
- [ ] Can choose appropriate database for given use case
- [ ] Documented 3 complete system designs with caching + DB layers

---

## Week 7: Microservices Architecture & Communication Patterns

### Topics to Cover
1. **Microservices Fundamentals**:
   - Monolith vs Microservices trade-offs
   - Service boundaries (Domain-Driven Design basics)
   - API Gateway pattern
2. **Service Communication**:
   - REST vs gRPC vs GraphQL
   - Synchronous vs Asynchronous communication
   - Message queues (RabbitMQ, Kafka concepts)
   - Event-driven architecture
3. **Service Reliability**:
   - Circuit breaker pattern
   - Retry strategies with exponential backoff
   - Rate limiting and throttling
   - Service mesh basics (Istio overview)
4. **Observability**:
   - Distributed tracing (OpenTelemetry)
   - Logging strategies
   - Metrics and monitoring

### Resources
- **Book**: 
  - *Building Microservices* by Sam Newman - Chapters 1-5, 8-11
  - *Release It!* by Michael Nygard - Patterns section
- **Video**: 
  - "Mastering Chaos - A Netflix Guide to Microservices"
  - GOTO Conferences - Microservices talks
- **Documentation**:
  - gRPC official docs and tutorials
  - Apache Kafka documentation
  - Circuit Breaker pattern (Martin Fowler)

### Practice Exercises
1. **Build Microservices System** (Python + Go):
   - 3 services: User service (Python), Order service (Go), Notification service (Python)
   - API Gateway (Go)
   - Use gRPC for inter-service communication
   - Implement circuit breaker
   - Add distributed tracing with OpenTelemetry
2. **Message Queue Implementation**:
   - Set up RabbitMQ locally
   - Implement pub-sub pattern
   - Handle message failures and retries
3. **Design Exercise**: 
   - Break down a monolithic e-commerce app into microservices
   - Define service boundaries
   - Design communication patterns
   - Document failure scenarios and handling

### Milestone Checkpoint
- [ ] Built working microservices system with 3+ services
- [ ] Implemented circuit breaker and retry logic
- [ ] Understands trade-offs between REST, gRPC, and message queues
- [ ] Can design service boundaries for a given domain
- [ ] Documented microservices design with failure handling

---

## Week 8: Integration, Advanced Topics & Interview Prep

### Topics to Cover
1. **Advanced Algorithms**:
   - String algorithms: KMP, Rabin-Karp
   - Advanced graph: Network flow, bipartite matching
   - Computational geometry basics (if time permits)
2. **System Design Patterns**:
   - Rate limiting algorithms (token bucket, leaky bucket)
   - Idempotency in distributed systems
   - Event sourcing and CQRS
   - Real-time systems (WebSockets, Server-Sent Events)
3. **Interview-Specific**:
   - System design interview framework
   - Common pitfalls and how to avoid them
   - Communicating trade-offs effectively

### Resources
- **Book**: 
  - *System Design Interview* by Alex Xu - Volume 1 & 2
  - *Cracking the Coding Interview* - System design section
- **Video**: 
  - Exponent YouTube channel - Mock system design interviews
  - "System Design Interview Survival Guide" by Success in Tech
- **Practice Platform**: 
  - Pramp (free mock interviews)
  - SystemsExpert (paid but good)

### Practice Exercises
1. **Complete System Designs** (whiteboard/document):
   - Design Twitter
   - Design Netflix
   - Design Uber
   - Design WhatsApp
   - Design URL shortener (with all details)
   
   For each: Focus on scalability, caching, databases, trade-offs
   
2. **Algorithm Review**:
   - Solve 2-3 problems from each week
   - Focus on problems you found difficult
   
3. **Mock Interviews**:
   - Schedule 2-3 mock interviews on Pramp
   - Practice explaining your thought process
   
4. **Build a Complete System** (Weekend):
   - URL shortener with:
     - Microservices architecture
     - Caching layer
     - Database sharding
     - Rate limiting
     - Monitoring
   - Deploy on cloud (AWS/GCP free tier)

### Milestone Checkpoint
- [ ] Completed 5 full system design exercises with documentation
- [ ] Can explain system design interview approach clearly
- [ ] Participated in 2+ mock interviews
- [ ] Built and deployed complete system with multiple components
- [ ] Comfortable discussing trade-offs in any design decision

---

## Weekly Study Schedule Template

### Weekday (2 hours)
- **30 min**: Read theory/watch lecture
- **60 min**: Solve practice problems or implementation
- **30 min**: Document learnings, review mistakes

### Weekend (4 hours per day = 8 hours total)
- **Saturday**:
  - 2 hours: Deep dive into advanced topics
  - 2 hours: Work on weekend project
- **Sunday**:
  - 2 hours: Continue weekend project
  - 1 hour: Review week's learnings
  - 1 hour: Prepare for next week

---

## Progress Tracking System

Create a GitHub repo with:
```
/week-1-trees
  /implementations
  /problems-solved.md
  /notes.md
  /checkpoint.md
/week-2-graphs
  ...
```

### Weekly Review Template
```markdown
# Week X Review

## Topics Covered
- [ ] Topic 1
- [ ] Topic 2

## Problems Solved
1. Problem name - Difficulty - Link - Status (✓/✗)
2. ...

## Implementation Projects
- Project name - GitHub link - Status

## Key Learnings
- Concept 1: Explanation
- Pitfall: What I struggled with

## Checkpoint Status
- [ ] Checkpoint item 1
- [ ] Checkpoint item 2

## Action Items for Next Week
- Review: [specific topics if checkpoint failed]
- Focus: [areas needing more attention]
```

---

## Recommended Tools

### For Practice
- **LeetCode**: Primary problem solving
- **HackerRank**: Additional practice
- **Codeforces**: Advanced algorithms (optional)

### For Implementation
- **Python**: Quick prototyping, DP problems
- **Go**: System design implementations, concurrency
- **Rust**: Low-level algorithms, performance-critical code

### For System Design
- **Draw.io**: System diagrams
- **Excalidraw**: Quick sketches
- **Docker**: Containerize your implementations
- **PostgreSQL/MongoDB**: Database practice

### For Tracking
- **Notion/Obsidian**: Note-taking
- **GitHub**: Code tracking
- **Anki**: Spaced repetition for concepts

---

## Important Notes

1. **Don't Skip Checkpoints**: If you fail a checkpoint, spend extra time before moving on. Rushing leads to gaps.

2. **Hands-on is Critical**: Don't just read/watch. You must implement and solve problems.

3. **Use Multiple Languages**: It reinforces understanding and shows different paradigms.

4. **Document Everything**: Your notes will be invaluable for future review and interviews.

5. **Join Communities**:
   - r/cscareerquestions
   - r/algorithms
   - Discord servers for system design

6. **Adjust as Needed**: This is aggressive. If a week needs more time, take it. Better to learn deeply than superficially cover everything.

---

## Post-8-Week Maintenance Plan

After completion:
- **Week 9-12**: Solve 3-4 problems daily (mix of algo + system design)
- **Monthly**: Re-implement one major project from scratch
- **Quarterly**: Read one distributed systems paper
- **Ongoing**: Follow engineering blogs (Netflix, Uber, Meta, Amazon engineering blogs)

---

## Success Metrics

By end of 8 weeks, you should be able to:
- ✓ Solve medium LeetCode problems in 20-30 minutes
- ✓ Design scalable systems on whiteboard with trade-off discussions
- ✓ Explain caching strategies for any given scenario
- ✓ Debug and optimize database queries
- ✓ Implement microservices with proper patterns
- ✓ Read and understand academic papers on distributed systems
- ✓ Feel confident in your technical foundation

**Most importantly**: You'll have a solid mental model of how large-scale systems work, making you a more effective engineer regardless of your domain.

Good luck! Remember: Consistency > Intensity. 2 hours every day beats 10 hours once a week.
