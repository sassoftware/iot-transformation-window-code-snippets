# join_exp_xml Instructions

This example contains two source windows joined by a left outer join in a join window.  The join window uses expressions to compute the non-key fields.

Use the following steps to execute the join_exp_xml code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input1.csv` and `input2.csv` files to the server directory you just created.

3.  Upload the `model.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/Uploading_a_Model_to_ESP_Studio.pdf) document for instructions.
  
4.  Double-click the project named `join_exp_xml` to open it.

5.  Edit the Input Data Connector for the `sourceWindow_01` window to include the full path to the `input1.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

6.  Edit the Input Data Connector for the `sourceWindow_02` window to include the full path to the `input2.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

6.  Edit the Subscriber Connector for the `joinWindow_01` window to include the full path to the `output.csv` file that will be created. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

7.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/Testing_Models.pdf) document for instrcutions.

8.  Execute the model on the ESP Server and Subscribe to the `joinWindow_01` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/Executing_a_Model_and_Viewing_the_Output.pdf) document for instructions.

9.  Download and open the `output.csv` file created by the model.
