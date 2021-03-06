Introduction
==============

Status of VAMDC-XSAMS
---------------------

The VAMDC consortium include many databases providers from very 
different fields of atomic, molecular and solid spectroscopy 
commmunity. Started with the 
International Atomic Energy Agency's XML Schema for Atomic, Molecular and Solid 
Data (XSAMS) version 0.1.1 [XSAMS]_ , VAMDC consortium has found that 
modifications/additions were necessary in order to meet the needs
of implementation and queries. 
This effort has been carried out within the WP6 workpackage
including contributions/requirements from all VAMDC partners.
This effort has resulted in the so-called VAMDC-XSAMS schema
that is used within VAMDC. Releases of VAMDC-XSAMS are planned
every 3 months and it is planned that VAMDC-XSAMS and XSAMS will
converge every year. The current version of VAMDC-XSAMS is version 0.3 
and it is part of the 11.11 Release of VAMDC Standards. The VAMDC release
documents for the VAMDC-XSAMS schema include: a tarball including the VAMDC-XSAMS 
schema files (main file is xsams.xsd) and some example files [VAMDC-XSAMS-SCHEMA]_, 
the current reference guide and its PDF file [VAMDC-XSAMS-PDF]_, the documentation created 
directly from the schema [VAMDC-XSAMS-DOC]_, the changelog document [VAMDC-XSAMS-LOG]_ 
that provides the log between the IAEA XSAMS version 0.1.1  [XSAMS]_ and the
VAMDC-XSAMS version 0.2 [VAMDC-XSAMS-SCHEMA]_, the documentation for the
case-by-case description of molecular states [case-by-case]_.


Motivation of XSAMS (and VAMDC-XSAMS)
-------------------------------------

Many fields in astronomy, physics, energy production and industry depend on
databases for atomic, molecular and particle-surface interaction processes
(AMPSI). A reliable exchange of such data has been recognized as important for
decades, and the Atomic and Molecular (A+M) Data Unit of the International
Atomic Energy Agency established a Data Centre Network (DCN) in 1976 to
address this vital issue in connection with fusion energy research
[Lorenz]_. Thus, the ALADDIN data exchange system was adopted in 1988 by
the DCN for use by the fusion community in a variety of applications
[Janev]_.  

While developments in data exchange within the fusion community were deemed to
be adequate two decades ago, a rapid expansion of the Internet resulted in an
equally impressive expansion of electronic databases. Most DCN members
maintain separate databases, each with a distinct interface and data formats.
Independently, the ADAS project was initiated in support of the JET programme
[ADAS]_, and the resulting system has developed into a large project with
a dedicated internal method of data exchange. Until recently, difficulties
were experienced in obtaining the underlying AMPSI data from ADAS without
being a member of the group. Furthermore, the astrophysics community has its
own set of dedicated databases and interfaces. Under these circumstances,
there is clearly an urgent need for a new data exchange standard based on the
latest technology. The International Virtual Observatory Alliance (IVOA)
undertook some initial work from 2002 onwards to define and adopt an XML
schema for data exchange [Hanisch]_. There have been other formats for
AMPSI data exchange involving selected data producers and databases, but they
did not include global efforts to define a data exchange process.   

During the course of the 2004 ICAMDATA meeting in Japan, group discussions
focused on the need to develop a more comprehensive schema for AMPSI data for
general use. This group consisted of Yu. Ralchenko of the National Institute
of Standards and Technology (USA), D. Schultz of the Oak Ridge National
Laboratory (USA), M.L. Dubernet of Universit\'e Pierre et Marie Curie (France)
and E. Roueff of the Observatoire Paris-Meudon (France), and 
D. Humbert and R.E.H. Clark of the International Atomic Energy
Agency (Austria), and they have met twice every year to develop such a schema.
Recently, P. Loboda and S. Gagarin have joined the group from the All-Russian
Institute of Technical Physics, Russia. Summary reports of the meetings are
available as IAEA reports and can be downloaded from the A+M Unit web site
[XSAMS]_. The resulting XML Schema for Atoms, Molecules and Solids (XSAMS)
can be found on the same A+M Unit website [XSAMS]_. 

The primary objective of the XSAMS exchange standard is to set up a framework
for the correct exchange of AMPSI data, rather than to exchange correct data.
Important issues such as data verification and data quality are not addressed
by XSAMS, which has been established solely as the data exchange procedure.
Although XSAMS does require inclusion of documentation of the source and
generation of the data, issues related to the correctness or applicability of
the data are left for consideration by data producers. 

The overall structure of XSAMS reflects the standard approach to description
of A+M physics in terms of physical processes connecting different states. 
Specific rules are used to describe the physical states of
atoms, molecules, ions, elementary particles and solids as unambiguously as
possible. States can be specified in any of a number of levels of detail and
in different coupling schemes. Processes between states can be described using
a reference to initial and final state, as well as a process type. The
numerical data for processes can be tabulated, or parameters for a fitting
procedure with provision for specifying the exact nature of the fitting
function.  Different types of differential cross sections as well as total
cross sections can be accommodated.  Finally, since the origin and history of
the data are necessary for data assessment, XSAMS imposes strict requirements
on the traceability of the data, with the mandatory inclusion of information
on data sources and the methods used to generate specific sets of data. 

XSAMS was developed through the joint efforts of researchers from the
International Atomic Energy Agency (Austria), National Institute of Standards
and Technology (USA), Oak Ridge National Laboratory (USA), Universit\'e
Pierre et Marie Curie and Observatoire
Paris-Meudon (France), with contributions from the All-Russian Institute of
Technical Physics (Russia). 

The schema for describing states of physical systems and
processes connecting different states are detailed in the following sections.
All required and optional entries are clearly described, and examples given.


Limitations of VAMDC-XSAMS
--------------------------

As of |today| , some parts of the schema are well developed (e.g., on atomic and
molecular structure or processes) while the others are only in the initial
phase of development (e.g., solids, environments). It was nevertheless decided to add those
less-advanced sections in order to provide some insight into future
development of the schema.


Document goal 
-----------------

The goal of this document is not to create a reference schema documentation,
but to define guidelines and examples on filling in data in schema.
For reference documentation, see autogenerated HTML docs [VAMDC-XSAMS-DOC]_.

