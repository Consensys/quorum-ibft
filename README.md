# The Istanbul BFT Consensus Algorithm

This repository contains authoritative paper describing the Istanbul BFT Consensus Algorithm, or IBFT, for short. IBFT is a simple and elegant algorithm for Byzantine fault-tolerant consensus and is used to implement state machine replication in the *Quorum* blockchain.

IBFT assumes a partially synchronous communication model, where safety does not depend on any timing assumptions and only liveness depends on periods of synchrony. The algorithm is deterministic, leader-based, and optimally resilient - tolerating *f* faulty processes out of *n*, where *n* is equal or greater than *3f+1*. During periods of good communication, IBFT achieves termination in three message delays and has *O(n^2)* total communication complexity.
