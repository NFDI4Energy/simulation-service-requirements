# Introduction

The use cases for Task Area 5 were defined to clarify the goals and define the requirements for the development in the different Measures.

# Use Cases

## UC01 - Search for simulation software
|||
|---|---|
| **Scope/Objective**               | Be able to search for simulation software in the registry (based on keywords) |
| **Stakeholder**                   | researcher, domain experts, software developer, student, industry |
| **Assumptions and Prerequisites** | \- Registry exists and is populated (filled) <br />\- Interface to search in the registry <br />\- Interface to refine search by selecting different criteria <br />\- Existing User Interface (GUI) |
| **Sequence/Workflow**             | 1\. Person is looking for simulation software to simulate [transient behaviour of a phaseshift transformer] <br />2\. Searching in software registry with the keywords: transient, phaseshift transformer <br />3\. gets a list with matching software and sugesstions to refine the search, like open source and proprietary software <br />4\. Get a list of compatible software that could be coupled / used with the current software and links to their description pages <br />5\. Selecting open source <br />6\. Getting refined list with matching software <br />7\. Selecting software from list to get simulation software overview page with detailed description and available data sets <br />8\. The description page also provides information regarding publications using the software and available results <br />9\. following link to get to software homepage to start downloading  |
| **Priority**                     | High |
| **Related Measures**             | M5.1 |

## UC02 - Compare simulation software and models
|||
|---|---|
| **Scope/Objective**               | Be able to search for simulation software in the registry and be able to compare simulation software in the registry based on attributes (based on keywords) |
| **Stakeholder**                   | researcher, domain experts, software developer, student, industry |
| **Assumptions and Prerequisites** | \- Registry exists and is populated (filled) <br />\- Interface to search in the registry <br />\- Interface to refine search by selecting different criteria <br />\- Existing User Interface (GUI) |
| **Sequence/Workflow**             | 1\. Person is looking for simulation software to simulate transient behaviour of a phaseshift transformer Searching in software registry with the keywords: transient, phaseshift transformer <br />2\. gets a list with matching software <br />3\. Selecting multiple softwares from list to get simulation software overview of attributes to compare softwares <br />4\. User decides which software fits the needs and chooses it |
| **Priority**                     | High |
| **Related Measures**             | M5.1 |

## UC03 - Find best-suited co-simulation framework
|||
|---|---|
| **Scope/Objective**               | The user has to be supported in finding the best simulation framework for integrating a PV plant simulation model including simulator into a surrounding distribution power grid.  |
| **Stakeholder**                   | researcher, student, domain expert |
| **Assumptions and Prerequisites** | \- The simulation frameworks and models have to be described in a standardized way and made available in a registry. <br />\- The registry also contains example scenarios that use the same PV controller as the requested one. <br />\- The user already knows which model will be used (**REF TO UCXYZ**). |
| **Sequence/Workflow**             | 1\. The user is looking for a co-simulation framework. <br />2\. The user looks in the NFDI4Energy platform and can input requirements (Which co-simulation framework is best-suited for my simulation model and supports a suitable power grid simulator?). <br />3\. The possible co-simulation frameworks are shown in a comparable way (table)  <br />4\. The user chooses one of the frameworks that is best-suited for the use case. |
| **Priority**                     | High |
| **Related Measures**             | M5.1 |

## UC04 - Find simulation model and data for co-simulation
|||
|---|---|
| **Scope/Objective**               | The user has to be supported in finding a simulation model for a PV plant to use it in a co-simulation, furthermore the user needs to find data for the model |
| **Stakeholder**                   | researcher, student, simulation framework developer, domain expert, industry  |
| **Assumptions and Prerequisites** | \- The simulation models have to be described in a standardized way and made available in a registry <br />\- It has to be specified if a simulation model can be coupled with a specific co-simulation framework <br />\- The available data has to be described in a standardized way and made available in a registry <br />\- It has to be specified which data can be used by which simulation software/model <br />\- Input and output of the simulation model is known |
| **Sequence/Workflow**             | 1\. The user is looking for PV model (not software specific) with certain requirement to be able to integrate it into a co-simulation <br />2\. The user looks into NFDI4Energy platform, gives the requirements and gets a filtered list of all available models <br />3\. By choosing a specific model, information regarding data and parameters needed to get the model running (Exemplary data) |
| **Priority**                     | High |
| **Related Measures**             | M5.2, M5.1 |

