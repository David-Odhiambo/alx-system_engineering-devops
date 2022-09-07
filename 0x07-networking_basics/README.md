The Open Systems Interconnection model (OSI model) is a conceptual model that 'provide[s] a common basis for the coordination of [ISO] standard development from the purpose of system interconnection'.[2] In the OSI reference model, the communications between a computing system are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application.[3]

The model partitions the flow of data in a communication system into seven abstraction layers, to describe networked communication from the physical implementation of transmitting bits across a communications medium to the highest-level representation of data of a distributed application. Each intermediate layer serves a class of functionality to the layer above it and is served by the layer below it. Classes of functionality are realized in all software development through all and any standardized communication protocols.

Each layer in the OSI model has its own well-defined functions, and the functions of each layer communicate and interact with the layers immediately above and below it, unless the layer does not have layers below or above. In either case, each layer of the OSI model has its own well-defined functions that describe the basic applications for communication of all communication protocols.

The Internet protocol suite has a separate model, the layers of which are mentioned in RFC 1122 and RFC 1123. That model combines the physical and data link layers of the OSI model into a single link layer, and has a single application layer for all protocols above the transport layer, as opposed to the separate application, presentation and session layers of the OSI model.

In comparison, several networking models have sought to create an intellectual framework for clarifying networking concepts and activities,[citation needed] but none have been as successful as the OSI reference model in becoming the standard model for discussing, teaching, and learning for the networking procedures in the field of Information technology. Additionally, the model allows transparent communication through equivalent exchange of protocol data units (PDUs) between two parties, through what is known as peer-to-peer networking (also known as peer-to-peer communication). As a result, the OSI reference model has not only become an important piece among professionals and non-professionals alike, but also in all networking between one or many parties, due in large part to its commonly accepted user-friendly framework.[4]


Communication in the OSI-Model (example with layers 3 to 5)

Contents
1	History
2	Definitions
2.1	Standards documents
3	Layer architecture
3.1	Layer 1: Physical layer
3.2	Layer 2: Data link layer
3.3	Layer 3: Network layer
3.4	Layer 4: Transport layer
3.5	Layer 5: Session layer
3.6	Layer 6: Presentation layer
3.7	Layer 7: Application layer
4	Cross-layer functions
5	Programming interfaces
6	Comparison to other networking suites
6.1	Comparison with TCP/IP model
7	See also
8	Further reading
9	References
10	External links
History
The development of the OSI model started in the late 1970s to support the emergence of the diverse computer networking methods that were competing for application in the large national networking efforts in the world (see Protocol Wars). In the 1980s, the model became a working product of the Open Systems Interconnection group at the International Organization for Standardization (ISO). While attempting to provide a comprehensive description of networking, the model failed to garner reliance during the design of the Internet, which is reflected in the less prescriptive Internet Protocol Suite, principally sponsored under the auspices of the Internet Engineering Task Force (IETF).

In the early- and mid-1970s, networking was largely either government-sponsored (NPL network in the UK, ARPANET in the US, CYCLADES in France) or vendor-developed with proprietary standards, such as IBM's Systems Network Architecture and Digital Equipment Corporation's DECnet. Public data networks were only just beginning to emerge, and these began to use the X.25 standard in the late 1970s.[5][6]

The Experimental Packet Switched System in the UK circa 1973–1975 identified the need for defining higher level protocols.[5] The UK National Computing Centre publication 'Why Distributed Computing' which came from considerable research into future configurations for computer systems,[7] resulted in the UK presenting the case for an international standards committee to cover this area at the ISO meeting in Sydney in March 1977.[8]

Beginning in 1977, the ISO initiated a program to develop general standards and methods of networking. A similar process evolved at the International Telegraph and Telephone Consultative Committee (CCITT, from French: Comité Consultatif International Téléphonique et Télégraphique). Both bodies developed documents that defined similar networking models. The OSI model was first defined in raw form in Washington, DC, in February 1978 by Hubert Zimmermann of France and the refined but still draft standard was published by the ISO in 1980.[9]

The drafters of the reference model had to contend with many competing priorities and interests. The rate of technological change made it necessary to define standards that new systems could converge to rather than standardizing procedures after the fact; the reverse of the traditional approach to developing standards.[10] Although not a standard itself, it was a framework in which future standards could be defined.[11]

In 1983, the CCITT and ISO documents were merged to form The Basic Reference Model for Open Systems Interconnection, usually referred to as the Open Systems Interconnection Reference Model, OSI Reference Model, or simply OSI model. It was published in 1984 by both the ISO, as standard ISO 7498, and the renamed CCITT (now called the Telecommunications Standardization Sector of the International Telecommunication Union or ITU-T) as standard X.200.

OSI had two major components, an abstract model of networking, called the Basic Reference Model or seven-layer model, and a set of specific protocols. The OSI reference model was a major advance in the standardisation of network concepts. It promoted the idea of a consistent model of protocol layers, defining interoperability between network devices and software.

The concept of a seven-layer model was provided by the work of Charles Bachman at Honeywell Information Systems.[12] Various aspects of OSI design evolved from experiences with the NPL network, ARPANET, CYCLADES, EIN, and the International Networking Working Group (IFIP WG6.1). In this model, a networking system was divided into layers. Within each layer, one or more entities implement its functionality. Each entity interacted directly only with the layer immediately beneath it and provided facilities for use by the layer above it.

The OSI standards documents are available from the ITU-T as the X.200-series of recommendations.[13] Some of the protocol specifications were also available as part of the ITU-T X series. The equivalent ISO/IEC standards for the OSI model were available from ISO. Not all are free of charge.[14]

OSI was an industry effort, attempting to get industry participants to agree on common network standards to provide multi-vendor interoperability.[15] It was common for large networks to support multiple network protocol suites, with many devices unable to interoperate with other devices because of a lack of common protocols. For a period in the late 1980s and early 1990s, engineers, organizations and nations became polarized over the issue of which standard, the OSI model or the Internet protocol suite, would result in the best and most robust computer networks.[8][16][17] However, while OSI developed its networking standards in the late 1980s,[18][19] TCP/IP came into widespread use on multi-vendor networks for internetworking.

The OSI model is still used as a reference for teaching and documentation;[20] however, the OSI protocols originally conceived for the model did not gain popularity. Some engineers argue the OSI reference model is still relevant to cloud computing.[21] Others say the original OSI model doesn't fit today's networking protocols and have suggested instead a simplified approach.
