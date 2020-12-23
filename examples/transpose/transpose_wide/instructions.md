# transpose_wide Instructions

This example transposes information in wide mode. You will process information about the pitch, yaw, roll, and velocity of an aircraft in flight.

Use the following steps to execute the transpose_wide code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input_wide.csv` file to the server directory you just created.

3.  Upload the `Transpose_wide.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/uploading.md) document for instructions.
  
4.  Double-click the project named `Transpose_wide` to open it.

5.  Edit the Input Data Connector for the `SourceW` window to include the full path to the `input_wide.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/connectors.md) document for instructions.

6.  Edit the Subscriber Connector for the `TransposeW` window to include the full path to the `output.csv` file that will be created. Refer to the [Editing Connectors](../../../docs/connectors.md) document for instructions.

7.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/testing.md) document for instrcutions.

8.  Execute the model on the ESP Server and Subscribe to the `TransposeW` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/executing.md) document for instructions.

9.  Download and open the `output.csv` file created by the model.