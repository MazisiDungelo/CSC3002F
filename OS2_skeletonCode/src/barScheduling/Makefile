JAVAC = javac
JAVAFLAGS = -cp . -d .

# List of Java source files
SOURCES = DrinkOrder.java  Patron.java Barman.java SchedulingSimulation.java 

# List of class files to be compiled
CLASSES = $(SOURCES:.java=.class)

# Compile Java source files into class files
%.class: %.java
	$(JAVAC) $(JAVAFLAGS) $<

# Compile all classes
all: $(CLASSES)

# Run
run: all
	java -cp . SchedulingSimulation

# Clean up generated class files
clean:
	$(RM) $(CLASSES)
	$(RM) *.class