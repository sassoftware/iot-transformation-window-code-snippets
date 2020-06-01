# transpose_long Instructions

This example transposes information in long mode. You will process information about the pitch, yaw, roll, and velocity of an aircraft in flight.

Use the following steps to execute the transpose_long code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input_long.csv` file to the server directory you just created.

3.  Upload the `Transpose_long.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/Uploading_a_Model_to_ESP_Studio.pdf) document for instructions.
  
4.  Double-click the project named `Transpose_long` to open it.

5.  Edit the Input Data Connector for the `SourceW` window to include the full path to the `input_long.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

6.  Edit the Subscriber Connector for the `TransposeL` window to include the full path to the `output.csv` file that will be created. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

7.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/Testing_Models.pdf) document for instrcutions.

8.  Execute the model on the ESP Server and Subscribe to the `TransposeL` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/Executing_a_Model_and_Viewing_the_Output.pdf) document for instructions.

9.  Download and open the `output.csv` file created by the model.
