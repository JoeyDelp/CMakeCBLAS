cmake_minimum_required(VERSION 3.11 FATAL_ERROR)

project(CMakeCBLAS VERSION 5.2.2 LANGUAGES C)

include(${PROJECT_SOURCE_DIR}/cmake/setup_cblas.cmake)

set(cblas_SRC
	src/caxpy.c
	src/ccopy.c
	src/cdotc.c
	src/cgemv.c
	src/cgerc.c
	src/chemv.c
	src/cher2.c
	src/cscal.c
	src/cswap.c
	src/ctrsv.c
	src/dasum.c
	src/daxpy.c
	src/dcabs1.c
	src/dcopy.c
	src/ddot.c
	src/dgemv.c
	src/dger.c
	src/dnrm2.c
	src/drot.c
	src/dscal.c
	src/dswap.c
	src/dsymv.c
	src/dsyr2.c
	src/dtrsv.c
	src/dzasum.c
	src/dznrm2.c
	src/icamax.c
	src/idamax.c
	src/isamax.c
	src/izamax.c
	src/sasum.c
	src/saxpy.c
	src/scasum.c
	src/scnrm2.c
	src/scopy.c
	src/sdot.c
	src/sgemv.c
	src/sger.c
	src/snrm2.c
	src/srot.c
	src/sscal.c
	src/sswap.c
	src/ssymv.c
	src/ssyr2.c
	src/strsv.c
	src/zaxpy.c
	src/zcopy.c
	src/zdotc.c
	src/zgemv.c
	src/zgerc.c
	src/zhemv.c
	src/zher2.c
	src/zscal.c
	src/zswap.c
	src/ztrsv.c)
	
cblas_target(cblas "${cblas_SRC}")