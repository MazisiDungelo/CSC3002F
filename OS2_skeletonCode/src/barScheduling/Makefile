	JAVAC = javac
	JAVAFLAGS = -cp . -d bin

	# List of Java source files
	SOURCES = Barman.java DrinkOrder.java Patron.java SchedulingSimulation.java

	# List of class files to be compiled
	CLASSES = $(SOURCES:.java=.class)

	# Compile Java source files into class files
	%.class: %.java
		$(JAVAC) $(JAVAFLAGS) $<

	# Compile all classes
	all: $(CLASSES)

	# Clean up generated class files
	clean:
		$(RM) $(CLASSES)
		$(RM) bin/*.class