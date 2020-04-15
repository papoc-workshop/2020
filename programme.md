---
title: Programme
---

Participating in the PaPoC workshop
-----------------------------------

We will use the [Zoom](https://zoom.us/) videoconferencing software to hold the PaPoC workshop online.
The workshop will take place on April 27, 2020, during daytime hours in European time zones.
Anybody is welcome to participate in the workshop; advance registration through EuroSys will be required (free of charge).
We will post details on how to register here once they are available.


Keynote
-------

The keynote at PaPoC will be given by [**Hagit Attiya**](https://hagit.net.technion.ac.il/)
(Professor, The Harry W. Labov and Charlotte Ullman Labov Academic Chair, Faculty of Computer Science, Technion, Israel).

**Abstract:**

Modern replicated data stores aim to provide high availability, by immediately responding to client
requests, often by implementing objects that expose concurrency and do not have a sequential
specification, like multi-valued registers (MVRs). We explore a recent model for replicated data
stores that can be used to precisely specify causal consistency for such objects, and liveness
properties like eventual consistency, without depending on details of the underlying implementation.
The model is used to prove what is the strongest consistency model that can be supported by an
eventually consistent data store implementing MVRs, for a large class of protocols. For the same
class, we prove that an eventually consistent and causally consistent replicated data store must
send messages of unbounded size.

We further specify the list object, modeling the core functionality of replicated data stores for
collaborative text editing and allowing users to concurrently edit a shared document, inserting and
deleting elements (e.g., characters or lines). A major factor determining the efficiency and
practical feasibility of a collaborative text editing protocol is the space overhead of its
metadata. We prove that for a large class of protocols implementing a list, this space overhead is
at least linear in the number of elements deleted from the list. A protocol in this class almost
matches the lower bound.


Accepted Papers
---------------

Schedule coming soon.

* **The Intrinsic Cost of Causal Consistency**

  Albert van der Linde, Pedro Fouto, João Leitão, and Nuno Preguiça (NOVA LINCS, DI - FCT - UNL)

* **Preserving Reciprocal Consistency in Distributed Graph Databases**

  Jack Waudby, Paul Ezhilchelvan (Newcastle University), Jim Webber (Neo4j), and Isi Mitrani (Newcastle University)

* **Orion: Time Estimated Causally Consistent Key-Value Store**

  Diptanshu Kakwani and Rupesh Nasre (IIT Madras)

* **Moving Elements in List CRDTs**

  Martin Kleppmann (University of Cambridge)

* **A Low-Cost Set CRDT Based on Causal Lengths**

  Weihai Yu and Sigbørn Rostad (The Arctic University of Norway)

* **AutoCouch: A JSON CRDT Framework**

  Pascal Grosch, Roman Krafft, Marcel Wölki, and Annette Bieniusa (TU Kaiserslautern)

* **Chronofold: a data structure for versioned text**

  Victor Grishchenko and Mikhail Patrakeev (N.N. Krasovskii Institute of Mathematics and Mechanics)

* **Paxos vs Raft: Have we reached consensus on distributed consensus?**

  Heidi Howard and Richard Mortier (University of Cambridge)

* **Efficient Renaming in Sequence Conflict-Free Replicated Data Types**

  Matthieu Nicolas, Gérald Oster, and Olivier Perrin (Université de Lorraine)

* **PushPin: Towards Production-Quality Peer-to-Peer Collaboration**

  Peter van Hardenberg (Ink & Switch) and Martin Kleppmann (University of Cambridge)

* **On combining fault tolerance and partial replication with causal consistency**

  Albert van der Linde, Diogo Serra, João Leitão, and Nuno Preguiça (NOVA LINCS, DI - FCT - UNL)

* **Flec: a versatile programming framework for eventually consistent systems**

  Jim Bauwens and Elisa Gonzalez Boix (Vrije Universiteit Brussel)

* **Low-Latency Geo-Replicated State Machines with Guaranteed Writes**

  Michael Eischer, Benedikt Straßner, and Tobias Distler (Friedrich-Alexander University Erlangen-Nürnberg)

* **Composing and Decomposing Op-Based CRDTs with Semidirect Products**

  Matthew Weidner, Heather Miller, and Christopher Meiklejohn (Carnegie Mellon University)
