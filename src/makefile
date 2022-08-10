.PHONY: door_struct list_test
CC =gcc
CFLAGS = -Wall -Werror -Wextra -c
Q1_SOURCES = dmanager_module.c
Q1_OBJECTS = $(Q1_SOURCES:.c=.o)

Q2_SOURCES = list.c list_test.c
Q2_OBJECTS = $(Q2_SOURCES:.c=.o)

EXECUTABLE = main
QUEST = Quest_

all: $(OBJECTS)
	$(CC) $(OBJECTS) -o $(EXECUTABLE)
	
$(EXECUTABLE): $(OBJECTS)
	$(CC) $(OBJECTS) -o $(EXECUTABLE)


door_struct: $(Q1_OBJECTS)
	$(CC) $(Q1_OBJECTS) -o $(QUEST)1

list_test: $(Q2_OBJECTS)
	$(CC) $(Q2_OBJECTS) -o $(QUEST)2

rebuild: clean all

.o: .c
	$(CC) $< -o $@

clean:
	-rm $(OBJECTS)
	-rm $(EXECUTABLE)
	-rm $(QUESTS)
