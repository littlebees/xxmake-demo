main: main.cpp sta.o dyn.so
	g++ -I~ -o $@ $^


dyn.so: dyn.cpp
	g++ -fPIC -shared -o $@ $^
%.o: %.cpp
	g++ -c -o $@ $<
	# current , first
clean:
	rm *.o *.so

.PHONY: clean
