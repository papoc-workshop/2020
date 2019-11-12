---
title: Call for Papers
---

Consistency is one of the fundamental issues of distributed computing.
Beyond the well-known tension between Consistency, Availability, and Partition-tolerance, as captured by the CAP theorem, many nuanced consistency models and algorithms have been developed for different purposes.
These consistency models have subtly different behaviour in practice, which translates to difficult choices between fault tolerance, performance, and programmability.
The issues and trade-offs are particularly vexing at scale, with a large number of processes or large shared databases, and in the presence of high latency and failure-prone networks, such as edge computing and peer-to-peer networks.

Since its inception in 2014, the PaPoC workshop series has brought together researchers and practitioners who seek to develop better techniques and a better understanding of consistency in distributed systems.
We welcome contributions from a wide range of backgrounds: system development, distributed algorithms, concurrency, fault tolerance, databases, programming languages, and verification.
While there is no one universally best solution, we believe that by bringing together these perspectives, we can develop techniques that provide useful guarantees to applications, that are usable by application developers, and that satisfy real-world scalability, performance, and reliability requirements.

The workshop is looking for contributions on the following, and associated, topics:

* Design principles, correctness conditions, and programming patterns for scalable distributed data management systems.
* Techniques for relaxed consistency models: session guarantees, causal consistency, operational transformation, conflict-free replicated data types (CRDTs), monotonic programming, state merging, operation commutativity, etc.
* Data consistency in geo-replicated, peer-to-peer, and edge networks.
* Techniques for scaling and improving the performance of strongly consistent systems (e.g., Paxos-based, state machine replication, shared-log consensus, blockchains).
* How to expose consistency vs. performance and scalability trade-offs in the programming model, and how to help developers choose.
* How to support composed operations spanning multiple objects (transactions, sagas, workflows).
* Reasoning, analysis and verification of application programs using storage systems with weak consistency models.
* Strengthening the guarantees beyond consistency: fault tolerance, security, ensuring invariants are preserved, bounding metadata size, and controlling divergence.

How to submit your work
-----------------------

The PaPoC workshop invites two types of submissions:

* Short papers (5-6 pages) discussing original contributions, experience reports, or work in progress reports (supported by initial validations);
* Contributed talks, summarized in 2 page extended abstracts, reporting positions and visions for the future, identifying new challenges and research venues, or reports for early ongoing work. 

We accept longer proposals or submissions to other conferences, under the understanding that PC members are only expected to read the first six pages (in the case of papers) or two pages (in the case of extended abstracts) of such longer submissions.
All submissions should be written in English and provided in PDF format.
Submissions do not need to be anonymised.

Authors of accepted papers will have the opportunity to choose whether they want their papers published in ACM Digital Library (along with papers from other EuroSys workshops).
In any case, accepted papers and abstracts will be made available to participants of the workshop.
At least one author of each accepted submission is expected to present their work at the workshop, and to be available for discussions.

Instructions for submissions will appear here closer to the submission deadline.

Important Dates
---------------

| Submission deadline: | February 21, 2020 |
|----------------------|-------------------|
| Notification date:   | March 13, 2020    |
| Camera-Ready:        | March 27, 2020    |
| Workshop:            | April 27, 2020    |