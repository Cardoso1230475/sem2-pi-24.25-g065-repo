# Supplementary Specification (FURPS+)

## Functionality

_Specifies functionalities that:  
&nbsp; &nbsp; (i) are common across several US/UC;  
&nbsp; &nbsp; (ii) are not related to US/UC, namely: Audit, Reporting and Security._

* The system must allow users to create, save, and load maps and scenarios.

* It must support cargo generation, transformation, and transport through a network of stations.

* Reporting tools must allow visualization of statistical data (e.g., cargo transported, station performance).

* Audit logs must record train purchases, station constructions, and route assignments.

* Security measures must ensure only authenticated editors can create or modify scenarios.

## Usability 

_Evaluates the user interface. It has several subcategories,
among them: error prevention; interface aesthetics and design; help and
documentation; consistency and standards._

**Help and documentation:**

* The application and all the documents support the English language.

## Reliability

_Refers to the integrity, compliance and interoperability of the software. The requirements to be considered are: frequency and severity of failure, possibility of recovery, possibility of prediction, accuracy, average time between failures._

* Cargo production and consumption must be accurate and consistent based on station reach and industry logic.

* Simulation operations must be deterministic under the same input conditions.

## Performance

_Evaluates the performance requirements of the software, namely: response time, start-up time, recovery time, memory consumption, CPU usage, load capacity and application availability._

**Response Time**

* All activities must have a quick response from the system.

## Supportability

_The supportability requirements gathers several characteristics, such as:
testability, adaptability, maintainability, compatibility,
configurability, installability, scalability and more._

**Adaptability**

The team must adopt:

* Best practices for identifying requirements and for OO software analysis and design,
* Recognized coding conventions and standards (e.g., Camel Case).


## +

### Design Constraints

_Specifies or constraints the system design process. Examples may include: programming languages, software process, mandatory standards/patterns, use of development tools, class library, etc._

**Programming Languages:**

* The application must be developed in Java language using the IntelliJ IDE or Netbeans.
* The application graphical interface is to developed in JavaFX 11.
* The unit tests should be implemented using the JUnit framework.

**Mandatory standards/patterns:**

* All the images/figures produced during the software development process should be recorded in SVG format.
* The application should use object serialization to ensure data persistence between two runs of the application.

**Development Tools:**

* The team must use Javadocs to generate useful documentation for Java Code.
* The unit should be implemented using the JUnit 5 framework.
* The JaCoCo plugin should be used to generate the coverage report.

### Implementation Constraints

_Specifies or constraints the code or construction of a system such
such as: mandatory standards/patterns, implementation languages,
database integrity, resource limits, operating system._

**Resource limits**

* The program ought to use little memory and CPU.

### Interface Constraints

_Specifies or constraints the features inherent to the interaction of the
system being developed with other external systems._

* The system must support exporting statistics in CSV or JSON formats.

* No direct interaction with external APIs or real-time online services is required.

### Physical Constraints

_Specifies a limitation or physical requirement regarding the hardware used to house the system, as for example: material, shape, size or weight._

* The application must be responsive on screens with a resolution of at least 1366x768 pixels.

* Must support full-screen and windowed mode.