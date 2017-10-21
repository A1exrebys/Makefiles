CC=gcc

O_DIR = ./../obj
I_DIR = ./../include
EXEC_FILE = ./../output

SOURCES := $(wildcard *.c)
OBJECTS := $(SOURCES:.c=.o)

OBJ := $(addprefix $(O_DIR)/,$(OBJECTS))

all: $(OBJECTS)

%.o:%.c
	$(CC) -c -I$(I_DIR) $< -o $(O_DIR)/$@

link:
	$(CC) -o $(EXEC_FILE) $(OBJ)

clean:
	rm -rf $(OBJ) $(EXEC_FILE)
