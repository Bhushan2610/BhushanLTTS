# Name of the project
PROJECT_NAME = Game

# Output directory
BUILD = build

# All source code files
SRC = PROJECT.\
src/testproject.c\


# All test source files
TEST_SRC = src/PROJECT.c\
src/PROJECT.c\
test/testproject.c\
unity/unity.c\

TEST_OUTPUT = $(BUILD)/Test_$(PROJECT).exe

# All include folders with header files
INC	= -Iinc\
-Iunity\

#Library Inlcudes
#if working with CUnit 
#INCLUDE_LIBS = -lcunit
INCLUDE_LIBS =

# Project Output name
PROJECT_OUTPUT = $(BUILD)/$(PROJECT).exe

# Document files
DOCUMENTATION_OUTPUT = documentation/html

# Default target built
$(PROJECT_NAME):all

# Run the target even if the matching name exists
.PHONY: run clean test doc all

all: $(SRC) $(BUILD)
	gcc $(SRC) $(INC) -o $(PROJECT).exe

# Call `mingw32-make` to run the application
run:$(PROJECT_NAME)
	./$(PROJECT_OUTPUT).out




# Build and run the unit tests
test:$(BUILD)
	gcc $(TEST_SRC) $(INC) -o $(TEST_OUTPUT)
	./$(TEST_OUTPUT)

	./$(TEST_OUTPUT)


# Create new build folder if not present
$(BUILD):
	mkdir build
