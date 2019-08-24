## JAX-P
Java Api for XML Processing

Implementation of JAX-p : Crimson, Xerces2, Oracle V2 Parser etc. and in Java 1.5+ Xerces2 is by default available 

## XML Processing Methodologies:
For processing the XML there are may  method. Some of method are :

 1. SAX
 2. DOM.
 3. STAX
 
 

## SAX

 - Simple Access for XML.
 - Event based processing model. It contain 3 actor:
	 1. **Source:** :Originator of event , who could raise serveral type of event.
	 2. **Listner** : It will listen the event from the source.
	 3. **Event Handler**: One event listen it will be given to event handler for processing the event.
 - Process XML elements sequentially from top to the bottom. While processing the document, it places a pointer to the document and increments sequentially from the top.
 
 

## DOM:

 - Document Object Modal.
 - Read XML in Hierarchical fashion. Tree based.
 - When it reads the entire XML into the memory, loads it and builds a content tree.
 - As it is in memory we can navigate in Random Order.
 - Adding in DOM is called Node. There are serval type of Node like Document Node, Element Node, Text Node.
 - When it load the XML it place pointer to top level i.e root which is called Document Node.
 - To navigate between Them we can traverse.
 
 
 

## STAX Iterator:

The StAX API exposes methods for iterative, event-based processing of XML documents. It is pull based event parser.
In Stax we don't have schma validation

## Push Based v/s Pull Based Parsor.
In push based XML data call the client . SAX parser call the the event handler . So in push we dont have control when and how the parser iterate the file. Once we start paser it iterate through end. 
In Pull based mean Handle will call the XML data i.e parser. So Handler control when the parser is to move on next event. And also we can stop parsing at any point.

## Difference Between SAX and DOM
|SAX| DOM |
|--|--|
| Event based |hierarchical Processing  |
|Process XML sequentially| Process XML at once|
|Consume less memory | Consume More Meory|
|Faster Compared to DOM. No need to load anything | Slower then SAX. Need to load XML first|
| Cant access element of XML random| Access element of XML Random|



 - 
