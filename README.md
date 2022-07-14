Purpose of the work: Create two JavaBeans components for presenting a set of experimental data:
• a component for tabular presentation of a data set and work with it;
• a component for graphical representation of a data set.
1.2 Implementation of basic classes
As for the implementation, the main code examples will be given in the appendices. In this section, we will describe each of the main classes of the project:
• Data: class for representing a string with data.
• DataHandler:
• DataSheet: a class that provides the entire data set (Listing A.1).
• DataSheetChangeEvent: a class that inherits from the EventObject class and contains a field with serialization control.
• DataSheetChangeListener: An interface that follows the EventListener class.
• DataSheetGraph: A derived class from JPanel. Contains a field with serialization control. The showGraph() method directly draws the graph (Listing A.2).
• DataSheetTable: a class for table display of data and working with it. This class extends the standard JPanel class (Listing A.3).
• DataSheetTableModel: A visual model class that contains the data structure, including the contents of the table cells. This class contains a list in which all listeners connected to the component will be stored. When an event occurs, all listeners from this list will receive the necessary information about it.
• XMLParser: a class designed to create a DOM object based on the data structure and save it to a file (Listing A.4).
• MainFrame: the successor class of the JFrame class, in which we create the main window of our program (Listing A.5).
