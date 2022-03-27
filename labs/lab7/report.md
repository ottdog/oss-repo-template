# Checkpoint 1
![image](https://user-images.githubusercontent.com/55850761/160262457-6fb2e76a-c7c7-4258-a2e7-3508d59de55a.png)

#Checkpoint 2

1)
The build "Debian_Unstable-Clang-libcxx" passed all 673 tests it was given, including tests such as Alias Target, CheckCompilerRelatedVariables, CMake.EndStuff, and CPackComonents.

Build vs15-64-ninja failed one test: RunCMake.ctest_memcheck. It did not print the expected stdout, or anything to stdout for that matter. Given the test was called DummyValgrindPrePost, it is useful to the devoplers to know the error at least had something to do with memory and valgrind. Normally a good test would help narrow down what the failures could be, but this is a rather vauge error...

I don't know what the exact error in vs15-64-ninja is, but given that it's valgrind related there's probably a memory leak somewhere that I need to be worried about if I keep the program running for extended periods of time

3)
I was unable to install cmake
![image](https://user-images.githubusercontent.com/55850761/160263857-3d266e8b-5e34-43e0-814f-73cc59b841d4.png)

