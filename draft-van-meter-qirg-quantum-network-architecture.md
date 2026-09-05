---
stand_alone: true
ipr: trust200902
cat: info
submissiontype: IRTF
area: IRTF
wg: QIRG

docname: draft-van-meter-qirg-quantum-network-architecture-latest
pi: [toc, sortrefs, symrefs]

title: A Quantum Network Architecture
abbrev: QNA
lang: en
kw:
  - network architecture
  - quantum repeater
# date: 2022-02-02 -- date is filled in automatically by xml2rfc if not given

venue:
#  group: WG
#  type: Working Group
#  mail: WG@example.com
#  arch: https://example.com/WG
  github: "moonshot-nagayama-pj/draft-van-meter-qirg-quantum-network-architecture"
  latest: "https://moonshot-nagayama-pj.github.io/draft-van-meter-qirg-quantum-network-architecture/draft-van-meter-qirg-quantum-network-architecture.html"

author:
- ins: R. Van Meter
  name: Rodney Van Meter
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  email: rdv@sfc.wide.ad.jp
- ins: N. Benchasattabuse
  name: Naphan Benchasattabuse
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  email: whit3z@sfc.wide.ad.jp
- ins: A. Taherkhani
  name: Amin Taherkhani
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  email: amin@sfc.wide.ad.jp
contributor: # Same structure as author list, but goes into contributors
- ins: M. Hajdusek
  name: Michal Hajdusek
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  contribution: |
    Michal was involved in document development and technical discussions from the beginning.
- ins: A. Todd
  name: Andrew Todd
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  contribution: |
    Andrew leads the software team implementing much of the network, and provides feedback on system structure.
- ins: M. Tokuyama Friedrich
  name: Monet Tokuyama Friedrich
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  contribution: |
    Contributed presentations and clarity; reviewed this document; authoring related specifications.
- ins: S. Nagayama
  name: Shota Nagayama
  org: Keio University
  street: 5322 Endo, Fujisawa
  region: Kanagawa
  code: 252-0882
  country: JP
  contribution: |
      Contributed presentations and clarity; reviewed this document and related documents; technical and managerial leadership.
- ins: A. Soeda
  name: Akihito Soeda
  org: National Institute for Informatics
  street: 2-1-2 Hitotsubashi, Chiyoda-ku
  region: Tokyo
  code: 101-8430
  country: JP
  contribution: |
      Technical and managerial discussions.

# bugfix for umlaut and quotes in title & author list
entity:
  uuml: ü
  ldquo: “
  rdquo: ”

normative:

informative:
  RFC1122:
  RFC1123:
  RFC1958:
  RFC5218:
  RFC6250:
  RFC6852:
  RFC9340:
  RFC9413:
  RFC9583:
  I-D.draft-dahlberg-ll-quantum:
  I-D.draft-hajdusek-qirg-timing-physics:
  I-D.draft-kaws-qirg-advent:
  I-D.draft-zhu-qirg-qdcp:
  res-mgmt-het:
    target: https://aqua.sfc.wide.ad.jp/publications/whit3z-thesis-local-compiled.pdf
    title: Resource Management in Heterogeneous Quantum Repeater Networks
    author:
        ins: N. Benchasattabuse
        name: Naphan Benchasattabuse
        org: Keio University
    date: 2025
    seriesinfo:
      "Ph.D.": "Dissertation, Keio University"
    format:
      PDF: https://aqua.sfc.wide.ad.jp/publications/whit3z-thesis-local-compiled.pdf
  rdv-thesis:
    target: https://arxiv.org/abs/quant-ph/0607065
    title: Architecture of a Quantum Multicomputer Optimized for Shor's Factoring Algorithm
    author:
        ins: R. D. Van Meter III
        name: Rodney Doyle Van Meter III
        org: Keio University
    date: 2006
    seriesinfo:
      "Ph.D.": "Dissertation, Keio University"
    format:
      PDF: https://arxiv.org/pdf/quant-ph/0607065
  nist-singles: DOI.10.6028/NIST.IR.8486r1
  abane-routing: DOI.10.48550/arXiv.2408.01234
  aboy-governance: DOI.10.1126/science.adw0018
  ambainis-multiparty-coin: DOI.10.1109/CCC.2004.1313848
  aparicio-spie: DOI.10.1117/12.893272
  awschalom-roadmap: DOI.10.2172/1900586
  azuma-rmp: DOI.10.1103/RevModPhys.95.045006
  azuma-rgs: DOI.10.1038/ncomms7787
  BB84: DOI.10.1016/j.tcs.2014.05.025
  BBM92: DOI.10.1103/PhysRevLett.68.557
  bennett-mixed: DOI.10.1103/PhysRevA.54.3824
  broadbent-bfk-protocol: DOI.10.1109/FOCS.2009.36
  bugalho-dist-multipartite: DOI.10.22331/q-2023-02-09-920
  buterakos-graph-generation: DOI.10.1103/PhysRevX.7.041023
  choi-fat-tree: DOI.10.48550/arXiv.2306.09216
  christandl-anon: DOI.10.1007/11593447_12
  degen-sensing: DOI.10.1103/RevModPhys.89.035002
  dahlberg-ll-arxiv: DOI.10.48550/arXiv.1903.09778
  dally-towles:
      title: Principles and Practices of Interconnection Networks
      author:
      -
        ins: W. J. Dally
        name: William James Dally
      -
        ins: B. P. Towles
        name: Brian Patrick Towles
      date: 2004
      seriesinfo:
        ISBN: 978-0-08-049780-8
  divincenzo-criteria: DOI.10.48550/arXiv.quant-ph/0002077
  delle-donne-os-arxiv: DOI.10.48550/arXiv.2407.18306
  delle-donne-os-nature: DOI.10.1038/s41586-025-08704-w
  delle-donne-thesis:
    target: https://pure.tudelft.nl/ws/portalfiles/portal/153555360/dissertation_cdelledonne.pdf
    title: Software Abstractions for Programmable Quantum Network Nodes
    author:
        ins: C. Delle Donne
        name: Carlo Delle Donne
        org: Technical University of Delft
    date: 2023
    seriesinfo:
      "Ph.D.": "Dissertation, Technical University Delft"
    format:
      PDF: https://pure.tudelft.nl/ws/portalfiles/portal/153555360/
  drost: DOI.10.1364/JOCN.8.000331
  dulek-homomorphic: DOI.10.4086/toc.2018.v014a007
  dur-w-state: DOI.10.1103/PhysRevA.62.062314
  E91: DOI.10.1103/PhysRevLett.67.661
  fan-dgs-dist: DOI.10.1109/TQE.2025.3552006
  farhadi-sdn: DOI.10.1016/j.comnet.2015.02.014
  fischer-dgs: DOI.10.1109/QCE52317.2021.00049
  fittipaldi-sat: DOI.10.1109/QCE60285.2024.00222
  fitzsimons-blind: DOI.10.1038/s41534-017-0025-3
  ge-linear: DOI.10.1103/PhysRevLett.121.043604
  ghz: DOI.10.48550/arXiv.0712.0921
  giovannetti-metro: DOI.10.1038/nphoton.2011.35
  gottesman-telescope: DOI.10.1103/PhysRevLett.109.070503
  haener-qmpi: DOI.10.1145/3458817.3476172
  ilo-okeke-clock: DOI.10.1038/s41534-018-0090-2
  hajdusek-qcomm: DOI.10.48550/arXiv.2311.02367
  haldar-sat-dist: DOI.10.1103/PhysRevA.107.022615
  hein-multiparty: DOI.10.1103/PhysRevA.69.062311
  hein-graph-entanglement: DOI.10.3254/978-1-61499-018-5-115
  hilaire-logical-bsm: DOI.10.1103/PhysRevA.104.052623
  hilaire-rgs-optimizing-gen-time: DOI.10.22331/q-2021-02-15-397
  horsman-lattice-surgery: DOI.10.1088/1367-2630/14/12/123011
  huang-imaging-stars: DOI.10.1103/PhysRevLett.129.210502
  humphreys-deterministic-link: DOI.10.1038/s41586-018-0200-5
  khatri-spooky: DOI.10.1038/s41534-020-00327-5
  kim-ft-million: DOI.10.1145/3620665.3640388
  koyama-24: DOI.10.1109/QCE60285.2024.00219
  leone-remote: DOI.10.48550/arxiv.2406.18764
  li-cosmic: DOI.10.1038/s41467-025-59778-z
  litinski-gosc: DOI.10.22331/q-2019-03-05-128
  mahadev-homomorphic: DOI.10.1137/18M1231055
  martinis-correlated: DOI.10.1038/s41534-021-00431-0
  mayers-unconditional: DOI.10.48550/arXiv.quant-ph/9802025
  mccanne-bpf:
      title: "The BSD packet filter: a new architecture for user-level packet capture"
      author:
      -
        ins: S. McCanne
        name: Steven McCanne
      -
        ins: V. Jacobson
        name: Van Jacobson
      date: 1993-01-25
      rc: "USENIX'93: Proceedings of the USENIX Winter 1993 Conference Proceedings on USENIX Winter 1993 Conference Proceedings"
  meignant-dgs: DOI.10.1103/PhysRevA.100.052333
  mori-psds: DOI.10.1109/QCE60285.2024.00218
  morimae-blind: DOI.10.1103/PhysRevA.87.050301
  muralidharan-generations: DOI.10.1038/srep20463
  proctor-quantum-sensing: DOI.10.48550/arXiv.1702.04271
  proctor-multiparm: DOI.10.1103/PhysRevLett.120.080501
  ramette-remote: DOI.10.1038/s41534-024-00855-4
  sakuma-q-fly: DOI.10.48550/arXiv.2412.09299
  sane-jobs: DOI.10.48550/arXiv.2504.18298
  sane-phonons: DOI.10.1109/QCE57702.2023.00156
  satoh-attacking: DOI.10.1109/TQE.2021.3094983
  schoute-shortcuts: DOI.10.48550/arXiv.1610.05238
  shapourian-qdc-infra: DOI.10.48550/arXiv.2501.05598
  sinclair-ft-interconnect: DOI.10.48550/arxiv.2408.08955
  sutcliffe-dist-qec: DOI.10.1109/QCE65121.2025.00076
  taherkhani-byz: DOI.10.1088/2058-9565/aa9bb1
  van-meter-opt-timing: DOI.10.48550/arXiv.1701.04586
  van-meter-path-sel: DOI.10.1007/s13119-013-0026-2
  van-meter-qi-arch: DOI.10.1109/QCE53715.2022.00055
  van-meter-q-net-book: DOI.10.1002/9781118648919
  van-meter-sys-design: DOI.10.1109/TNET.2008.927260
  I-D.draft-van-meter-qirg-quantum-connection-setup:
  vepsaelaeinen-ionizing: DOI.10.1038/s41586-020-2619-8
  wu-mitigating: DOI.10.1103/4ctq-r6w6
  xu-dist-qec: DOI.10.1103/PhysRevLett.129.240502
  yin-1200km: DOI.10.1126/science.aan3211
  yoder-tour-de-gross: DOI.10.48550/arXiv.2506.03094
  zukowski-entanglement-swapping: DOI.10.1103/PhysRevA.65.032118
