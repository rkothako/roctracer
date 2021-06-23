# ROC-tracer
```
ROC-tracer library: Runtimes Generic Callback/Activity APIs.
The goal of the implementation is to provide a generic independent from
specific runtime profiler to trace API and asyncronous activity.

The API provides functionality for registering the runtimes API callbacks and
asyncronous activity records pool support.

ROC-TX librray: code annotation evemts API
Includes basic API: roctxMark, roctxRangePush, roctxRangePop.
```

## Usage
```
rocTracer API:
  To use the rocTracer API you need the API header and to link your application with roctracer .so librray:
  - the API header: /opt/rocm/roctracer/include/roctracer.h
  - the .so library: /opt/rocm/lib/libroctracer64.so

rocTX API:
  To use the rocTX API you need the API header and to link your application with roctx .so librray:
  - the API header: /opt/rocm/roctracer/include/roctx.h
  - the .so library: /opt/rocm/lib/libroctx64.so
```

## The library source tree
```
 - doc - documentation
 - inc/roctracer.h - rocTacer library public API header
 - inc/roctx.h - rocTX library puiblic API header
 - src  - Library sources
   - core - rocTracer library API sources
   - roctx - rocTX library API sources
   - util - library utils sources
 - test - test suit
   - MatrixTranspose - test based on HIP MatrixTranspose sample
```

## Documentation
 - API description: 
   - ['roctracer' / 'rocTX' profiling C API specification](doc/roctracer_spec.md)
 - Code examples:
   - [test/MatrixTranspose_test/MatrixTranspose.cpp](test/MatrixTranspose_test/MatrixTranspose.cpp)
   - [test/MatrixTranspose/MatrixTranspose.cpp](test/MatrixTranspose/MatrixTranspose.cpp)

## To build and run test
```
 Please follow the instructions mentioned @ https://rocmdocs.amd.com/en/latest/Installation_Guide/Tools-Installation.html
```