## UC05 - Find and reuse existing co-simulation scenarios
|||
|---|---|
| **Scope/Objective**               | Improve the Findability and reusability of co-simulation scenarios and create FAIR co-simulation scenarios |
| **Stakeholder**                   | student, researcher, industry |
| **Assumptions and Prerequisites** | \- Collection with simulation scenarios <br />\- Methods to search the collection <br />\- Meta data to describe simulation scenarios / Common format for scenarios <br />\- Documentation or tutorial how to reuse the scenario <br />\- Provide a list or an overview of existing simulation scenarios and make them downloadable |
| **Sequence/Workflow**             | 1\. User wants to simulate a model for charging cars in a flexible way. <br />2\. User goes onto the NFDI4Energy Platform to look for similar scenarios <br />3\. User enters the search-terms "flexibility" and "electric cars".  <br />4\. User gets a list with example scenarios that match this terms and articles that describe necessary steps for a similar simulation. <br />5\. Read description of simulation scenarios / read simulation scenario itself (preview of file) <br />6\. Compare simulation scenarios (split view) <br />7\. User selects one of the examples and goes over the list of prerequisites and installs required software. <br />8\. User runs the chosen scenario locally and adapts it to their needs. |
| **Priority**                     | Medium |
| **Related Measures**             | M5.2, M5.1 |

## UC06 - Creation of simulation scenarios
|||
|---|---|
| **Scope/Objective**               | Guide a user through the process of creating a co-simulation based on already chosen components. Include tools to automate part of the process. |
| **Stakeholder**                   | researchers, industry, student |
| **Assumptions and Prerequisites** | \- simulation framework and simulation components are already chosen (UC05 and UC07) <br />\- metadata of simulation components is available (UC07)  |
| **Sequence/Workflow**             | 1\. The user wants to create  a scenario based on already chosen framework and model. <br />2\. The user uses the NFDI4Energy platform and provides the chosen framework, components and metadata. <br />3\. User gets support on how to connect the chosen simulation components to create the scenario (e.g., assisted by a wizard or getting recommendations). This can also contain connection rules to make connections between groups of entities easier. <br />4\. The user gets configuration files and instructions for the execution (as a text-file).  |
| **Priority**                     | High |
| **Related Measures**             | M5.2 |

## UC07 - Guided creation of simulation scenario based on research goal
|||
|---|---|
| **Scope/Objective**               | Guide a user through the process of creating a co-simulation based on the general research goal. Include tools to automate part of the process. |
| **Stakeholder**                   | researcher, industry, student |
| **Assumptions and Prerequisites** | \- simulation framework and simulation components are not yet strictly chosen. <br/>\- a domain ontology exists |
| **Sequence/Workflow**             | 1\. The user describes the research goal (i.e., the output the simulation should provide) on the NFDI4Energy platform based on a domain ontology. <br/>2\. The user provides additional information about the planned simulation (e.g., time resolution) <br/>3\. The user gets recommendations for suitable co-simulation frameworks. (See also UC05) <br />4\. The user chooses suitable co-simulation framework. <br/>5\. The user gets recommendations for suitable simulation models. (See also UC07)  <br />6\. The user chooses suitable simulation models. <br />7\. User gets support on how to connect the chosen simulation components to create the scenario (e.g., assisted by a wizard or getting recommendations). This can also contain connection rules to make connections between groups of entities easier. (See also UC08) <br />8\. The user gets configuration files and instructions for the execution (as a text-file).  |
| **Priority**                     | High |
| **Related Measures**             | M5.2 |

