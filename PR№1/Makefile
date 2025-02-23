CC = g++
CFLAGS = -Wall -std=c++11
TARGET = longest_words

all: $(TARGET)

$(TARGET): longest_words.cpp
	$(CC) $(CFLAGS) -o $(TARGET) longest_words.cpp

clean:
	rm -f $(TARGET)

check_compiler:
	@if ! command -v $(CC) &> /dev/null; then \
		echo "Ошибка: Компилятор $(CC) не установлен."; \
		exit 1; \
	fi

install_dependencies:
	sudo apt-get install -y build-essential

.PHONY: all clean check_compiler install_dependencies