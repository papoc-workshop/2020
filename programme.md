---
title: Programme
---

Participating in the PaPoC workshop
-----------------------------------

We will use the [Zoom](https://zoom.us/) videoconferencing software to hold the PaPoC workshop online.
The workshop will take place on April 27, 2020, during daytime hours in European time zones.
Anybody is welcome to participate in the workshop, but you must
[register in advance through EuroSys](https://www.eurosys2020.org/registration/) (free of charge).

Schedule times are given in [Central European Summer Time](https://www.timeanddate.com/time/zones/cest)
(CEST), and converted into your local time zone based on your web browser's settings. Please note
that CEST is not the same timezone as the workshop would have followed if it had taken place
physically in Crete.


Keynote
-------

09:30–10:15 CEST (<span class="schedule">07:30–08:15 UTC</span>)


* **Specification and complexity of replicated objects** [[abstract](#abstract-0)]

  [Hagit Attiya](https://hagit.net.technion.ac.il/) (Technion, Israel)

  <div id="abstract-0">
  <p><strong>Abstract:</strong></p>
  <p>Modern replicated data stores aim to provide high availability, by immediately responding to client
  requests, often by implementing objects that expose concurrency and do not have a sequential
  specification, like multi-valued registers (MVRs). We explore a recent model for replicated data
  stores that can be used to precisely specify causal consistency for such objects, and liveness
  properties like eventual consistency, without depending on details of the underlying implementation.
  The model is used to prove what is the strongest consistency model that can be supported by an
  eventually consistent data store implementing MVRs, for a large class of protocols. For the same
  class, we prove that an eventually consistent and causally consistent replicated data store must
  send messages of unbounded size.</p>
  <p>We further specify the list object, modeling the core functionality of replicated data stores for
  collaborative text editing and allowing users to concurrently edit a shared document, inserting and
  deleting elements (e.g., characters or lines). A major factor determining the efficiency and
  practical feasibility of a collaborative text editing protocol is the space overhead of its
  metadata. We prove that for a large class of protocols implementing a list, this space overhead is
  at least linear in the number of elements deleted from the list. A protocol in this class almost
  matches the lower bound.</p>
  </div>


Session 1: Databases and consensus
----------------------------------

10:30–11:30 CEST (<span class="schedule">08:30–09:30 UTC</span>)

* **Paxos vs Raft: Have we reached consensus on distributed consensus?**
  [[abstract](#abstract-1),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393681),
  [video](https://www.youtube.com/watch?v=JQss0uQUc6o)]

  Heidi Howard and Richard Mortier (University of Cambridge)

  <div id="abstract-1">
  <p><strong>Abstract:</strong></p>
  <p>Distributed consensus is a fundamental primitive for constructing fault-tolerant,
  strongly-consistent distributed systems. Though many distributed consensus algorithms have been
  proposed, just two dominate production systems: Paxos, the traditional, famously subtle,
  algorithm; and Raft, a more recent algorithm positioned as a more understandable alternative to
  Paxos.</p>
  <p>In this paper, we consider the question of which algorithm, Paxos or Raft, is the better
  solution to distributed consensus?  We analyse both to determine exactly how they differ  by
  describing a simplified Paxos algorithm using Raft's terminology and pragmatic abstractions.</p>
  <p>We find that both Paxos and Raft take a very similar approach to distributed consensus,
  differing only in their approach to leader election.  Most notably, Raft only allows servers with
  up-to-date logs to become leaders, whereas Paxos allows any server to be leader provided it then
  updates its log to ensure it is up-to-date.  Raft's approach is surprisingly efficient given its
  simplicity as, unlike Paxos, it does not require log entries to be exchanged during leader
  election.  We surmise that much of the understandability of Raft comes from the paper's clear
  presentation rather than being  fundamental to the underlying algorithm being presented.</p>
  </div>

* **Low-Latency Geo-Replicated State Machines with Guaranteed Writes**
  [[abstract](#abstract-2),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393686),
  [video](https://www.youtube.com/watch?v=eioQwMehKsw)]

  Michael Eischer, Benedikt Straßner, and Tobias Distler (Friedrich-Alexander University Erlangen-Nürnberg)

  <div id="abstract-2">
  <p><strong>Abstract:</strong></p>
  <p>When deployed in geo-distributed environments, existing state-machine replication protocols
  require at least one wide-area communication step for establishing a total order on client
  requests.  For use cases in which clients are not interested in the actual result of a request,
  but just need a guarantee that the request will be processed eventually, this property usually
  incurs unnecessarily high response times.  To address this problem we present Weave, a cloud-based
  geo-replication protocol that relies on replica groups in multiple geographic regions to
  efficiently assign stable sequence numbers to incoming requests.  This approach enables Weave to
  offer <em>guaranteed writes</em> which in the absence of faults only wait for communication within
  a client's local replica group to produce an execution guarantee for a particular sequence number.
  Our experiments with a distributed queue and a replicated log show that guaranteed writes can
  significantly improve response times of geo-replicated applications.</p>
  </div>

* **Preserving Reciprocal Consistency in Distributed Graph Databases**
  [[abstract](#abstract-3),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393675),
  [video](https://www.youtube.com/watch?v=n1JWPd-GCaQ)]

  Jack Waudby, Paul Ezhilchelvan (Newcastle University), Jim Webber (Neo4j), and Isi Mitrani (Newcastle University)

  <div id="abstract-3">
  <p><strong>Abstract:</strong></p>
  <p>Our earlier work identifies <em>reciprocal consistency</em> as an important property that must
  be preserved in distributed graph databases. It also demonstrates that a failure to do so
  seriously undermines the integrity of the database itself in the long term. Reciprocal
  consistency can be maintained as a part of enforcing any known isolation guarantee and such an
  enforcement is also known to lead to reduction in performance. Therefore, in practice, distributed
  graph databases are often built atop BASE databases with no isolation guarantees, benefiting from
  good performance but leaving them susceptible to corruption due to violations of reciprocal
  consistency. This paper designs and presents a lightweight, locking-free protocol and then
  evaluates the protocol's abilities to preserve reciprocal consistency and also offer good
  throughput. Our evaluations establish that  the protocol can offer both integrity guarantees and
  sound performance when the value of its parameter is chosen appropriately.</p>
  </div>


Session 2: Causal consistency
-----------------------------

12:30–13:30 CEST (<span class="schedule">10:30–11:30 UTC</span>)


* **Orion: Time Estimated Causally Consistent Key-Value Store**
  [[abstract](#abstract-4),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393676),
  [video](https://www.youtube.com/watch?v=xux0U1_1cmI)]

  Diptanshu Kakwani and Rupesh Nasre (IIT Madras)

  <div id="abstract-4">
  <p><strong>Abstract:</strong></p>
  <p>This paper presents a causally consistent key-value store Orion, which uses a novel protocol
  for Read Only Transactions (ROT). Unlike most of the existing protocols, Orion uses only one round
  of communication in the best case, and not more than two rounds in the worst case. We provide
  a theoretical bound on its communication complexity and qualitatively compare it with recent ROT
  protocols. We also quantitatively compare Orion with state-of-the-art protocol CausalSpartanX and
  illustrate that Orion achieves up to 1.7x higher throughput and generates 10x fewer messages on
  widely-used YCSB workload.</p>
  </div>

* **The Intrinsic Cost of Causal Consistency**
  [[abstract](#abstract-5),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393674),
  [video](https://www.youtube.com/watch?v=ymqEBG7BNXQ)]

  Albert van der Linde, Pedro Fouto, João Leitão, and Nuno Preguiça (NOVA LINCS, DI - FCT - UNL)

  <div id="abstract-5">
  <p><strong>Abstract:</strong></p>
  <p>In the last few years, causal consistency has become a popular consistency model for
  geo-replicated databases. The algorithms proposed to enforce causal consistency typically
  associate with each operation some metadata, which is used to guarantee that an operation is not
  executed if its execution would break causality. This may lead to the impression that causal
  consistency is intrinsically costly and non scalable.</p>
  <p>In this paper, we analyze the metadata costs of enforcing causal consistency and put these
  costs in perspective, considering the metadata that is necessary to enforce reliability. We show
  that by wisely ordering the propagation of operations it is possible to enforce causal consistency
  without any additional metadata other than the already necessary to enforce reliability.</p>
  </div>

* **On combining fault tolerance and partial replication with causal consistency**
  [[abstract](#abstract-6),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393684),
  [video](https://www.youtube.com/watch?v=-1VrGa3y-bU)]

  Albert van der Linde, Diogo Serra, João Leitão, and Nuno Preguiça (NOVA LINCS, DI - FCT - UNL)

  <div id="abstract-6">
  <p><strong>Abstract:</strong></p>
  <p>The purpose of this paper is to discuss the limitations imposed by introducing fault-tolerance
  in a partial replication system which aims to provide causal consistency.</p>
  <p>The general outcome is that, to provide support for indefinite replica-failure, the notion of
  partial in partial replication becomes not-really-partial-at-all.  We prove that to implement
  causal consistency when indefinite replica-failures are possible, it is impossible to respect the
  concept of genuine partial replication -- not storing or propagating operations which are on
  objects a given replica does not replicate locally.</p>
  <p>In our initial approach to tackle this issue client replicas need only to replicate the
  operations they depend on which have not yet been marked as durable by the centralised component.
  We discuss remaining limitations and expected improvements in future work.</p>
  </div>


Session 3: CRDT algorithms (1)
------------------------------

14:30–15:30 CEST (<span class="schedule">12:30–13:30 UTC</span>)


* **Chronofold: a data structure for versioned text**
  [[abstract](#abstract-7),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393680),
  [video](https://www.youtube.com/watch?v=YcZQzvxC05k)]

  Victor Grishchenko and Mikhail Patrakeev (N.N. Krasovskii Institute of Mathematics and Mechanics)

  <div id="abstract-7">
  <p><strong>Abstract:</strong></p>
  <p>Chronofold is a replicated data structure for versioned text, based on the extended Causal Tree
  model. Past models of this kind either retrofitted local linear orders to a distributed system
  (the OT approach) or employed distributed data models locally (the CRDT approach). That caused
  either extreme fragility in a distributed setting or egregious overheads in local use. Overall,
  that local/distributed impedance mismatch is cognitively taxing and causes lots of complexity. We
  solve that by using subjective linear orders locally at each replica, while inter-replica
  communication uses a distributed model. A separate translation layer insulates local data
  structures from the distributed environment. We modify the Lamport timestamping scheme to make
  that translation as trivial as possible. We believe our approach has applications beyond the
  domain of collaborative editing.</p>
  </div>

* **Efficient Renaming in Sequence Conflict-Free Replicated Data Types**
  [[abstract](#abstract-8),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393682),
  [video](https://www.youtube.com/watch?v=uHMj-xzkNI8)]

  Matthieu Nicolas, Gérald Oster, and Olivier Perrin (Université de Lorraine)

  <div id="abstract-8">
  <p><strong>Abstract:</strong></p>
  <p>To achieve high availability, large-scale distributed systems have to replicate data and to
  minimise coordination between nodes. Literature and industry increasingly adopt Conflict-free
  Replicated Data Types (CRDTs) to design such systems. CRDTs are data types which behave as
  traditional ones, e.g. the Set or the Sequence. However, unlike traditional data types, they are
  designed to natively support concurrent modifications. To this end, they embed in their
  specification a conflict-resolution mechanism.</p>
  <p>To resolve conflicts in a deterministic manner, CRDTs usually attach identifiers to elements
  stored in the data structure. Identifiers have to comply with several constraints, such as
  uniqueness or belonging to a dense order. These constraints may hinder the identifiers’ size from
  being bounded. As the system progresses, identifiers tend to grow. This inflation deepens the
  overhead of the CRDT over time, leading to performance issues.</p>
  <p>To address this issue, we propose a new CRDT for Sequence which embeds a renaming mechanism.
  It enables nodes to reassign shorter identifiers to elements in an uncoordinated manner.
  Experimental results demonstrate that this mechanism decreases the overhead of the replicated data
  structure and eventually limits it.</p>
  </div>

* **Moving Elements in List CRDTs**
  [[abstract](#abstract-9),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393677),
  [video](https://www.youtube.com/watch?v=TYBV324NWNQ)]

  Martin Kleppmann (University of Cambridge)

  <div id="abstract-9">
  <p><strong>Abstract:</strong></p>
  <p>Conflict-free Replicated Data Types (CRDTs) for lists allow multiple users to concurrently
  insert and delete elements in a shared list object. However, existing algorithms behave poorly
  when users concurrently move list elements to a new position (i.e. reorder the elements in the
  list). We demonstrate the need for such a move operation, and describe an algorithm that extends
  a list CRDT with an explicit move operation. Our algorithm can be used in conjunction with any
  existing list CRDT algorithm. In addition to moving a single list element, we also discuss the
  open problem of moving ranges of elements.</p>
  </div>


Session 4: CRDT algorithms (2)
------------------------------

16:00–16:40 CEST (<span class="schedule">14:00–14:40 UTC</span>)


* **A Low-Cost Set CRDT Based on Causal Lengths**
  [[abstract](#abstract-10),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393678),
  [video](https://www.youtube.com/watch?v=l4JxlK8Qzvs)]

  Weihai Yu and Sigbørn Rostad (The Arctic University of Norway)

  <div id="abstract-10">
  <p><strong>Abstract:</strong></p>
  <p>CRDTs, or Conflict-free Replicated Data Types, are data abstractions that guarantee convergence
  for replicated data. Set is one of the most fundamental and widely used data types. Existing
  general-purpose set CRDTs associate every element in the set with causal contexts as meta data.
  Manipulation of causal contexts can be complicated and costly. We present a new set CRDT, CLSet
  (causal-length set), where the meta data associated with an element is simply a natural number
  (called causal length). We compare CLSet with existing general purpose CRDTs in terms of semantics
  and performance.</p>
  </div>

* **Composing and Decomposing Op-Based CRDTs with Semidirect Products**
  [[abstract](#abstract-11),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393687),
  [video](https://www.youtube.com/watch?v=jOGVp55VwO0)]

  Matthew Weidner, Heather Miller, and Christopher Meiklejohn (Carnegie Mellon University)

  <div id="abstract-11">
  <p><strong>Abstract:</strong></p>
  <p>Operation-based Conflict-free Replicated Data Types (CRDTs) are eventually consistent
  replicated data types that automatically resolve conflicts between concurrent operations.
  Op-based CRDTs must be designed differently for each data type, and current designs use ad-hoc
  techniques to handle concurrent operations that do not naturally commute. We present a new
  construction, the <em>semidirect product</em> of op-based CRDTs, which combines the operations of
  two CRDTs into one while handling conflicts between their concurrent operations in a uniform way.
  We demonstrate the construction's utility by decomposing several existing CRDTs as semidirect
  products of simpler CRDTs, as well as by using it to construct novel CRDTs. Although it
  reproduces common CRDT semantics, the semidirect product can be viewed as a restricted kind of
  operational transformation, thus forming a bridge between the two fields.</p>
  </div>


Session 5: CRDT systems
-----------------------

17:30–18:30 CEST (<span class="schedule">15:30–16:30 UTC</span>)

* **AutoCouch: A JSON CRDT Framework**
  [[abstract](#abstract-12),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393679),
  [video](https://www.youtube.com/watch?v=D2_irGwRpjc)]

  Pascal Grosch, Roman Krafft, Marcel Wölki, and Annette Bieniusa (TU Kaiserslautern)

  <div id="abstract-12">
  <p><strong>Abstract:</strong></p>
  <p>Most web-based applications require an undisrupted connection to some kind of server for
  updating the current application state and propagating changes made locally at the clients. By
  their very nature, CRDTs provide the right semantics for these applications as they resolve
  conflicts after concurrent state changes from different users or when a user reconnects after some
  period of unavailability. Although the JSON format is often used to summarize and represent the
  complete state of web applications, there is currently – to our knowledge – no generic integrated
  implementation of a JSON CRDT framework that supports the standard client-server setup for web
  apps.</p>
  <p>In this paper, we present the AutoCouch framework which combines the benefits of the Automerge
  CRDT library with the widely used CouchDB framework. It provides an out-of-the-box use of
  a conflict-free JSON document that is replicated on server side and in browsers on client side,
  while requiring few adaptations to provide smooth online/offline transitions for web apps.</p>
  </div>

* **Flec: a versatile programming framework for eventually consistent systems**
  [[abstract](#abstract-13),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393685),
  [video](https://www.youtube.com/watch?v=uIRU15TdR0g)]

  Jim Bauwens and Elisa Gonzalez Boix (Vrije Universiteit Brussel)

  <div id="abstract-13">
  <p><strong>Abstract:</strong></p>
  <p>Modern distributed applications increasingly replicate data in order to guarantee both high
  availability of systems and an optimal user experience. Conflict-Free Replicated DataTypes
  (CRDTs) are a family of data types specially designed for highly available systems which guarantee
  some form of eventual consistency. However, currently CRDT implementations are hard to integrate
  with existing applications and/or programming languages. In this extended abstract we describe
  Flec, a versatile programming framework for operation-based CRDTs that ultimately can be run in
  any environment supporting WebAssembly.</p>
  </div>

* **PushPin: Towards Production-Quality Peer-to-Peer Collaboration**
  [[abstract](#abstract-14),
  [paper](https://dl.acm.org/doi/abs/10.1145/3380787.3393683),
  [video](https://www.youtube.com/watch?v=u4bJIdVwZCQ)]

  Peter van Hardenberg (Ink & Switch) and Martin Kleppmann (University of Cambridge)

  <div id="abstract-14">
  <p><strong>Abstract:</strong></p>
  <p>Fully peer-to-peer application software promises many benefits over cloud software, in
  particular, being able to function indefinitely without requiring servers. Research on
  distributed consistency mechanisms such as CRDTs has laid the foundation for P2P data
  synchronisation and collaboration. In this paper we report on our experience in taking these
  technologies beyond research prototypes, and working towards commercial-grade P2P collaboration
  software. We identify approaches that work well in our experience, such as the functional
  reactive programming paradigm, and highlight areas in need of further research, such as the
  reliability of NAT traversal and usability challenges.</p>
  </div>


<script>
// Hide or show abstracts when clicking on links
for (let link of document.querySelectorAll('a[href^="#abstract-"]')) {
  link.addEventListener('click', (event) => {
    event.preventDefault();
    const id = event.target.getAttribute('href').replace(/^#/, '');
    document.body.classList.toggle('show-' + id);
  });
}

function twoDigit(number) {
  return number.toLocaleString('en-US', {minimumIntegerDigits: 2, useGrouping:false});
}

// Time zone conversion of schedule times
for (let session of document.querySelectorAll('span.schedule')) {
  let [_, hourStart, minStart, hourFinish, minFinish] = session.innerText.match(/^([0-9]+):([0-9]+)–([0-9]+):([0-9]+) UTC/);
  let start  = new Date(Date.UTC(2020, 3, 27, parseInt(hourStart),  parseInt(minStart)));
  let finish = new Date(Date.UTC(2020, 3, 27, parseInt(hourFinish), parseInt(minFinish)));
  session.innerText = [
    twoDigit(start .getHours()), ':', twoDigit(start .getMinutes()), '–',
    twoDigit(finish.getHours()), ':', twoDigit(finish.getMinutes()), ' ',
    Intl.DateTimeFormat().resolvedOptions().timeZone
  ].join('');
}
</script>
