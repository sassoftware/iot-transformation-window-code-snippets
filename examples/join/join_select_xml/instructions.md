# join_select_xml Instructions

This example contains two source windows joined by a left outer join in a join window.  The join window uses field-selections to select the non-key fields.

Use the following steps to execute the join_select_xml code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `trades.csv` and `traders.csv` files to the server directory you just created.

3.  Upload the `model.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/uploading.md) document for instructions.
  
4.  Double-click the project named `join_select_xml` to open it.

5.  Edit the Input Data Connector for the `sourceWindow_01` window to include the full path to the `trades.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/connectors.md) document for instructions.

6.  Edit the Input Data Connector for the `sourceWindow_02` window to include the full path to the `traders.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/connectors.md) document for instructions.

7.  Edit the Subscriber Connector for the `joinWindow_01` window to include the full path to the `output.csv` file that will be created. Refer to the [Editing Connectors](../../../docs/connectors.md) document for instructions.

8.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/testing.md) document for instrcutions.

9.  Execute the model on the ESP Server and Subscribe to the `joinWindow_01` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/executing.md) document for instructions.

10.  Download and open the `output.csv` file created by the model.