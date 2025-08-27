# Sample Projects

- The sample projects should be small enough to be interview questions but complex enough for a senior engineer to show
  depth and strong signals

## LRU Cache

- Use a Hashmap and a doubly linked list
- Support different eviction strategies
- Make it thread-safe
- Signals: Lock granularity, eviction policy, memory management

## Rate Limiter

- Support Fixed Window and Bucket strategies
- Make it thread-safe
- Signals: Time-windowing, atomic counters, scalability

## Custom Thread Pool

- Implement basic `ExecutorService`
- Support task queue, worker threads, graceful shutdown
- Bonus: priority queue and backpressure
- Signals: Thread lifecycle, blocking queues, graceful degradation

## In Memory Key-Value Store

- Redis-lite
- Support TTL
- Support Persistence
- Support Transactions
    - `begin()`, `commit()`, `rollback()`
- Handle nested transactions and dirty reads
- Write-ahead logging
- Signals: ACID principles, state management, rollback logic

## Object Pool

- Focus: Resource management, lifecycle control
- Resuse expensive objects (e.g. DB connections, threads)
- Handle max pool size, idle timeout, eviction
- Thread-safe with blocking `acquire()` and `release()`
- Signals: Thread coordination, resource efficiency, lifecycle hooks

## Expression Evaluator

- Evaluate expressions like `(2 + 3) * (4 - 1)`
- Support operator precedence and parentheses
- Bonus: add variables and assignment
- Signals: stack-based parsing, recursive descent, interpreter design