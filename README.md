## PM4PY for process mining 
// This documentation assumes that the user has basic understanding of process mining and python concepts.


  ## Installation guide for PM4PY 

 __Installing PM4PY on Windows operating system.__
  PM4PY can be installed on windows operating system using two methods one is installing all the necessary libraries needed for processing and visualization and other is installing a zip file directly which is given in the below user manual.

  [Click here](pm4pywindows.pdf) to get user manual for step-by- step installation guide of PM4PY using command line and as well as zip file.

 __Installing PM4PY on Linux opetaing system.__
  You can choose between an Docker image or the classical installation process to get PM4PY up and running on your linux operating system. Find user manual for downloading and installing PM4PY.
  
  [Click here!](pm4pyLinux.pdf) to get user manual for step-by-step installation guide of PM4PY using docker and classical installtion
  
  __Installing PM4PY on mac Operating system.__
   In Mac operating system you can use same docker image to run PM4PY on mac machine or you can use teminal to download PM4PY and run.Find user manual step-by-step guide for installing PM4PY on mac OS
   
   [Click here!](pm4pymacos.pdf) to get user manual for step-by-step installation guide of PM4PY using docker image and classical installation.
   

## Handling Event Data in PM4PY


 __Importing Data__ 

  PM4PY offers simplified interface to import/export event logs. This provides restricted set of choices in comparison to normal interface moreover PM4PY also provides s simple interface to convert the formats of log data objects.
  
  Find python function which provide simplified interface for __Importing IEEE XES__ and __Importing CSV__ files. 
   
   [Click Here!](pm4pyimportieeexes.pdf) for step-by-step guide for importing IEEE XES files.
   IEEE XES is a standard format describing how event logs are stored. For more information about the format, please study the [IEEE XES Website!](http://www.xes-standard.org/)
   
   [Click Here!](pm4pyimportcsv.pdf) for step-by-step guide for importing CSV files.
   
   
   
  __Converting Event Data__
  
  In this section, we describe how to convert event log objects from one object type to another object type. As mentioned in the previous section, the conversion functionality of event logs is located in pm4py.objects.conversion.log.converter. There are three objects, which we are able to 'switch' between, i.e., Event Log, Event Stream and Data Frame objects. Please refer to the previous code snippet for an example of applying log conversion (applied when importing a CSV object). Finally, note that most algorithms internally use the converters, in order to be able to handle an input event data object of any form. In such a case, the default parameters are used.
  
  | Variant | Parameter Key | Type | Default | Description|
  |:---|:----:|:---:|:---:|:---|
  |TO_EVENT_LOG|STREAM_POST_PROCESSING| Boolean | False | Removes events that have no type information.|
  | |CASE_ATTRIBUTE_PREFIX|string|'case:'|Any attribute (column in case of DF) with the prefix 'case:' is stored as a trace attribute.|
  | |	CASE_ID_KEY|	string|'case:concept:name'|Attribute (column in case of DF) that needs to be used to define traces.|
  | |DEEP_COPY|boolean|false|If set to True objects will be created using a deep-copy (if applicable). Avoids side-effects (specifically when converting an Event Stream to an Event Log).|
  |TO_EVENT_STREAM|	STREAM_POST_PROCESSING|boolean|false|(Same as TO_EVENT_LOG)|
  | |CASE_ATTRIBUTE_PREFIX|string|'case:'|Any trace attribute (in case of converting an Event Log to an Event Stream object) will get this prefix. Not applicable if we translate a DataFrame to an Event Stream object.|
  ||DEEP_COPY|boolean|false|(Same as TO_EVENT_LOG)|
  |TO_DATA_FRAME|CASE_ATTRIBUTE_PREFIX|string|'case:'|(Same as TO_EVENT_STREAM; will only be applied if input is an Event Log object, i.e., which will first be translated to an Event Stream Object.)|
  | |DEEP_COPY|boolean|false|(Same as TO_EVENT_STREAM)|
  
  
  __Exporting Data__
  
  [Click Here!](pm4pyexportieeexes.pdf) for step by step guide for exporting IEEE XES files
  [Click Here!](pm4pyexportcsv.pdf) for step by step guide for exporting CSV files
  
  
