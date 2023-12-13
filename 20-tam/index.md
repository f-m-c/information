---
title: TAM Overview
---

# Technical Architecture Modeling (TAM)

## SAP has used FMC early

SAP offers mission-critical business software, such as Enterprise Resource Planning (ERP), Supply Chain Management(SCM), Human Capital Management (HCM), and many others. There are thousands of people working on one product, requiring a well-organized division of labor. Supportability is one of the key features of SAP software, driving many architecture decisions.

SAP started using FMC in 1990 to capture the knowledge of the application server technology of the R/3 system (which was released in 1993). The results were a set of so-called "bluebooks", technical reports that introduce one specific product part or technology on a technical level.

## With TAM, SAP combines FMC and UML

Since 1999, SAP looked for ways to combine FMC with the upcoming UML notation to increase the acceptance. The findings were condensed in an SAP-internal standard for modeling architecture: TAM (Technical Architecture Modeling) has been released and rolled out to the organization in the last years. Now TAM is the standard way to model and describe technical architecture at SAP.

So what is TAM and how does it differ from FMC and UML? In short, TAM is a pragmatic combination of FMC and UML based on modeling best practices at SAP, defining a reasonable subset of diagram types and elements. One important finding is to distinguish two levels for architecture modeling: The conceptual level and the design level. At SAP, UML typically covers design level, while the conceptual level is more the FMC domain. But the decision was made not to have two different kinds of notation for the two levels - although it would be easier to distinguish the levels, the number of diagram types had to be small.

On conceptual level, TAM is FMC with (partly) UML notation. For behavior, it uses activity diagrams instead of petri nets (and sequence diagrams for examples). For E/R structures, UML class diagrams are used. For compositional structure, block diagrams are used in the known FMC notation, since the UML does not offer an aequivalent diagram type.

## TAM in practice

Although TAM and FMC have been used before by a number of architects and developers at SAP, the TAM roll-out activities and the inclusion in the SAP-internal development policy has lead to a broad usage of TAM at SAP. Some architects called TAM "THE language to communicate about architecture".

But TAM is not only useful for architects and developers. An increasing number of consultants is using TAM (mainly FMC block diagrams) to analyze and discuss the customer's system landscape and how to insert the SAP solution into the landscape. These consultants are happy with TAM because it allows them to be precise enough without having to dive too deeply into the implementation details.

## How to use TAM

To get more information about TAM, please read the TAM definition document. Here, the subset of diagram types and elements is defined, including rules when to use which (on conceptual or design level).

TAM shows that it is not necessary to decide between FMC and UML - they can be combined to complement each other very well. The choice to use UML notation for FMC (on conceptual level) surely has some drawbacks regarding expressiveness; on the other hand, complex behavior descriptions are rather rare, and E/R structures in UML mainly lack nesting, which is tolerable in practice. To improve readability, the same layout rules as for FMC diagrams also apply to TAM diagrams. Finally, FMC (and therefore TAM) is not primarily about notation (although it is important for communication) — it is about how to think about systems to be able to share this knowledge with others.