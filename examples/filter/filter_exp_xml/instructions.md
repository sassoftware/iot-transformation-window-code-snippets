# filter_exp_xml Instructions

This example contains a single source window and filter window with a filter expression.

Use the following steps to execute the filter_exp_xml code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input.csv` file to the server directory you just created.

3.  Upload the `modelfilterexp.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/uploading.md) document for instructions.
  
4.  Double-click the project named `projectfilterexp` to open it.

5.  Edit the Input Data Connector for the `sourceWindow` window to include the full path to the `input.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/connectors.md) document for instructions.

6.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/testing.md) document for instrcutions.

7.  Execute the model on the ESP Server and Subscribe to the `filterWindow` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/executing.md) document for instructions.
