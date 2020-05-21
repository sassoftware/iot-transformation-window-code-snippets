# removeState Instructions

This example demonstrates how to facilitate the transition of a stateful part of a model to a stateless part of a model.

Use the following steps to execute the removeState code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `InputRemove.csv` file to the server directory you just created.

3.  Upload the `RemoveState.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](docs/Uploading_a_Model_to_ESP_Studio.pdf) document for instructions.

4.  Double-click the project named `RemoveState` to open it.

5.  Edit the Input Data Connector for the `SourceWindow` window to include the full path to the `InputRemove.csv` file you uploaded. Refer to the [Editing Connectors](docs/Connectors.pdf) document for instructions.

6.  Save your changes and test your model. Refer to the [Testing Models](docs/Testing_Models.pdf) document for instrcutions.

7.  Execute the model on the ESP Server and Subscribe to the `Copy` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](docs/Executing_a_Model_and_Viewing_the_Output.pdf) document for instructions.