...

--- abstract

This quantum network architecture defines a set of planes providing different views of the network, supporting different responsibilities and modes of operation; a set of device, node and link types; some network topologies, deployment scenarios and their relationship to applications; and key design decisions as a result of corresponding requirements.

--- middle

# Introduction

This document introduces the key architectural decisions, classical and quantum communication systems, and main node types for several classes of quantum networks.

We define the verb _to architect_ as: within a set of environmental constraints, using a set of building blocks, design a system that satisfies a need, elegantly and economically.
We use the noun _architecture_ as: the set of blocks or subsystems, their roles and their interfaces and their overall arrangement, that defines the system. This architecture defines the overall structure, and is connected to a specific implementation as an example.

For a description of the key concepts in quantum networks and additional references, see {{RFC9340}} and the book _Quantum Communications_ {{hajdusek-qcomm}}.

For more background and discussion of the design choices in this architecture, see the Ph.D. dissertation of Naphan Benchasattabuse [res-mgmt-het].

# Requirements Language

{::boilerplate bcp14-tagged}

# Goals and Non-Goals of this Document

This section describes goals and non-goals for this document itself, rather than the technical goals and requirements for a network.

## Goals

* To define the principal concepts in a quantum network, principally for quantum multicomputer interconnects but also data center and wide-area networks where possible.
* To enumerate some of the key architectural decisions for this architecture.
* To describe how device, link and node types are defined.
* To provide a guide to other documents.

## Non-Goals

* Specification of physical links
* Internetworking

# Relationship to Documents by QIRG and Other Organizations

Other organizations, including national laboratories and standards development organizations, are developing documents describing quantum networks and quantum computing technology. These are mostly _pre-standardization_ documents, not yet on any formal standardization track. To the extent possible, this document conforms to their terminology. However, as this document describes a specific quantum network architecture, it does not attempt to conform to specific design decisions made in other contexts.  See an August 2025 Science Policy Forum {{aboy-governance}} for additional discussion of some standardization efforts and their value.

Some of these are listed here for reference:

