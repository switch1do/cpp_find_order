cpp_find_order
==============

C++ template optimization - for finding rows by using Full Table Scan (or as part of Range Index Scan in strategy Index Only Scan)

$> testit.py 20

building samples...

2.9    : cl.exe main.c -nologo -O2 -FeMSVC7.1-0.exe <br />
15.0   : cl.exe main.c -nologo -O2 -D_FORCEINLINE -FeMSVC7.1-1.exe <br />
5.2    : cl.exe main.c -nologo -O2 -FeMSVC10.1-0.exe <br />
59.7   : cl.exe main.c -nologo -O2 -D_FORCEINLINE -FeMSVC10.1-1.exe <br />
3.4    : cl.exe main.c -nologo -O2 -FeMSVC11.2-0.exe <br />
5.5    : cl.exe main.c -nologo -O2 -D_FORCEINLINE -FeMSVC11.2-1.exe <br />
1.4    : gcc.exe main.c -O3 -oGCC3-0.exe <br />
2.1    : gcc.exe main.c -O3 -oGCC4-0.exe <br />
2.2    : gcc.exe main.c -O3 -D_FORCEINLINE -oGCC4-1.exe <br />
2.1    : clang.exe main.c -O3 -oCLANG3-0.exe <br />
1.5    : clang.exe main.c -O3 -D_FORCEINLINE -oCLANG3-1.exe <br />
2.3    : icl.exe main.c -nologo -O2 -FeICL12.1-0.exe <br />
2.1    : icl.exe main.c -nologo -O2 -D_FORCEINLINE -FeICL12.1-1.exe <br />

testing samples...

MSVC7.1-0.exe           0.024    0.105    4.375 <br />
MSVC7.1-1.exe           0.011    0.101    9.182 <br />
MSVC10.1-0.exe          0.023    0.063    2.739 <br />
MSVC10.1-1.exe          0.015    0.062    4.133 <br />
MSVC11.2-0.exe          0.023    0.066    2.870 <br />
MSVC11.2-1.exe          0.036    0.066    1.833 <br />
GCC3-0.exe              0.023    0.066    2.870 <br />
GCC4-0.exe              0.023    0.067    2.913 <br />
GCC4-1.exe              0.023    0.066    2.870 <br />
CLANG3-0.exe            0.023    0.055    2.391 <br />
CLANG3-1.exe            0.015    0.054    3.600 <br />
ICL12.1-0.exe           0.019    0.054    2.842 <br />
ICL12.1-1.exe           0.023    0.066    2.870 <br />

