EXAMPLES = \
	allocator \
	bulk_oneway_always_blocking \
	bulk_oneway_never_blocking \
	bulk_oneway_possibly_blocking \
	oneway_always_blocking \
	oneway_never_blocking \
	oneway_never_blocking_continuation \
	oneway_possibly_blocking \
	polymorphic_bulk_oneway_always_blocking \
	polymorphic_bulk_oneway_never_blocking \
	polymorphic_bulk_oneway_possibly_blocking \
	polymorphic_oneway_always_blocking \
	polymorphic_oneway_never_blocking \
	polymorphic_oneway_never_blocking_continuation \
	polymorphic_oneway_possibly_blocking

CXXFLAGS = -std=c++17 -pthread -Wall -Wextra -I../../include

.PHONY: all clean

all: $(EXAMPLES)

clean:
	rm -f $(EXAMPLES)

$(EXAMPLES): %: %.cpp
	$(CXX) $(CXXFLAGS) -o$@ $<
