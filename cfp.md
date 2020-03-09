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

Details on submissions
----------------------

The PaPoC workshop invites two types of submissions:

* Short papers (5–6 pages) discussing original contributions, experience reports, or work in progress reports (supported by initial validations);
* Contributed talks, summarized in 1–2 page extended abstracts, reporting positions and visions for the future, identifying new challenges and research venues, or reports for early ongoing work. 

We accept longer proposals, under the understanding that PC members are only expected to read the first six pages (in the case of papers) or two pages (in the case of extended abstracts) of such longer submissions.
All submissions should be written in English and provided in PDF format.
Submissions do not need to be anonymised.

Authors of accepted papers will have the opportunity to choose whether they want their papers published in ACM Digital Library (along with papers from other EuroSys workshops).
In any case, accepted papers and abstracts will be made available to participants of the workshop.
At least one author of each accepted submission is expected to present their work at the workshop, and to be available for discussions.

Authors may submit work that has appeared elsewhere or that is currently under submission elsewhere, provided that it is identified as such.
In this case, if their submission is accepted, the authors will be asked to produce a two-page summary that cites the full version of their work.
This summary is what will appear in the PaPoC materials.

How to submit your work
-----------------------

Submissions should be made [via Easychair](https://easychair.org/conferences/?conf=papoc2020).

Submissions should be in PDF format.
We suggest that you use the [ACM template for LaTeX or MS Word](https://www.acm.org/publications/proceedings-template), but this is not requried.
If using the LaTeX template, please use the following document class (which matches the [format used by EuroSys](https://www.eurosys2020.org/paper-submission/)):

    \documentclass[sigplan,10pt]{acmart}

In case of any questions, please contact the Program Chairs at [papoc2020@easychair.org](mailto:papoc2020@easychair.org).

Important Dates
---------------

| Submission deadline: | ~~February 21, 2020~~ March 1, 2020 (23:59 [AoE](https://www.timeanddate.com/time/zones/aoe)) |
|----------------------|-------------------|
| Notification date:   | ~~March 13, 2020~~ March 20, 2020    |
| Camera-Ready:        | March 27, 2020    |
| Workshop:            | April 27, 2020    |
