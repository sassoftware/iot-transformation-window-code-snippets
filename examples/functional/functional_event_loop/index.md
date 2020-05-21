# functional_event_loop Instructions

This is an example of the event looping capabilities of the functional window. The data involved represents several auto accident insurance claims. It is contained in relatively complex XML data. The model takes the XML into its source window and routes the data down different paths representing claims, parties, vehicles, and injuries.

This example is unique in that it uses the ESP Client to publish a file and to subscribe to the output.

Use the following steps to execute the functional_event_loop code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input.xml` and `model.xml` files to the server directory you just created.

3.  Open a terminal window and start the model on the ESP XML Server using the following command. Ensure you use the full path for the model.

~~~bash
dfesp_xml_server -model file:///home/sasdemo/model.xml
~~~
  
4.  Open another terminal window and publish the input file `input.xml` using the ESP Client. Ensure you use the full path for the input file.

~~~bash
dfesp_xml_client -url "http://localhost:51001/SASESP/windows/project/query/source/state?value=injected&eventUrl=file:///home/sasdemo/input.xml" -put
~~~

5.  Subscribe to the `claimStats` window using the ESP Client.

~~~bash
dfesp_xml_client -url "http://localhost:51001/SASESP/events/project/query/claimStats"
~~~

