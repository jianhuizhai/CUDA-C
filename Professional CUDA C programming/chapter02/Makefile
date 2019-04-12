C_APPS = sumArraysOnHost

CU_APPS = checkDimension defineGridBlock sumArraysOnGPU-small-case

all:${C_APPS} ${CU_APPS}

%: %.c
	nvcc -arch=sm_30 -o $@ $<

%: %.cu
	nvcc -arch=sm_30 -o $@ $<

clean:
	rm -f ${C_APPS} ${CU_APPS}