## UC08 - Automated execution of a simulation scenario
|||
|---|---|
|**Scope/Objective**|Provide the possibility to execute a simulation scenario on the SIMaaS service|
|**Stakeholder**| researchers, industry, students |
|**Assumptions and prerquisites**|The input configuration for the simulation scenario does exist in a format and schema as is specified by the co-simulation scenario ontology|
|**Sequence/Workflow**|1. The user wants to execute a scenario that he or she has available locally<br />2. The SIMaaS is initialized with the upload of the scenario configuration<br />3. The user can review and modify the scenario configuration in the UI<br />4. Simulation is started and live execution dashboard is opened to visualize the progress (and data)<br />5. Simulation finishes and the dashboard updates to include the simulation results<br />6. The user downloads the bundle of the scenario configuration and the output data|
|**Priority**|high|
| **Related Measures**             | M5.3, M5.4 |

## UC09 - Investigating and reproducing the results of a co-simulation
|||
|---|---|
|**Scope/Objective**|A user wants to investigate and reproduce the results of existing research|
|**Stakeholder**| researcher, student, industry |
|**Assumptions and prerquisites**|\- The user has found an existing simulation scenario with results on the co-simulation scenario registry service or has uploaded his own scenario config and results bundle there|
|**Sequence/Workflow**|1. The user opens the result visualization view on the NFDI4Energy co-simulation scenario registry for the respective co-simulation scenario<br />2. The UI displays all available data so the user is able to investigate it<br />3. The user starts another co-simulation run and also published the results<br />4. The user selects both result sets and opens the result compparison view to investigate if the results are reproducible|
|**Priority**|low|
| **Related Measures**             | M5.4 |

## UC10 - Add software to the NFDI4Energy research software registry
|||
|---|---|
|**Scope/Objective**|Add software to the energy research software registry|
|**Stakeholder**| software developer, researcher, student, industry |
|**Assumptions and prerquisites**|- Registry exists<br />- Software to be added has a public link<br />- Metadata schema for software records is available<br />- Software developers want to improve visbility of their software, want feedback from the community or want to increase their sales.<br />- Research insitutes either want feedback on their software or increase visibility and credibility in terms of collaboration or project proposal.|
|**Sequence/Workflow**|1. The user checks if the software is already registered in the NFDI4Energy research software registry<br />2. If not, he creates a metadata record with the assistance of the service, which also includes the purpose of the software and how it can be used<br />3. The user publishes the record on the registry|
|**Priority**|medium|
| **Related Measures**             | M5.1 |


## UC11 - Add simulation model to the NFDI4Energy research software registry
|||
|---|---|
|**Scope/Objective**|Add a model to the energy research software registry|
|**Stakeholder**| software developer, researcher, student, industry |
|**Assumptions and prerquisites**| \- The simulation model already exists<br />\- The simulation software that the model uses exists on the registry<br />\- Ability to reference other existing models with similar scope to make comparison easier<br />\- Motivation for adding a simulation model is similar to UC 5.1.1 |
|**Sequence/Workflow**|same as 5.1.1 but use other metadata schema for models instead|
|**Priority**|medium|
| **Related Measures**             | M5.1 |

## UC12 - Sharing the results of a co-simulation FAIRly
|||
|---|---|
|**Scope/Objective**|The user needs to be supported in recording his scenario and the result of his co-simulation. Furthermore, he needs to be able to share this|
|**Stakeholder**| researcher, student, industry |
|**Assumptions and prerquisites**| \- The scenario and its results can be recorded in a standardized way based on our ontology.<br />\- The metadata schema developed in M4.3 has to be used fro annotation of result data.<br />\- The user works on a specfic research question.|
|**Sequence/Workflow**|1. The user describes his co-simulation in the standardized (ontology based) scenario config file<br />2. The results are annotated with metadata according to the predefined schema<br />3. The user uploads all relevant data sets with the assistance of the SIMaaS service and the co-simulation scenario registry service.|
|**Priority**|medium|
| **Related Measures**             | M5.4, M4.3 |

# Stakeholder

The following potential stakeholder were identified.

- researcher (including phd student)
- student (e.g., in a modeling courses)
- simulation model developer
- interested non-experts
- data analyst
- domain expert
- simulation framework expert/maintainer/developer
- simulation maintainer/organizer
