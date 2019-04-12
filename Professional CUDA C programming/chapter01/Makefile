APPS=hello

all: ${APPS}

%: %.cu
	nvcc -O2 -arch=sm_30 -o $@ $<
clean:
	rm -f ${APPS}
