# copy_with_slots_xml Instructions

This example contains a source window using output slots to feed different event subsets to three copy windows based on an output slot function.

Use the following steps to execute the copy_with_slots_xml code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input.csv` file to the server directory you just created.

3.  Upload the `model.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](docs/Uploading_a_Model_to_ESP_Studio.pdf) document for instructions.
  
4.  Double-click the project named `copy_with_slots_xml` to open it.

5.  Edit the Input Data Connector for the `sourceWindow_01` window to include the full path to the `input.csv` file you uploaded. Refer to the [Editing Connectors](docs/Connectors.pdf) document for instructions.

6.  Edit the Subscriber Connector for the `copyWindow_01` window to include the full path to the `copy1.csv` file that will be created. Refer to the [Editing Connectors](docs/Connectors.pdf) document for instructions.  

7.  Edit the Subscriber Connector for the `copyWindow_02` window to include the full path to the `copy2.csv` file that will be created. Refer to the [Editing Connectors](docs/Connectors.pdf) document for instructions. 

8.  Edit the Subscriber Connector for the `copyWindow_03` window to include the full path to the `copy3.csv` file that will be created. Refer to the [Editing Connectors](docs/Connectors.pdf) document for instructions. 

9.  Save your changes and test your model. Refer to the [Testing Models](docs/Testing_Models.pdf) document for instrcutions.

10.  Execute the model on the ESP Server and Subscribe to the `copyWindow_01`, `copyWindow_02`, and `copyWindow_03` windows using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](docs/Executing_a_Model_and_Viewing_the_Output.pdf) document for instructions.

11.  Download and open the `copy1.csv`, `copy2.csv`, and `copy3.csv` files created by the model.
