# union_xml Instructions

This example includes a Union using strict policy.

Use the following steps to execute the union_xml code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input_sw_01_1.csv`, `input_sw_01_2.csv`, and `input_sw_02.csv` files to the server directory you just created.

3.  Upload the `model.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/Uploading_a_Model_to_ESP_Studio.pdf) document for instructions.
  
4.  Double-click the project named `modeling_union` to open it.

5.  Edit the Input Data Connector for the `sourceWindow_01` window to include the full path to the `input_sw_01_1.csv` and `input_sw_01_2.csv` files you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

6.  Edit the Input Data Connector for the `sourceWindow_02` window to include the full path to the `input_sw_02.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.
 
7.  Edit the Subscriber Connector for the `unionWindow_strict` window to include the full path to the `output.csv` file that will be created. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

8.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/Testing_Models.pdf) document for instrcutions.

9.  Execute the model on the ESP Server and Subscribe to the `unionWindow_strict` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/Executing_a_Model_and_Viewing_the_Output.pdf) document for instructions.

10.  Download and open the `output.csv` file created by the model.
