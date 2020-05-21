# ESP Transformation Windows Code Snippets

## Overview

This repository includes code snippets that you can execute for the Transformation windows of SAS Event Stream Processing (ESP). There is a directory for each example that contains all the files you need to execute the example. There is also a document for each code snippet to provide any instructions unique to the particular example.

The following sections list the examples and provide a description of each. You can click on the name of each example to go to the appropriate diretory containing the files.

### Aggregate Window

The Aggregate window allows to perform calculations on non-key fields. The following examples demonstrate the use of the Aggregate window. 

| Example | Description |
| ------ | ------ |
| [aggregate_exp_xml](examples/aggregate/aggregate_exp_xml) | This example includes a single source window followed by an aggregate window that uses expressions to calculate the non-key field values. This is the XML expression version of the XML modeling example aggregate_func_xml. |

### Compute Window

The Compute window enables a one-to-one transformation of input events to output events through the computational manipulation of the input event stream fields. The following examples demonstrate the use of the Compute window. 

| Example | Description |
| ------ | ------ |
| [compute_exp_udf_xml](examples/compute/compute_exp_udf_xml) | This example includes a single source window followed by a compute window that uses user defined functions to calculate the non-key field values. | 
| [compute_exp_xml](examples/compute/compute_exp_xml) | This example includes a single source window followed by a compute window that uses expressions to calculate the non-key field values. |

### Copy Window

The Copy window allows you to copy a parent window and retain events through retention policies. The following examples demonstrate the use of the Copy window. 

| Example | Description |
| ------ | ------ |
| [copy_with_retention_xml](examples/copy/copy_with_retention_xml) | This example contains a single source window followed by one copy window. The copy window retains events for 300 seconds based on a field in the event. |
| [copy_with_slots_xml](examples/copy/copy_with_slots_xml) | This example contains a source window using output slots to feed different event subsets to three copy windows based on an output slot function. | 

### Filter Window

Filter windows use expressions, user-defined functions, and registered plug-in functions to determine what input events are permitted to stream through. The following examples demonstrate the use of the Filter window. 

| Example | Decsription |
| ------ | ------ |
| [filter_exp_xml](examples/filter/filter_exp_xml) | This example contains a single source window and filter window with a filter expression. |
| [filter_on_flag_xml](examples/filter/filter_on_flag_xml) | This example contains a single source window followed by one filter window. The filter window uses ESP_FLAGS to filter out all retention deletes. |
| [filter_on_opcode_xml](examples/filter/filter_on_opcode_xml) | This example contains a single source window followed by one filter window. The filter window uses ESP_OPCODE to filter out all but events with an opCode of insert. |

###  Functional Window

The Functional window calls functions to manipulate and transform event fields. The following example demonstrates the use of the Functional window. 

| Example | Description |
| ------ | ------ |
| [functional_event_loop](examples/functional/functional_event_loop) | This is an example of the event looping capabilities of the functional window. The data involved represents several auto accident insurance claims. It is contained in relatively complex XML data. The model takes the XML into its source window and routes the data down different paths representing claims, parties, vehicles, and injuries. |
 
### Join Window

The Join window receives events from a left input window and a right input window and combines them into a single event stream. The following examples demonstrate the use of the Join window. 

| Example | Description |
| ------ | ------ |
| [join_exp_xml](examples/join/join_exp_xml) | This example contains two source windows joined by a left outer join in a join window.  The join window uses expressions to compute the non-key fields. |
| [join_select_xml](examples/join/join_select_xml) | This example contains two source windows joined by a left outer join in a join window.  The join window uses field-selections to select the non-key fields. | 

### Remove State Window

The Remove State window allows you to transition a stateful part of a model into a stateless part of a model. The following example demonstrates the use of the Remove State window.

| Example | Description |
| ------ | ------ |
| [removeState](examples/removeState/removeState) | This example demonstrates how to facilitate the transition of a stateful part of a model to a stateless part of a model. |

### Transpose Window

The Transpose window changes a event rows as columns, or columns as event rows. The following examples demonstrate the use of the Transpose window. 

| Example | Description |
| ------ | ------ |
| [transpose_long](examples/transpose/transpose_long) | This example transposes information in long mode. You will process information about the pitch, yaw, roll, and velocity of an aircraft in flight. |
| [transpose_wide](examples/transpose/transpose_wide) | This example transposes information in wide mode. You will process information about the pitch, yaw, roll, and velocity of an aircraft in flight. | 

### Union Window

The Union window takes two or more event streams and combines them into a single stream. The following example demonstrates the use of the Union window.

| Example | Description |
| ------ | ------ |
| [union_xml](examples/union/union_xml) | Union using strict policy |
 
 
## Contributing

> We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to submit contributions to this project. 

## License

> This project is licensed under the [Apache 2.0 License](LICENSE).

## Additional Resources

* [SAS Event Stream Processing 6.2 Product Documentation](https://go.documentation.sas.com/?cdcId=espcdc&cdcVersion=6.2&docsetId=espov&docsetTarget=home.htm&locale=en)