* ETSI
    - [Industry Specification Group (ISG) on Quantum Key Distribution (QKD)](https://www.etsi.org/committee/qkd)
* IEEE Standards Association
    - [IEEE Standards & Projects for Quantum Technologies](https://standards.ieee.org/initiatives/quantum-standards-activities/)
    - [Standardization Roadmap on Quantum Applications](https://ieee-sa.imeetcentral.com/p/eAAAAAAASqm9AAAAAFU6etg)
* ISO
    - [IEC/ISO JTC 3 Quantum technologies](https://www.iso.org/committee/10138914.html)
* ITU-T
    - [ITU-T Focus Group on Quantum Information Technology for Networks (FG-QIT4N)](https://www.itu.int/en/ITU-T/focusgroups/qit4n/Pages/default.aspx)
    - [Y.3800 series](https://www.itu.int/itu-t/recommendations/index.aspx?ser=Y) on quantum key distribution networks
* National Institute of Standards and Technology (NIST)
    - Single-Photon Sources and Detectors Dictionary {{nist-singles}}
* [Quantum Internet Research Group (QIRG)](https://datatracker.ietf.org/group/qirg/about/) (part of IRTF)
    - {{RFC9340}}
    - {{RFC9583}}

# Prerequisite Knowledge

This document assumes basic knowledge of the underlying technology and goals of quantum communications.  The following list of topics may help readers who are not yet familiar with the concepts.

* Linear algebra
* Quantum information basics
    - Dirac ket notation
    - von Neumann density matrix notation
    - Superposition
    - Entanglement
    - Interference
    - Unitary operation
    - Measurement
    - Decoherence
    - No-cloning theorem
    - Clifford group
    - Basics of quantum error correction (QEC)
* Classical Internet-family networking
* Quantum networking
    - Teleportation
    - Purification
    - Entanglement swapping
    - Quantum key distribution {{BB84}}, {{E91}}, {{BBM92}}
    - "Generations" of quantum repeaters {{muralidharan-generations}}, {{azuma-rmp}}
    - (Repeater graph states may be helpful, but are not used in the current architecture)

Because terms such as _fidelity_ have varying definitions, they will be defined in this set of documents (where? Timing Regimes?).

Readers needing additional background are referred to:

* {{RFC9340}}
* {{RFC9583}}
* Van Meter, _Quantum Networking_ {{van-meter-q-net-book}}
* Hajdusek and Van Meter, _Quantum Communications_ {{hajdusek-qcomm}}

# Terminology

In this document, we use the abbreviations and other related technical terms listed in the following table:

| Term | Description |
| ---- | ----------- |
| BSA | Bell state analyzer, generally optical and incorporating one or more beamsplitters and either two or four single-photon detectors |
| CRQC | cryptographically relevant quantum computer |
| device | manipulates photons in some fashion; a component of a node |
| FASQ | fault-tolerant application-scale quantum |
| fidelity | measures how close a quantum state is to the state we have tried to create. Varies between 0 and 1, with unit fidelity indicating the actual state is the same as the desired state. It expresses the probability that the state will behave exactly the same as our desired state. (adapted from RFC 9340) |
| FTQC | fault-tolerant quantum computer |
| group switch | In the Q-Fly architecture, the set of devices that connect the end nodes to the pool of BSAs, and the group to other groups |
| NISQ | near-term intermediate-scale quantum |
| node | a self-contained subsystem with a clear boundary that is visible to other such nodes as a single entity on one or more planes |
| optical mode | roughly, a place and time that a photon might be, which may be occupied by some, all or none of the amplitude of a single photon. More accurately, it is a field distribution obtained from solving Maxwell's equations given some boundary conditions. An optical mode is an eigensolution of the wave equation given the physical properties of the waveguide (dimensions, refractive index). It is a particular field distribution that can propagate through the waveguide. The state of a single photon can be expressed as a coherent superposition of such optical modes. For optics engineers, a 'mode' (or optical mode to be more precise) refers to a specific spatiotemporal distribution of electromagnetic field fluctuation. For quantum network engineers, especially those that would most likely be reading RFCs, two optical detectors are detecting different optical modes if one detector can be activated by light without activating the other. In that case, it is not wrong to say that the two detectors are detecting two independent optical modes. |
| path | the set of nodes and links that a connection passes through, including the end points |
| plane (architectural) | a view of the entire network for a particular purpose, such as management or data transmission |
| plane (optical) | a defined plane in physical space through which a photon passes; also referred to as a surface |
| QBER | quantum bit error rate |
| QNIC | quantum network interface card; in practice, the physical interface to a link plus the set of quantum memories under the control of the network stack. |
| QPU | quantum processing unit |
| RuleSet | a set of SDN-inspired, event-driven, short, real-time or near-real time, near-determininistic programs executed at nodes along a path to build application-requested entangled states |
| SNSPD | Superconducting Nanowire Single Photon Detector |
| multiqubit Pauli operators | tensor product of Pauli operators acting on two or more qubits |
| switch point | a 2x2 junction that can be either X (cross) or = (straight) |
| switch device | a single integrated, fiber- or free space-connected (physical) component, comprising one or more switch points |
| teledata | application execution via teleporting data from node to node, then executing gates locally.  May be done remotely, mediated by Bell pairs. |
| telegate | application execution via remote gates (as defined by Eisert et al.).  May be done remotely, mediated by Bell pairs. |
| time bin | compare to window and time slot |
| time slot | compare to window and time bin |
| window | compare to time bin and time slot |

# Applications of Networks

The requirements for a network are determined by the application workload.  This section orients architectural decisions by briefly introducing applications and the communication patterns they exhibit, which is a key factor determining the suitability of particular architectures.

## Types of Applications

Applications fall into two large categories: inherently distributed applications, or subdivision of monolithic applications for distributed execution, as in supercomputing applications running on multicomputer architectures.

For a discussion of some inherently distributed applications of quantum networks, see {{RFC9583}}. This network architecture supports the applications listed in that RFC, though not all networks will support all applications.

## Entangled States Consumption Patterns

The text in this section is adapted and extended from unpublished text in {{van-meter-opt-timing}}.

Distinct from the classification of quantum repeater generations by Muralidharan et al. {{muralidharan-generations}}, one can categorize distributed quantum systems by how applications interface with the network; specifically, the timing at which network interface qubits are freed after attempting entangled state generation.

In the early days of quantum information research, Bennett et al. recognized {{bennett-mixed}} that the component qubits of an entangled state may be held at different times in different locations, termed _time-separated Bell pairs_.
Based on this principle, we can describe the timeline of information availability between two nodes.
This model assumes entangled states are requested dynamically during execution, rather than pre-caching entangled states　{{schoute-shortcuts}} for immediate consumption.

### The Entanglement Information Timeline

The lifecycle of an entanglement request, from initiation to full state knowledge, follows three distinct stages:

1. **Attempt:** The entangled states are requested.
For memory-based links, this corresponds to the quantum memory emitting a photon and transmitting it through the link.
1. **Heralded:** The entangled states are physically established, but the specific states are unknown.  The node has received confirmations that photons arrived at the BSA and the BSM succeeded, but the Pauli frame information is not yet available.  Without this information, an entangled state will be _fully mixed_, with a fidelity of 0.25 for a two-qubit state.
1. **Correct:** The classical message regarding the Pauli frame arrives.
The node now knows the exact entangled state created and can apply corrections (or software frame updates) to align with the expected state.

### Classification of Consumption Patterns

Based on the timeline above, we classify Bell pair consumption into three classes {{van-meter-opt-timing}}.
These classes are defined by whether the application must **block execution** while waiting for information at the _Heralded_ or _Correct_ stages.
Note that the term "blocking" here refers to the blocking versus non-blocking execution models, similar to kernel-level I/O blocking or the event-driven programming paradigm, and is distinct from the concept of blocking in network switches.

| Class | Wait for Heralding? | Wait for Pauli Frame? | Application Behavior |
| :---- | :------------------ | :-------------------- | :------------------- |
| **Unentangled State Tolerant (B)** | No | No | **Non-Blocking:** The application consumes the qubit immediately, handling failures or corrections in post-processing. |
| **Reactive Correction (C)** | Yes* | No | **Partially Blocking:** The application waits only for confirmation of existence (heralding), then proceeds by tracking errors in software. |
| **Deterministic (T)** | Yes | Yes | **Strictly Blocking:** The application blocks until the state is fully verified and corrected. |

_\*Note for Class C: If the link is fully deterministic (guaranteeing success), the application does not need to pause for heralding and become non-blocking._

### Class Selection and Resource Implications

It is important to note that these classes are determined by the **nodes**, not the network.
The application nodes assess their own capabilities (number of buffer memories, gate and qubit error rate) and the network's performance (fidelity, rate, success probability) to select the appropriate operating class.

The selection of a class significantly impacts network resource utilization.
For example, if a node possesses sufficient buffer memory, it may elect to operate in **Class B** from the perspective of the network interface.
By moving the entangled state from the communication qubit to storage immediately (or measuring it immediately), the node frees up the network interface to service other requests.
This reduces the workload on the network and increases the repetition rate, even if the application logic itself eventually requires the data for a Class T operation.

### Unentangled State Tolerant (B Class) Applications

The defining characteristic of B Class applications is the ability to consume the (potential) entangled states immediately without waiting (fully non-blocking).
The application effectively takes over the burden of validation from the network.

**Execution Flow:** The application does not stop.
It measures or stores the qubit immediately.
If the entanglement attempt failed (information received later), the data is discarded or treated as an erasure error.

**Examples:**

* **Classical Correlation:** Applications like Quantum Key Distribution (QKD) protocols (e.g., E91) or link fidelity estimation.
The application filters out failed attempts during classical post-processing.

* **Fault-Tolerant Operations:** Certain remote quantum error correction schemes, such as remote lattice surgery {{horsman-lattice-surgery}}, {{ramette-remote}}, {{leone-remote}}, {{sinclair-ft-interconnect}} of the surface code.
If the probability of creating a link is high enough, unsuccessful attempts can be treated as depolarizing errors, which the logical code can tolerate without stalling the pipeline.

### Reactive Correction (C Class) Applications

In C Class applications, the system requires confirmation that a link exists, but does not wait for the state details.
The application proceeds by assuming a specific Bell state and managing deviations via software tracking.

**Execution Flow:** The application pauses briefly to ensure the Bell pair is _Heralded_.
Once confirmed, it executes immediately.
It does not wait for the _Correct_ stage (Pauli frame); instead, it uses a "Pauli Frame Tracker" to propagate the necessary corrections through the circuit virtually.
If the network link is deterministic, the specific wait for heralding is removed, as the node assumes success by default.

**Examples:** Clifford circuit execution, distributed Pauli-based computation with time-optimal scheme {{litinski-gosc}}, and state teleportation.

### Deterministic (T Class) Applications

T Class applications impose the strictest timing constraints, requiring the entangled state to idle the longest before being consumed.

**Execution Flow:** The application **completely stalls**.
It must wait until the network provides both the confirmation of creation (_Heralded_) and the specific state information (_Correct_).
Execution only resumes once the exact state is known or corrected.

**Examples:** Execution of circuits involving non-Clifford gates. While non-Clifford operations _can_ theoretically be corrected post hoc (similar to Class C), doing so often requires consuming _additional_ entangled states to fix the error.
Since consuming extra resources is more costly than waiting, these operations default to Class T to ensure the state is correct before proceeding.

# Architectural Concepts

This section introduces concepts in classical and quantum computer and network architecture that may be unfamiliar, or that have a specific role in this network architecture.

## Quantum Devices

A quantum device stores, carries, measures or computes on quantum variables.

A quantum device (often shortened to just "device" in this specification) is under software control; i.e. optical fibers or beam splitters are not classified as quantum devices.

Control of devices is usually done with respect to some physical characteristic of the device itself, rather than dealing with the abstract notion of qubits.  A controllable wave plate, for example, may be adjusted in units of degrees of rotation of the plate.  An example of a software package that provides such functionality is PnPQ.

## Quantum Nodes

A node comprises one or more quantum devices, and serves as a single locus of control for network protocols.  The classes of nodes are described later in this document.

A _logical node_ or _composite node_ provides a single communication and control point for the services of a particular node type or a composite node type, but may comprise a set of physical devices rather than a single device, and may be physically packaged in more than one box.

## Quantum Links

Links are described in {{links}}.

## Photonic Synchronization Domains

A photonic synchronization domain (PSD) is the range of devices and channels (fiber or free space) over which photons must be controlled with high precision in order to effect e.g. photonic entanglement swapping {{mori-psds}}. The primary concern of a PSD is getting photons to arrive at beamsplitters "simultaneously", with sufficient overlap in their wavepackets, as specified in {{I-D.draft-hajdusek-qirg-timing-physics}}.

Note that the most common operational mode uses only pairs of photons, one from each of two nodes, not multi-photon operations; the definition of PSD does not imply that all channels in a network must be synchronized with each other and used in a single operation.

## Direct and Indirect Multicomputer Architectures

In multicomputer architectures, a _direct_ architecture features links that go directly from computational node to computational node. Hypercubes, meshes and toruses are typically direct architectures.  An _indirect_ architecture interposes one or more switches between computational nodes.  Fat trees, Clos and Benes networks, and the various -fly topologies are generally indirect {{dally-towles}}.

The distinction is somewhat artificial in that direct architectures sometimes incorporate a small switch inside the node, in which case the matching term depends on where you draw the boundary of the node, and because computational nodes can be configured to act only as routers within the network, modeling an indirect architecture using direct hardware.

## Detector-centric Architecture

Several detectors may be packaged as a single subsystem for purposes such as cooling, power, control and time stamping.  An architecture built around a shared pool of detectors is a _detector-centric architecture_. This structure facilities entanglement distribution in a quantum system interconnect, data center network or some forms of local area network.

A detector-centric architecture is an indirect architecture if the pool of detectors is behind a switch or network of switches.

## Source-centric Architecture

Many of the detector-centric network topologies can be inverted, such that the pool of detectors is replaced by a pool of entangled photon pair sources.  The network then is used to distribute entanglement, with the photons measured, absorbed into memories, interfered with locally generated photons, or otherwise utilized at or near the end nodes.  Such a network was proposed by Drost _et al._ {{drost}}.

# A Sketch of the System Model

As noted in the 2022 roadmap for quantum interconnects {{awschalom-roadmap}}, entangled quantum network technology can be deployed in a variety of scenarios with different requirements and assumptions. A full description of each of these is delegated to other documents, but a brief description here will help to orient discussions of design points in order to justify certain decisions.

## Multicomputer

The first deployment of production-level, distant quantum entanglement is likely to be in a _quantum multicomputer_, based on the same principles as classical distributed-memory supercomputers from the [Caltech Cosmic Cube](https://en.wikipedia.org/wiki/Caltech_Cosmic_Cube) to [Fugaku](https://en.wikipedia.org/wiki/Fugaku_(supercomputer)) {{rdv-thesis}}.  Multicomputer deployments will likely involve computational nodes, optical switches, Bell state analyzers, and possibly entangled photon pair sources (all defined below).  Quantum repeaters with memory are less likely to be deployed in multicomputers, though one such architecture {{choi-fat-tree}} has been proposed. Because the current technology roadmaps favor this type of deployment, where network design choices are in conflict or unclear, multicomputer designs are given priority over wide-area networks in this set of specifications.

A multicomputer may be a noisy, intermediate-scale quantum (NISQ) system without quantum error correction, or may be a fault-tolerant system.  Fault-tolerant systems are variously described as fault-tolerant quantum computers (FTQC), fault-tolerant application-scale quantum (FASQ) systems, or cryptographically relevant quantum computers (CRQC).  FTQCs require the network to generate many more entangled states with tight timing requirements to allow distributed quantum error correction or the creation of fully error-corrected entangled states for application use.

The execution model is expected to be much like the classical supercomputing [Message Passing Interface (MPI)](https://en.wikipedia.org/wiki/Message_Passing_Interface), in the sense that nodes cooperate in a tightly coupled fashion, exchanging data and controlling program execution, with each node executing a portion of a single, large computation.  One specific implementation of Quantum MPI has, in fact, been proposed {{haener-qmpi}}, but here we mean this in the broader sense.)

General hardware environment:

* A multicomputer consists of a set of quantum nodes that are connected via quantum optical channels. The system may be either a direct (point-to-point, end node-to-end node) or an indirect (switched) design.
* Every quantum node has a set of quantum devices and a classical controller.
* End nodes are generally computational nodes, but measurement-only, sensor, and specialized memory storage nodes may be included.
* End nodes are capable of running application programs as well as executing the minimum operations to build end-to-end entangled states.
* End nodes may be built using multi-level hardware interconnects; when gates between physically distant qubits are mediated by first creating shared entangled states, the creation of those entangled states is the responsibility of the network subsystem.
* Multicomputer interconnects are closed systems, with no need for cryptographic security mechanisms.

Many aspects of compilation and job execution are beyond the scope of this set of specifications, but some points will affect the network node definitions and interfaces, so it is important to present them here to establish a basis for design decisions:

* The general purpose of a multicomputer system is to execute application programs that exceed the capabilities of a single quantum node. The subdivision of the application into smaller quantum programs and the assignment of those sub-programs to nodes in the network is beyond the scope of this specification, and may be either automatically done by the compiler or manually done by the programmer.
* Programs are centrally compiled and distributed to nodes.  (Note that, technically, this is different from classical MPI, where a _command_ is sent to worker nodes, but the mapping of that command to an executable program and versioning and distribution of programs are outside the scope of MPI. It is, however, a convenient assumption and common practice to ensure the same program is executed at all worker nodes.)
* Execution is coordinated by a job controller: every node executes the same program, but with different parameters (e.g., which portion of the problem to work on).
* Applications consist of both classical computation and quantum computation; within a node, the classical portion of the program delegates certain computational tasks to the quantum processor (sometimes called a QPU), similar to a classical [coprocessor](https://en.wikipedia.org/wiki/Coprocessor) such as a [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit).
* Classical data related to quantum operations (principally measurement results and event notifications that trigger further actions) is sent peer-to-peer, not back to the centralized controller, during execution.
* Within the runtime system, the interface between the (portion of the) application running at each node's classical controller is analogous to the interface between an application and the MPI messaging system or a [socket](https://en.wikipedia.org/wiki/Network_socket) in an ordinary Internet application. This quantum socket is an active area of research and is not defined here.
* The creation of sequences of end-to-end entangled states, roughly equivalent to TCP, is the responsibility of RuleSets, inspired by [software-defined networking (SDN)](https://en.wikipedia.org/wiki/Software-defined_networking) {{farhadi-sdn}}. A RuleSet can also be viewed as something like a Berkeley Packet Filter (BPF) {{mccanne-bpf}} : it's a small program that handled actions that the application could do, but the application can't achieve the low, reliable latency to do it.
* In principle, all nodes are running the same program, distributed to all nodes. Since the compiled application circuits are often parameter- or input-dependent as well, separate nodes may have separate instances of the application. This may result in a small additional burden on the execution management system.
* In principle, the application and the communication system are separately compiled and managed. However, in practice the RuleSet may be compiled as part of the application by using a library of network functions.  (As with classical parallel program runtime systems, the boundary between the application program, supplied libraries, and the kernel itself (if any) is implementation-dependent.)
* Compiling the network communication into the application program eliminates the need for separate program and RuleSet distribution protocols. However, the event messages that are part of the architecturally defined RuleSet operation are sent and received as usual, such that the behavior of the node is the same regardless of such implementation choices.
* Compilation and execution may achieve application goals via teledata, telegate or measurement of multiqubit Pauli operators transparently; the network is unaware of this distinction. Management of application-level variables and their movement from node to node, if any, is the responsibility of the compiler and is beyond the scope of this specification.
* The resources in a multicomputer may be partitioned to run multiple jobs {{sane-jobs}}, but this is beyond the scope of the current specifications.

The realities of quantum hardware result in a few important differences from classical multicomputers:

* Multicomputer interconnects may be either optically switched or composed entirely of point-to-point links. In switched networks, depending on optical hardware as well as photonic qubit representation, reconfiguring the switch or switches may be an extremely high-latency operation.
* Application execution at end nodes proceeds in phases tied to specific communication patterns. Even with a fixed sequence of application-level operations, the execution time of a phase can be variable because entanglement generation is probabilistic. Local gates can also be probabilistic under some circumstances, but for many node hardware types, fast local gate execution means the impact of variable gate execution time will be small.
* In switched systems, reconfiguration of switches is centrally coordinated between phases. Thus, while classical data moves directly node-to-node during autonomous phase execution, advancing from phase to phase must be done at the direction of the job controller.
* Because execution is centrally coordinated, the network system is not required to provide multiplexing. (This is a substantial difference from data center networks, QLANs and QWANs.)
* The compiler may include multihop communication within a phase using hop-by-hop teleportation without reconfiguring any switches; this is beyond the scope of this architecture.
* Execution of the quantum portion of the node program generally involves hard real-time actions, both unconditional and conditioned on prior quantum measurement results. This generally requires compilation of the quantum program to very low-level actions to be executed by FPGAs or ASICs.
* Systems may be partially or completely emulated, decoupling development of different subsystems. e.g., an EPPS plus a MEAS together can emulate a COMP node that emits single photons.
* Systems may be noisy, intermediate-scale quantum (NISQ); near-term, small-scale fault tolerant; or fault-tolerant, application-scale quantum (FASQ).
* Quantum error correction is above the level of these specifications, but may involve distributed lattice surgery {{ramette-remote}}, {{leone-remote}}, or {{sinclair-ft-interconnect}}.

## Data Center Network (QDCN)

The hardware for quantum data center networks will be almost identical to multicomputers; the primary differences are in the workload, scheduling, programming model and assumptions of trust. Distributed control and protocols for multiplexing and connection setup may be necessary.

## Local-Area Network (QLAN)

A QLAN will be deployed within a building or across a campus. It may connect quantum computers (including but not necessarily multicomputers) and sensors. A sensor, for example, may be connected to a computer with substantial memory for e.g. shadow tomography, learning from few measurements and related protocols.

A QLAN will have a less regular topology than a multicomputer or QDCN. Distance, latency, fidelity, and success probability will all vary on a per-link basis.

Distributed control and protocols for multiplexing and connection setup are necessary {{aparicio-spie}}.

## Wide-Area Network (QWAN)

Wide-area networks may involve client-server or peer-to-peer communication. One particular scenario of interest is a measurement-only (MEAS) client end node connecting to a centralized, supercomputer-scale quantum computer (perhaps, but not necessarily, a multicomputer) for the purposes of executing _blind quantum computation_ {{fitzsimons-blind}}, {{morimae-blind}}.

QWAN client-server communication very likely will suffer from the "incast" problem of excessive traffic concentrating near certain nodes. Management of this problem is beyond the scope of this document.

# Quantum Optical Building Blocks

This section informally describes the physical building blocks and concepts used in the physical layer of a quantum network.  These definitions will use equations defined in {{I-D.draft-hajdusek-qirg-timing-physics}}.

## Qubits

In this network architecture, we use only qubits, which may have two states identified as 0 and 1.  Quantum information systems using qutrits, qudits, qunats or continuous variable (c.v.) quantum states are beyond the scope of the current set of specifications.

Qubits (also defined in RFC 9340) must conform to a sufficient subset of the DiVincenzo criteria {{divincenzo-criteria}}.

## Photons, Wave Packets and Optical Modes

Optical mode (link-layer view).

An optical mode is a well-defined slot of a physical link, specified by path, time window, frequency, polarization, or similar parameters, such that the receiver can be configured to monitor that slot and determine whether it is occupied by at least one photon or is empty.

The mode exists regardless of whether a photon is present; a photon is an excitation of the mode, not the mode itself.

In quantum networking, link capacity and state must be described in terms of modes (slots), not photons; photons merely occupy modes, while empty modes correspond to vacuum states that are still physically and operationally meaningful.

Technical note: In idealized models, distinct modes correspond to orthogonal field solutions, ensuring perfect distinguishability.

Short example:
A quantum optical link may define one mode per time window. During each window, the receiver monitors the mode. A detection event indicates that the mode was occupied by at least one photon; the absence of a detection indicates that the same mode was empty. Both outcomes correspond to distinct physical states of the link.

## Photonic Qubits

Photons are used in networks to carry qubits. There are several possible on-the-wire photonic qubit representations, e.g.

* Polarization
* Time bin
* Which path
* Energy level (wavelength)

These representations and more about the concept of an _optical mode_ are discussed in the Standard Photons document, and are provided here only for informational purposes.

## Memories

For our purposes, we do not need to worry about the physical implementation of memories, only that they may hold quantum data (qubits) that may be under the management of the network software and protocols. They may be entangled with photons or with other memory qubits.

Generally, the creation or entanglement of a state in memory is imperfect, and the memory has a finite lifetime.

The entanglement of a memory qubit with a photon is a technology-dependent process. To create fiber-compatible and optical equipment-compatible photons, wavelength conversion via transduction may be necessary. In 2025, transduction is a low-probability process, and hurts fidelity as well.

## Photon Sources

Photons may be emitted by _sources_ of many types {{nist-singles}} .  Single photons may come from attenuated lasers, or be emitted by a variety of quantum devices, such as quantum dots, or by individual atoms.

Photons may be unentangled, entangled with other photons, or entangled with quantum memories.

### Unentangled Single Photons

Unentangled photons exhibit quantum properties.  They can carry information in any of the characteristics listed above, and may be put into a superposition of multiple basis states for e.g. quantum key distribution purposes.  In this document, unentangled individual photons are not used.

### Entangled Photon Pairs

Pairs of photons entangled with each other can be made via a variety of physical processes. Devices that make such pairs can be components of nodes such as the Entangled Photon Pair Source (EPPS), described in a separate document.

### Memory-Emitted Photons

Photons emitted by quantum memories, such as single atoms, may remain entangled to the memory, if the memory was in a superposition of basis states.

## Detectors

Detectors may be either _single-photon detectors_, which click when _one or more_ photons hit the detector, or _number resolving detectors_, which can distinguish between one, two, or more photons hitting the detector within the same time window {{nist-singles}}. In this document, detectors may be assumed to be single-photon detectors.

# Requirements

This section documents the requirements for all networks adhering to this architecture.

## Normative Requirements

* The architecture must support an open development process {{RFC6852}}.
* The architecture must support the creation of robust, extensible, maintainable protocols in keeping with best current practice {{RFC9413}} {{RFC6250}} {{RFC1958}} {{RFC5218}}.

## General Requirements

### Functional Requirements

* Operates on qubits. (Qutrits, qudits, qunats and continuous-variable systems are out of scope of this architecture, except where physical or link layers present such physical variables as qubits.)
* Is independent of physical implementation of memories, photonic data representations, etc. (Multipartite states created by the network are not a requirement of the network.)
* Supports pairwise Bell pair creation between nodes with one or more of the B, C or T timing classes above.
* Support deployments ranging from multicomputer to wide area networks.
* Support multiple photonic synchronization domains, as either point-to-point or optically switched paths.  The architecture must support some form of buffering between PSDs.
* Support entanglement swapping.  (Note that single PSD deployments may not need entanglement swapping.)
* Support evolution of single-photon, unentangled, single-purpose quantum key distribution networks to fully entangled, multipurpose networks.

### Interface Requirements

* Supports one or more applications, such as the ones in {{RFC9583}}, with APIs consistent with the B, C, or T classes.
* The network must enable applications to match quantum states at each end of the Bell pair by name.

### Physical Requirements

Physical requirements such as distance, wavelength, vibration, power, etc. will be case-dependent.

### Environmental Requirements

Physical requirements such as distance, wavelength, vibration, power, etc. will be case-dependent.

## Network Management Requirements

### Fault Management

* Supports isolation of hardware and software faults.
* Supports monitoring and reporting of fidelity.

### Configuration Management

* The architecture must support the use of both manual and automated network configuration tools.

# Top Level Architecture

<!--
### Summary

* Service provided is two-party entanglement; multiparty entanglement is deferred to applications
* Four planes
    - Quantum
    - Data
    - Control
    - Management
* RuleSet-based connections
    - stateful E2E connections
    - inspired in part by SDN and computation-in-network research
* Connection setup
    - Decentralized two-pass (for wide-area, distributed, federated and internetworking)
    - Centralized controller (for QLANs and system interconnects)
* Comprised of numerous node types
    - qNode host requirements
    - Repeater nodes:
        + Rep1
        + Rep2 (undefined for now)
        + RTR
    - Support nodes:
        + OSW
        + MEAS
        + BSA
        + EPPS
        + RGSS (undefined for now)
        + ABSA (undefined for now)
    - End nodes:
        + COMP (NISQ or FASQ)
        + STOR
        + SNSR
* Links
    - Multiple on-the-wire photonic qubit representations, e.g.
        + Polarization
        + Time bin
        + Which path
        + Energy level (wavelength)
    - Multiple channel types, e.g.
        + fiber
        + free space point-to-point
        + satellite to ground point-to-point
    - Photonic Synchronization Domains (PSDs)
    - Multiple link architectures, e.g.
        + MIM
        + MSM
        + MM
        + RGS
    - Multidrop link types
        + switched photons
        + photonic synchronization domains
* Multiplexing and Routing
    - Stateful connections require some active resource management
    - involving point-to-point PSDs
    - involving multidrop PSDs
* Classical Communication
    - Several key roles:
        + reporting of parameters fixed by physics
        + reporting and setting of parameters selectable by node configuration
        + reporting and adjustment of slowly-changing parameters (such as polarization)
        + connection-level control of switching of photons
        + real-time event notification
    - See Timing Regimes document for outline of requirements
    - RPC for some tasks
        + especially device-mode control
        + qRPC wrapper for classical RPC mechanisms
    - message broker or event broker for other tasks
        + especially qubit-mode RuleSet notifications
* Naming and Addressing
* APIs for Network Service ("Quantum Sockets")
* Security
-->

## Deterministic Classical Control of Quantum States

This network architecture is entirely classically controlled.  Its task is to generate shared quantum states for applications residing at separate nodes. While many quantum events are inherently probabilistic, and loss of photons is also inherently probabilistic, this architecture does not use multipartite quantum states for e.g. routing of two-party requests.  (An extension of this network architecture may support generation of multi-partite state for applications at a later date.)

# Communication Service

(Substantial portions of this section are adapted from Naphan Benchasattabuse's Ph.D. thesis, which in turn is adapted from earlier papers by Van Meter et al. {{van-meter-qi-arch}} and others.)

The design of a quantum network must begin with a clear definition of its fundamental services --- what quantum states or capabilities the network is expected to provide to end users.
These decisions determine the complexity of the protocols at the network layer and the applications that run above it.
A minimalist design treats _Bell pairs_ as the primary network-level service.
Bell pairs serve as the smallest unit of entanglement and the foundation for nearly all quantum communication protocols.
Restricting the service to Bell pair distribution simplifies the network's responsibilities.
However, this approach shifts complexity to the applications, which must construct multipartite or fault-tolerant states themselves and manage the coordination overhead that entails.

At the other end of the spectrum, networks may offer richer services such as multipartite entangled states {{ghz}}, {{dur-w-state}}, {{hein-multiparty}}, {{hein-graph-entanglement}}
or fault-tolerant state teleportation.
While applications can, in theory, synthesize these states from Bell pairs, direct network-level support may offer efficiency gains and reduce sensitivity to noise by internalizing complex procedures like direct graph state generations or supporting the delivery of error-correcting code encoded logical qubits.

In our architecture, we adopt Bell pair distribution as the core network service, as it allows for a well-scoped, foundational architectural framework.
<!-- As we will see later, in \cref{sec:architecture-memory:discussion},
this architecture is also extensible to multipartite entanglement services.
These extensions build naturally on the base protocols discussed here and suggest a path for future network capabilities. -->

Importantly, the semantics of Bell pair distribution are not merely those of passive delivery.
Even in this basic model, distributed quantum computation occurs along the path via entanglement swapping, possibly combined with purification at intermediate repeater nodes.
A proper service definition must account for this processing, as it directly affects fidelity, latency, and trust assumptions in the network.

In addition to quantum state delivery, timing information is often a critical part of the service.
Applications in distributed quantum sensing and clock synchronization {{degen-sensing}}, {{proctor-quantum-sensing}}, {{proctor-multiparm}}, {{giovannetti-metro}}, {{gottesman-telescope}}, {{ilo-okeke-clock}}
require precise knowledge of when entanglement was established or when measurement events occurred.
Hence, high-precision timestamps may need to be bundled into the service interface offered by the network.

# Architectural Planes

All nodes in the network will have one or more of the following classes of interfaces, also referred to as _planes_.

* **Quantum:** The quantum signals and in-channel, hardware-dependent, real-time classical signals for timing and synchronization of photon wave packets.  A node with a quantum plane incorporates one or more quantum devices.  The quantum devices may be local or remote.
* **Data:** Classical data plane for exchange of messages about in-progress quantum communication sessions.  Generally, the data plane consists of _event notifications_ and _measurement results_ related to RuleSet-driven connections or testing sessions.  A data plane must be accompanied by a control plane.
* **Control:** Classical control plane for establishing and managing connections and testing sessions.  Routing and multiplexing messages are included in the control plane.
* **Management:** Network management for configuring the devices and monitoring operation.  Managing services provided by nodes, security, addressing, etc., and monitoring health of links, collecting statistics on traffic through the node, any alerts such as security, etc.

## Quantum

The quantum signals and in-channel, hardware-dependent, real-time classical signals for timing and synchronization of photon wave packets.  A node with a quantum plane incorporates one or more quantum devices.  The quantum devices may be local or remote.

The quantum plane functionality executes the functions described as "Interferometric Stabilization" and "Wave Packet Overlap" and subject to the constraints in "Detector Timing Windows" in the Timing Regimes document.

## Data

When operating in qubit mode, the Data Plane consists of classical messages that convey events for RuleSet operation and the communication ports and software that generate and consume such messages.

When operating in device mode, the Data Plane consists of RPCs for controlling individual devices.

Data plane functions may share data with management plane functions as part of the link management process, e.g. using disti-mation. If this is done, security and privacy concerns must be addressed.

The control plane functionality executes the functions described as "Pre-configured Event-driven Tasks" in the Timing Regimes document.

## Control

The classical control plane is responsible for establishing and managing connections and testing sessions.  Routing and multiplexing messages are included in the control plane.

Control plane functions may share data with management plane functions, e.g. sharing parameter adjustment values and timings. If this is done, security and privacy concerns must be addressed.

The control plane functionality executes the functions described as "Measurement basis selection", "Optical switch control" and some tasks in "Host-side Application-level Tasks" in the Timing Regimes document.

## Management

While connection-specific changes to configuration, such as switching and necessary, immediate changes to e.g. polarization and optical delay may appear as control plane functions, slow-rate monitoring and adjustment of parameters such as timing or polarization due to drift in temperature, voltage or other parameters is the responsibility of the management plane. The management plane may receive useful data on the health and fidelity of links as a result of data plane and control plane operations.

The management plane functionality executes the functions described as "Background Tasks" in the Timing Regimes document.

# Protocol Layers

This document describes a network architecture. Network designs are often described in terms of a layered protocol stack such as the 7-layer [OSI model](https://en.wikipedia.org/wiki/OSI_model), although the Internet can be more accurately described as a [three-, four-, or five-layer model](https://en.wikipedia.org/wiki/Internet_protocol_suite#Layering_evolution_and_representations_in_the_literature), depending in part on whether a distinction is made between the physical and link layers and in part on how the application layer is subdivided.

In a layered network architecture, each layer processes a prepended header to complete its task. As messages move down the stack (from application toward actual transmission), they may be subdivided into smaller units, and additional layer-specific headers are prepended. On receipt, headers are removed as the message moves up the stack, and boundaries between messages may be altered.

A complete network architecture consists of much more than the layers processing individual packets; many of the critical supporting protocols around naming, routing, security, network management, etc. utilize messages carried using the same protocol stack designed for application data.

In a quantum network, this layering is less clear.  Classical network protocol layering is often presumed to include the sequential addition of headers while preparing a packet for transmission and processing proceeds down the protocol stack, with the process inverted on packet reception.  In quantum networks, the qubits themselves are not processed in this stacked fashion, and the related classical information typically involves separate messages with separate end points as hop-by-hop entanglement is extended to end-to-end entanglement through the actions of nodes all along the path.

Nevertheless, the notion of _layers of responsibility_ or _separation of concerns_ is valid,with different needs at the link, network, and application.

(More to be added here.)

<!-- block couldn't figure out how to mermaid
  columns 3
  a["A label"] b:2 c:2 d -->

~~~~~~~~
+---------------------------+
| Application               |
+---------------------------+
| Network (RuleSet)         |
+---------------------------+
| Link                      |
+---------------------------+
| Physical                  |
+---------------------------+
~~~~~~~~
{: artwork-name="fig-layers" artwork-align="center" title="Protocol Layers" }

## Physical Layer

The physical layer incorporates the quantum channel itself, whether free space or waveguide.  Specifcation of the physical layer is out of scope for this document, but the physical-layer specifications must include:

* signal transmission characteristics of the channel
* how nodes physically connect to the channel
* choice of photonic qubit
* wavelength
* wave packet envelope shape and duration
* timing/trial rate
* how link synchronization is achieved
* certain characteristics of detection subsystem

Additional details on how to specify a physical layer will be presented in documents on the "standard photon" and "photon train", to come.

## Link Layer

The primary service provided by the link layer is heralded, named entanglement across a quantum channel with defined endpoints {{I-D.draft-dahlberg-ll-quantum}}, {{dahlberg-ll-arxiv}}, {{delle-donne-thesis}}, {{delle-donne-os-nature}}.  The link layer sits below the network layer and uses physical-layer quantum phenomena plus classical messaging to provide its service.  In this architecture, the link service provides only bipartite entanglement.  The link layer architecture will support B, C and T class applications, though not all links are required to support all classes.  In support of these classes, the entangled states may be either still active and available for further use by the network layer, or one or both of the qubits may already have been measured, with the measurement basis and results recorded and reported.

See p. 36 of {{delle-donne-thesis}} for a decent description of the link service.  They refer to K-type (keep), M-type (measure) and R-type (remote) entanglement requests.  (What about reverse-R type?)

The link layer may deliver entangled states to the network layer either singly or as an ordered, tagged batch.

The link may operate entirely on demand, or as an always-on, free-running service where requests from the network layer are serviced by using recently created entanglement.

Can the network layer request states at one end where the status of the qubit at the other end is unknown, in either heralding or Pauli frame?  This seems to be necessary to support B class.

For multidrop links, the link layer must coordinate with multiplexing and switch control as part of the control plane {{I-D.draft-zhu-qirg-qdcp}}.

The link may consist of several network nodes.  Besides the two endpoints, switches, BSAs, and EPPSes may be involved.  Although these support nodes are part of the network architecture, their presence is not visible beyond the boundaries of the link or PSD.

In this architecture, fidelity is the responsibility of the network layer; the link layer always provides raw Bell pairs of base fidelity.  Thus, fidelity is part of neither the request to nor response from the link layer.  During connection setup, information about link fidelity is acquired from the link management and used by the Responder to plan the connection.

Thus, link monitoring and link fidelity management are the responsibility of the link architecture but are not part of the link layer protocol.

* "message" format
* addressing
* multiplexing for multi-drop links

### Link/Network Layer Interface

(should this get moved to the Link section below?)

The link/network interface is best described as a software interface, executed separately at each link endpoint.

The network-->link request:

* addresses of nodes
* single/fixed number/stream
* disposition: keep or measure, basis

The link-->network response:

* addresses of nodes
* length of array of entangled states
* array of entangled states
    - identifier for entangled state
    - (timestamp separate from identifier? needed or not?)
    - flags
        - confirmed/pending confirmation
        - measured/live
    - if measured, basis
    - if measured, result

## Network Layer: RuleSets

(responsible for both single- and multi-hop purification, and entanglement swapping)

The network layer subsumes the functions commonly divided into network and transport in many architectures.  It serves as a lightweight, restricted (not Turing complete) distributed computation platform.

## Application Layer

(mostly not defined here)

# Nodes and Node Types

(Substantial portions of this section are adapted from Naphan Benchasattabuse's Ph.D. thesis, which in turn is adapted from earlier papers by Van Meter et al. and others.)

The architecture of a quantum network is defined by its constituent nodes and their specialized functions.
In our architecture, we classify nodes into three main groups: end nodes, for application interaction; repeater and router nodes, for extending entanglement and path management; and support nodes, for auxiliary operational tasks.

The qNode specification (a document to be published) will provide additional details on the common roles and responsibilities of all quantum network nodes, and serves as the equivalent of the Internet hosts requirements RFCs {{RFC1122}}, {{RFC1123}}. Each node type is further defined in a detailed specification in a separate document.

## End Nodes

End nodes represent hosts that wish to execute a quantum application such as quantum key distribution, secret sharing and blind quantum computation {{broadbent-bfk-protocol}}, {{fitzsimons-blind}}.
The technological maturity required of an end node heavily depends on the desired application.
There are four major kinds of end nodes:

**A measurement (MEAS) node** is the most basic type of quantum end node, designed primarily for protocols that do not require quantum state storage.
Its core capability is to receive individual photons and perform measurements on them in at least two different bases.
Lacking quantum memory, MEAS nodes are well-suited for applications like quantum key distribution (QKD) or as simple terminals in certain forms of secure delegated computation protocols {{morimae-blind}},{{fitzsimons-blind}}, typically interacting with the network in a synchronous manner where measurement results directly yield classical data.

**A sensor (SNSR) node** is a specialized end node designed to utilize entangled states, often shared with distant parties, for high-precision measurements of physical quantities, for clock synchronization tasks, or for distributed sensing tasks {{ge-linear}}, {{proctor-quantum-sensing}}, {{degen-sensing}}, {{giovannetti-metro}}, {{proctor-multiparm}}.
These nodes typically feature limited quantum memory to hold working qubits (e.g., one half of an entangled pair) and possess specific quantum processing capabilities tailored for sensing protocols.
Such capabilities include performing joint measurements, like Bell State Measurements (BSMs), between their stored qubits and photons that have interacted with the environment {{huang-imaging-stars}}, {{gottesman-telescope}}.
While an SNSR node's internal processing is specialized, certain sensing applications may also necessitate high-rate entanglement generation from the network to achieve desired performance.
For SNSR nodes, precise timing information is almost invariably a critical component of the service they provide or require, and their operation typically culminates in outputting classical data that corresponds to the sensed phenomenon.

**A store (STOR) node** is a specialized end node whose primary function is to serve as a high-fidelity quantum data repository.
Its core capabilities are the long-term storage of quantum states---often prepared and teleported from other locations---and the ability to teleport these states out on demand.
While a STOR node does not require a universal gate set, it must support certain gates (e.g., Clifford gates) for active quantum error correction to preserve the stored quantum data.
This includes using quantum error-correcting codes to protect against decoherence, along with mitigation strategies for correlated errors from events such as cosmic ray strikes {{martinis-correlated}}, {{sane-phonons}}, {{xu-dist-qec}}, {{vepsaelaeinen-ionizing}}, {{wu-mitigating}}, {{li-cosmic}}.
In a network context, STOR nodes may function as data servers, enabling asynchronous applications where valuable states are prepared and stored for later retrieval.

**A computational (COMP) node** represents a full-fledged quantum processing endpoint within the network.
Equipped with quantum memory and additional algorithmic qubits, it can store, manipulate, and perform complex computations on quantum states received from the network or generated locally.
COMP nodes support a wide range of advanced quantum network applications, including distributed quantum algorithms, more general forms of blind quantum computation, and potentially fault-tolerant quantum computing, often requiring asynchronous interfaces to coordinate their local quantum workloads with network operations {{ambainis-multiparty-coin}}, {{taherkhani-byz}}, {{mayers-unconditional}}, {{christandl-anon}}, {{broadbent-bfk-protocol}}, {{fitzsimons-blind}}, {{mahadev-homomorphic}}, {{dulek-homomorphic}}, {{shapourian-qdc-infra}}, {{sutcliffe-dist-qec}}, {{yoder-tour-de-gross}}, {{kim-ft-million}}.

## Support Nodes

**An entangled photon pair source (EPPS)** is a device dedicated to generating pairs of entangled photons, commonly through processes like Spontaneous Parametric Down-Conversion (SPDC).
These entangled photons are then typically distributed over quantum channels to be captured or measured at link endpoints, forming the initial resource for entanglement-based protocols.
EPPS nodes can be deployed in various scenarios, including terrestrial fiber links or free-space satellite-to-ground communication {{fittipaldi-sat}}, {{haldar-sat-dist}}, {{khatri-spooky}}, {{yin-1200km}}.

**A Bell state analyzer (BSA)** is a crucial component for performing projective measurements on two incoming photons, ideally projecting their combined state into one of the four Bell states.
BSAs are fundamental for realizing photonic entanglement swapping{{zukowski-entanglement-swapping}},
a primary process that creates link-level entanglement, used particularly to convert memory-photon entanglement into memory-memory entanglement between distant quantum memories.
The efficiency and complexity of a BSA depend on the optical implementation and the specific photonic qubit encoding used.

**A Repeater Graph State Source (RGSS)** is a specialized source that generates multipartite entangled photonic states, specifically tailored for all-photonic (memory-less) quantum repeater architectures {{azuma-rgs}}, {{hilaire-rgs-optimizing-gen-time}},{{buterakos-graph-generation}}, {{hilaire-logical-bsm}}.
An RGSS typically distributes segments of the generated repeater graph state to adjacent network nodes, where subsequent measurements on these photonic qubits are performed to establish long-distance entanglement without relying on quantum memories.

**An advanced Bell state analyzer (ABSA)** represents a more sophisticated version of a BSA, particularly required in advanced all-photonic repeater protocols based on repeater graph states{{azuma-rgs}}, {{hilaire-rgs-optimizing-gen-time}},{{buterakos-graph-generation}}, {{hilaire-logical-bsm}}.
Unlike basic BSAs, an ABSA must be capable of performing measurements on single or multiple photons in dynamically selectable bases.
The choice of measurement basis often depends on the outcomes of prior measurements within the network and the specific structure of the repeater graph state being utilized, implying more complex hardware and real-time classical control logic.

**An optical switch (OSW)** is a device that can passively route photons from input optical fibers or paths to different output paths without performing measurements on them {{koyama-24}}.
OSWs, which can be based on technologies like nanomechanical systems or nanophotonic circuits, can be integrated as components within other node types (e.g., routers or complex end nodes) or can function as standalone elements in the network to dynamically reconfigure optical pathways.

An OSW node contains at least one switch device, which comprises at least once switch point.

## Repeater Nodes

**A first-generation repeater (REP1)** is a network node with two quantum interfaces, whose main task is to extend entanglement.
Its primary operations include generating link-level Bell pairs with its neighbors, performing entanglement swapping to connect these segments, and managing errors through heralded entanglement purification on physical qubits along the connection path.

**A second-generation repeater (REP2)** also focuses on entanglement swapping to bridge distances but generally requires a larger quantum memory capacity and higher fidelity local quantum operations than a REP1.
It utilizes quantum error correction (QEC) to manage operational errors in conjunction with heralded link-level entanglement generation.
Instead of, or in addition to, purifying link-level physical Bell pairs, a REP2 node operates on logical qubits, where quantum information is encoded across multiple physical qubits to protect it from errors.
This approach inherently demands more sophisticated hardware and advanced computational capabilities for encoding, decoding, and error correction routines during swapping.

**A quantum router (RTR)** is a more complex and versatile node, possessing all capabilities of a quantum repeater and typically featuring three or more quantum network interfaces, enabling it to make sophisticated path selection decisions in complex topologies.
Architecturally, an RTR may consist of multiple line cards and a quantum backplane, allowing it to run a full suite of network operation protocols.
Beyond basic repeating functions like entanglement swapping, an RTR can govern network borders potentially interfacing between different repeater generations or technologies, participate in generating multipartite entangled states if the network provides such a service {{meignant-dgs}} {{bugalho-dist-multipartite}} {{fischer-dgs}} {{fan-dgs-dist}},
and may act as a Responder in connection setups by rewriting or generating new RuleSets for different network domains.

## Composite Nodes

A node may also aggregate the functions of more than one node, in a form known as a _composite node_ or _composite logical node_. A common form of composite node is a switching BSA. When multiple devices of the same type are controlled by a single controller, they may be presented either as a node with multiple devices or as a composite node where each device is in turn represented as a node. Presenting as a single node is preferred.

# Links

## The Link Service

A link provides Bell pairs across a single PSD.  Each Bell pair is named via an identifier. This service may be either real time or batched.  Generally, the physical link entanglement generation mechanism is probabilistic but heralded.  Although it is possible to use repeated trials to present a near-deterministic service {{humphreys-deterministic-link}}, in this architecture we choose instead to expose the asynchronous creation of Bell pairs with timestamps.

(Does software control of buffer qubits appear in the architecture, or is it purely an implementation detail?)

## Photonic Path Description

The optical path over which photons flow from source to detector in the process of creating a Bell pair can be described using terminology that names the node types in the path; the direction of flow of photons can be inferred. This path description can be applied to point-to-point or switched links within a single PSD.

Device type single-letter abbreviations and their corresponding node type:

* M: memory (COMP or STOR)
* S: source (of entangled photons) (EPPS)
* I: interference (i.e., Bell state measurement) (BSA)
* D: detector (i.e. a measurement node) (MEAS)
* X: switch (OSW)

Examples of path descriptions that may commonly appear:

* DSD: detector-source-detector
* MIM: memory-interference-memory
* MSM: memory-source-memory
* MM: memory-memory
* DSISD: detector-source-inteference-source-detector

At any point in a path except the ends, a photon may pass through one or more switches.

In a switched architecture, for example, photons may pass through paths such as:

* DXSXD
* MXIXM
* MXXIXM

(Question: Does this notation also need to represent frequency conversion?)

## Point-to-point

Point-to-point links may be either fiber-based or free space. A link encompassing the path of one or more photons may be partially fiber and partially free space.

The photonic path description notation will include no 'X's.

## Switched

A system built around a pool of detectors, particularly organized as BSAs, utilizing switched MIM links can also be characterized as a _detector-centric architecture_.

For pseudocode for switching (routing) certain types of devices, see Koyama et al. {{koyama-24}}.

The photonic path description notation will include one or more 'X's.

## Multidrop or Bus

A multidrop link, or a bus, is a shared physical channel to which more than two stations may be attached.

### Link Management

Configuration.

Management of fidelity, trial rate, detection parameters, etc.

Monitors slowly changing fidelity.

Supplies information about link fidelity and rate to other subsystems such as routing and connection setup.

# Connections

No task involving quantum communication ever involves a single qubit or single entangled state. The connection provides the framework for managing the creation of an order set of entangled states to be consumed by applications. A connection is _stateful_ at the end nodes. Nodes involved in the creation of end-to-end entanglement for those end nodes will be _connection aware_, meaning that they can identify resources and messages and carry out communication tasks necessary for a specific connection, but may not have substantial amounts of state that is dynamically updated on a per-action basis; any actions for nodes in this class must be idempotent or known to occur only once. Some or all nodes may be _fully stateful_, tracking the disposition of specific, named quantum states.

Connections may be created using either a fully-distributed protocol {{I-D.draft-van-meter-qirg-quantum-connection-setup}} or a centralized mechanism.  In either case, qNodes involved in the connection receive RuleSets that are created by a single controller to coordinate local operations to build the end-to-end entangled states requested by an application.

Connections are unaware of the shared use of resources and of other connections. Multiplexing is the responsibility of a separate subsystem, though connection setup should be done with awareness of the availability of unavailability of resources at involved nodes.

# Resource Management: Multiplexing and Routing

Both link usage time slots and memory can be shared among multiple connections and therefore must be actively managed via a multiplexing system.  This task is particularly challenging in switched networks.

The discovery of the physical topology can be based on link state protocols, such as direct adaptation of OSPF or IS-IS {{I-D.draft-kaws-qirg-advent}}.  These protocols use a unitless link cost.  It is known that, at least for certain physical systems, selecting a link cost corresponding to "seconds per Bell pair of a given fidelity" produces good correlation between low path cost and high throughput {{van-meter-sys-design}}, {{van-meter-path-sel}}.  A number of approaches have been proposed {{abane-routing}}.

# Classical Communication

A quantum network depends on classical communication; indeed, almost all of the behavior is governed by, initiated by, or managed and reported via classical messages and signals. These messages and signals have several key roles, described in the following subsections. See the Timing Regimes document {{I-D.draft-hajdusek-qirg-timing-physics}} for an outline of the physics driving these requirements.

## Quantum Plane

Yes, the quantum plane includes some classical signals.

## Control Plane

* Qubit mode connections and communication
    - connection-level control of switching of photons
    - real-time event notification for RuleSets
* Device mode control

## Data Plane

* Qubit mode connections and communication
    - connection-level control of switching of photons
    - real-time event notification for RuleSets
* Device mode control

## Management plane: Node and link management

* reporting of parameters fixed by device physics
* reporting and setting of parameters selectable by node configuration
* reporting and adjustment of slowly-changing parameters (such as polarization drift)
* typical network node management tasks such as software updates

## Mechanisms

* RPC for some tasks
    - especially device-mode control
    - qRPC wrapper for classical RPC mechanisms
* message broker or event broker for other tasks
    - especially qubit-mode RuleSet notifications

# Naming and Addressing

## State naming and management in RuleSets

(Incorporates naming material from Naphan's thesis. Probably needs updating to account for testbed realities.)

Managing and agreeing upon the specific qubits for joint operations like entanglement purification or swapping among collaborating nodes are critical responsibilities handled by RuleSets.
While it is possible to draw inspiration from the IP architecture by employing network-wide unique naming for qubits, RuleSets have local execution contexts, making global naming for individual qubits unnecessary.

Instead, RuleSets use local logical names for qubits.
At the lowest level, physical qubits within a QNIC can be addressed by the local node using a tuple like `<QNICAddress,QubitIndex>`.
However, this level of detail is not, and should not be, visible to the RuleSet logic.

Within a RuleSet instance on a given node, the RuleSet mechanism identifies a quantum resource primarily by its **tag** --- a label that categorizes the resource into a specific pool corresponding to its current role or stage in the protocol.
<!--  (as discussed in \cref{subsec:architecture-memory:ruleset-definition}). -->
To ensure an unambiguous and absolute ordering of multiple resources that may share the same tag (e.g., several Bell pairs awaiting purification), each resource, upon being allocated to a tag, is automatically assigned a \emph{sequence number} by the local RuleSet engine.
The combination `<tag,seq no.>` thus serves as a distinct and locally unique key within that RuleSet instance for referencing a resource and associating it with relevant metadata, such as its tracked fidelity.
Actions specified within Rules typically reference these resources based on their tag and their relative order within that tag, for instance, by operating on the resource with the smallest sequence number (i.e., the oldest available in that pool).
This structured internal naming is vital for deterministic local operations and for preventing local operational mismatches that could lead to problems like the leapfrogging issue if not handled carefully at a higher protocol design level.

The RuleSet execution mechanism itself, therefore, only requires and manages this local `<tag,seq no.>` system for resource identification within a single node's RuleSet instance; it does not impose any inherent restrictions or requirements on how shared entangled states are identified between nodes.
It is recommended that a strategy be used wherein the RuleSet creator (e.g., the Responder during connection setup) devises RuleSets such that the `<tag,seq no.>` is kept consistent across the RuleSets of all nodes involved in a particular joint operation on that resource.
The responsibility thus lies with the RuleSet author to ensure that RuleSets are designed---potentially using this consistent naming strategy---to correctly manage shared resources and achieve the desired end-to-end protocol behavior.
This minimal local naming scheme provided by the RuleSet engine, combined with judicious design of the RuleSets themselves, is sufficient for implementing a wide range of complex quantum network protocols while allowing creativity with minimal restrictions on RuleSet creator parts.
<!--, as will be illustrated with examples in \cref{sec:architecture-memory:ruleset-definition-examples}. -->

# Example Networks

While a full taxonomy of networks is neither desirable nor possible here, we present a few network examples using point-to-point links or switched architectures.  In this section, the topology is briefly described, followed by analysis of the path characteristics of the shortest path and network diameter.

## Fully Connected Point-to-Point

Small networks may use nodes with multiple interfaces and provide a direct link between each pair of nodes, making a _direct_ network.  Assuming sufficient node-internal capabilities, such a network provides lowest loss (giving the fastest individual links) and the highest aggregate bandwidth, and is inherently nonblocking.  However, with n-1 links per node and O(n^2) links in the network, its scalability is poor.  It will always provide the highest performance, but not necessarily highest price/performance ratio.

If links are midpoint interference-based, an issue in design is packaging of the BSAs and detectors.

PSD: Each link is a separate PSD.

All paths: MIM

## Single Optical Switch

A number of the early quantum multicomputer proposals assumed a single, large optical switch.  Such a network is _indirect_.

PSD: Although the entire network is a single PSD, each pairing is adjusted independently.

All paths: MXIXM

## Q-Fly Multicomputer

An _indirect_ interconnect. A multi-group, BSA-centric architecture.  All nodes are part of the same PSD.  The Q-Fly architecture is described in Sakuma et al. {{sakuma-q-fly}}.

PSD: Although the entire network is a single PSD, each pairing is adjusted independently.

For DPFD topologies:

* Shortest paths
    - intra-group: MIXM
    - inter-group (network diameter): MXXIM
* Longer paths:
    - non-shortest path: MXXIXM or longer

For DPHD topologies:

* Shortest paths
    - intra-group: MXIXM
    - inter-group (network diameter): MXXIXM
* Longer paths:
    - non-shortest path: MXXXIXM or longer

For SPHD topologies:

* Shortest paths
    - intra-group: MXIXM
    - inter-group (network diameter): MXXIXM
* Longer paths:
    - non-shortest path: MXXXIXM or longer

## Optically Switched Fat Tree

An _indirect_ interconnect. Several parameters are needed to describe the full topology of a fat tree, which can also be called a _k_-ary _n_-tree:

* _k_ is the switch radix
* _n_ is the tree depth

This simplest description assumes homogeneous hardware, where all switches have the same number of ports and all links are the same bandwidth.  Leiserson's original fat tree proposed single links of increasing bandwidth at higher levels of the tree, giving the network its name; this approach provides no redundancy or path diversity, and achieving higher transfer rates is impractical in some technologies, including quantum.  Consequently, most fat tree deployments use multiple links to several switches at higher levels of the tree, in a configuration that is also know as a _folded Clos_ network.

PSD: Although the entire network is a single PSD, each pairing is adjusted independently.

## Repeater Fat Tree

The repeater fat tree is described in {{choi-fat-tree}}.

PSD: Each link is a separate PSD.

## 2-D Grid Multicomputer

A _direct_ interconnect. A 2-D grid of nodes, where nodes with memory and certain computational capabilities (canonically COMP nodes) have up to four interfaces connecting to neighboring nodes. Each node must act as a memory buffer and repeater to enable communication between non-neighboring nodes.

PSD: Each link is a separate PSD.

## Ring

A _direct_ interconnect. All nodes in a ring have exactly two neighbors. Each node must act as a memory buffer and repeater to enable communication between non-neighboring nodes.

A ring is described in (something from Simon's group).

PSD: Each link is a separate PSD.

## QLAN

A quantum local area network will have:

* irregular topology, possibly of heterogeneous link types
* distributed multiplexing
* distributed routing

PSD: If the QLAN does not include optical switches, but uses repeaters, each link is a separate PSD. If the QLAN includes optical switches, the PSDs may have irregular boundaries.

# APIs for Network Service ("Quantum Sockets")

The API used by classical software to interface with the quantum depends on which class of timing dependency pattern (B, C, or T) is to be supported.

# Security Considerations

Quantum multicomputer systems are assumed to be constructed as isolated, centrally controlled systems with no need for confidentiality, integrity, and availability (the "CIA triad") assurance via cryptographic methods.

Security considerations for other network types are an open topic of study and as such are not yet ready for specification and standardization {{satoh-attacking}}.

--- back
