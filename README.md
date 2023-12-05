# Complaints and Claims Management - EMSA

This project is designed to manage the complaints and claims process of Electrificadora del Meta (EMSA). It utilizes the BPMN (Business Process Model and Notation) to model the workflow and is implemented using Spring Boot for deployment on an embedded machine.

![BPMN Model](Docs/img/EMSA-2.0.0.png)

## BPMN Model Features

### Model Elements

1. **Call Activity**: Used to execute an independent process modeled as a separate activity.

    ![Call Activity](Docs/img/CallActivity.png)

2. **Subprocess**: Represents a set of activities grouped in a logical and reusable unit.

    ![Sub Process](Docs/img/SubProcess.png)

3. **Business Rule Task**: Task that executes a business rule.

    ![Sub Process](Docs/img/DMN.png)

4. **Auto Generate Form**: Automatic generation of forms based on the model.

    ![Sub Process](Docs/img/AutoGenerateForm.png)

5. **BPMN Form**: Form associated with a task or activity in the process.

    ![Sub Process](Docs/img/BPMNForm.png)

6. **Arithmetic Calculations**: Used to perform mathematical operations in the workflow.

    ![Sub Process](Docs/img/Arithmetic.png)

7. **Exclusive Gateways**: Logical decisions directing process flow based on conditions.

    ![Sub Process](Docs/img/Gateways.png)

8. **External Task using a "Java Class" implementation**: External task executed through a Java class, enabling integration with external systems.

    ![Sub Process](Docs/img/ExternalTask.png)

### Technologies Used

1. **Spring Boot**: Framework for Java application development.

2. **BPMN**: Standard notation for modeling business processes.

3. **Java**: Primary programming language used in the implementation.

4. **Embedded Camunda**: Deployed on an embedded machine for resource optimization and easy implementation.

## Installation and Execution Guide

### Prerequisites

1. Java JDK 17 or higher.
2. Maven.
3. IntelliJ IDEA Ultimate.
4. Camunda Modeler.

### Steps to Run the Project

1. Clone this [repository](https://github.com/jhonalexander019/The-SpringBoot-Project.git) to your local machine.
2. Open the documents in the **Models, Forms, and DMNs** folders in Camunda Modeler.

4. Open the **Camunda** folder using IntelliJ IDEA Ultimate.

5. Run the embedded Camunda machine in Spring Boot.
![Sub Process](Docs/img/deployment.png)

6. Deploy the model from Camunda Modeler pointing to the embedded Camunda in Spring Boot.

### Usage Example

Once the application is running, access the [URL](http://localhost:8080/) to interact with the complaints and claims flow. Follow the on-screen instructions to test the process.

![Sub Process](Docs/img/CamundaEmbedded.png)

![Sub Process](Docs/img/ExecuteInstance.png)

![Sub Process](Docs/img/FirstForm.png)

![Sub Process](Docs/img/Form.png)

