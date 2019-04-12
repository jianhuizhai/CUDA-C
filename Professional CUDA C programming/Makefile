APPS=hello

all: ${APPS}

%: %.cu
	nvcc -O2 -arch=sm_35 -o $@ $<
clean:
	rm -f ${APPS}
