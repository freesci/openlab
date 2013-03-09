---
layout: post
title: "Bioinformatics workflow management systems"
description: "lists and notes"
category: bioinformatics
tags: [workflows,frequentlyupdated]
---
{% include JB/setup %}

Originally, Wikipedia hosted [quite a decent list of bioinformatics workflow management systems](http://en.wikipedia.org/w/index.php?title=Bioinformatics_workflow_management_systems&oldid=521689910), however due to [its policies](http://en.wikipedia.org/wiki/Wikipedia:NOTDIRECTORY) the list was removed and only definition is left. Therefore, I'm going to maintain my own list with some comments on usability, cons and pros, etc. 

The text below is reformatted and slightly shortened version of aforementioned Wikipedia page:

### At first, two major workflow engines:

* [Galaxy]( http://usegalaxy.org/) is a pipeline system developed at Pennsylvania State University and Emory University.  Galaxy is available as a [free public web server](http://usegalaxy.org/) and as [downloadable software](http://getgalaxy.org/). Galaxy stresses ease of use and sharing and persisting analyses.
* Taverna workbench] is an open source workflow system that enables scientists (typically, though not exclusively, in bioinformatics) to compose and execute scientific workflows. It has been developed as part of a L5.5m EPSRC project called myGrid based at the University of Manchester. Independently, other researchers have created Programming by example workflow development tools that are interoperable with Taverna.

### Other workflow engines I have tried (sometimes only to install) or I see them used relatively frequently:

* UGENE|UGENE Workflow Designer is an open source visual environment designed for building and executing bioinformatics workflows. The main purpose of the system is providing user-friendly GUI for creating computational workflows that can be executed as well as on commodity hardware as on high-performance clusters and supercomputers.

* Kepler scientific workflow system|Kepler enables scientists in a variety of disciplines like biology, ecology and astronomy to compose and execute workflows. Kepler is based on the Ptolemy II system for heterogeneous, concurrent modeling and design. Ptolemy II was developed by the members of the Ptolemy project at University of California Berkeley. Although not originally intended for scientific workflows, it provides a mature platform for building and executing workflows, and supports multiple models of computation.

* BioExtract harnesses the power of online informatics tools for creating and customizing workflows. Users can query online sequence data, analyze it using an array of informatics tools, create and share custom workflows for repeated analysis, and save the resulting data and workflows in standardized reports.

* Ergat is a web-based system used to create, run, and monitor reusable bioinformatics analysis pipelines. It contains pre-built components for common bioinformatics analysis tasks, such as blast searches or storing data in a Generic Model Organism Database|Chado database. These components can be arranged graphically to create highly-configurable pipelines.


### Workflow engines I need to test:

* Anduril (workflow engine)|Anduril is an open source component-based workflow framework for scientific data analysis developed at the University of Helsinki. Anduril provides an execution engine written in Java, a large number of components for bioinformatics analysis, and the AndurilScript language to create and manage workflows.

* BioBike is a biocomputing platform based upon the KnowOS (Knowledge Operating System) e-science technology. Written entirely in Lisp (programming language)|Lisp, KnowOS's main distinguishing feature is "through-the-browser" programmability.
 
* BioManager is a bioinformatic data management and analysis workflow developed by the University of Sydney.

* [eHive](http://www.ensembl.org/info/docs/eHive/index.html)  is a fault tolerant distributed processing system initially designed to support comparative genomic analysis, based on blackboard systems, network distributed autonomous agents, dataflow graphs and block-branch diagrams.

* GenePattern is a genomic analysis platform developed at the Broad Institute|Broad Institute of MIT & Harvard that provides access to more than 220 tools for gene expression analysis, proteomics, SNP analysis, RNA-seq, flow cytometry, and common data processing tasks. A web-based interface provides access to these tools and allows the creation of multi-step analysis pipelines that enable reproducible in silico research.

Other workflow engines, often with functionality outside of my core interests:
	
* CellProfiler is an open source modular image analysis software developed at the Broad Institute. Capable of handling hundreds of thousands of images, it contains advanced algorithms for image analysis of cell-based assays and is optimized for high-throughput work. The software allows the user to construct a pipeline of individual modules; each module performs an image processing step, such as image loading, object identification, and feature extraction.
 
* DAGMan is the scientific workflow engine of the Condor High-Throughput Computing System. It has been introduced in the late 1990s and is still under active development. DAGMan is employed by higher level workflow systems like the Pegasus Workflow Management System.
 	
* Discovery Net.(circa 2000) is one of the earliest examples of scientific workflow systems. It was the winner of the Most Innovative Data Intensive Application Award at the ACM SC02 (Supercomputing 2002) conference and exhibition, based on a demonstration of a fully interactive distributed genome annotation pipeline for  a Malaria genome case study. It originated from a L2m EPSRC-funded project with the same name investigating the development of an e-Science platform for scientific discovery from high throughput data sources at Imperial College London. Many of the features of the Discovery Net(architecture features, visual front-end, simplified access to remote Web and Grid Services and inclusion of a workflow store) were considered novel at the time, and have since found their way into other academic and commercial systems. The workflow system developed in the project itself was later used as the basis for the commercial products of the Imperial College spin out company [http://www.inforsense.com](InforSense).
 	
* [http://www.geneprof.org](GeneProf) is a web-based, graphical software suite developed at the University of Edinburgh that allows users to build pipelines and analyse data produced using high-throughput sequencing platforms (RNA-seq and ChIP-seq)
 	
* Geodise (Grid Enabled Optimisation and Design Search for Engineering) was developed at the University of Southampton.
 	
* HCDC is an open source workflow system developed at ETH Zurich that is focus on large scale image based biological experiments. Include large collection of components for multiwell plate handling (96, 384, ...).
 	
* [http://www.inforsense.com](InforSense) is a commercial workflow system based on the Discovery Net system providing rapid development of analytical applications, integration of data and services from heterogeneous sources, producing repeatable, auditable analytical processes. It provides domain specific extensions for Bioinformatics, Cheminformatics, Health Informatics and Business Analytics. It also provides features such as Embedded Applications, Portals, Dashboards and Business Rules Engines.
 	
* LONI Pipeline is a Java-based distributed graphical data-analysis environment for constructing, validating, executing and disseminating scientific workflows. As the LONI Pipeline references all data, services and tools as external objects, it directly allows resource interoperability without the need for rebuilding the software.
 	
* Medicel Integrator Workflow is a cluster-enabled bioinformatics workflow design and execution application. It can be used stand-alone or integrated with a biology data warehouse.
 	
* [https://projets.pasteur.fr/projects/mobyle/wiki](Mobyle) is a framework and web portal specifically aimed at the integration of bioinformatics software and databanks. Mobyle is the successor of Pise and the RPBS server, previous systems that provided web environments to define and execute bioinformatics analyses.
 	
* Pegasus Workflow Management System|Pegasus is a flexible framework that enables the mapping of complex scientific workflows onto the Grid computing|grid developed at the Information Sciences Institute at the University of Southern California.
 	
* Pegasys is a software for executing and integrating analyses of biological sequences, developed by the University of British Columbia.
 	
* Pipeline Pilot is Accelrys scientific informatics platform that streamlines the data integration and analysis by using a Visual Programming Language (similar to LabVIEW) to build a pipeline to transform any number of inputs (raw data) into any number of outputs.
 	
* Remora is a web server implemented according to the BioMoby web-service specifications, providing life science researchers with an easy-to-use workflow generator and launcher, a repository of predefined workflows and a survey system.
 	
* RetroGuide is a query framework for querying retrospective bioinformatics data.
 	
* Sight (workflow platform)|Sight is a web agent oriented workflow platform that historically has extensive means to integrate websites with ordinary web forms and HTML responses (there is also support for WSDL as well). The system has a GUI-based workflow composer that supports modules with multiple ports and allows to access data from the modules that stand earlier in workflow. Sight was developed in University of Ulm|Ulm university using java and it currently released under GPL.
 	
* Triana is an open source problem solving environment developed at Cardiff University that combines an intuitive visual interface with powerful data analysis tools.
	
* Wildfire is a distributed, Grid-enabled workflow construction and execution environment. It has a graphical user interface for constructing and running workflows. Wildfire borrows user interface features from Jemboss and adds a drag-and-drop interface allowing the user to compose EMBOSS (and other) programs into workflows. For execution, Wildfire uses GEL, the underlying workflow execution engine, which can exploit available parallelism on multiple CPU machines including Beowulf-class clusters and Grids.
 
