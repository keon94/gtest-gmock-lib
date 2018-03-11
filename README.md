# gtest-gmock-lib

Visual Studio 2017 Project for compiling gtest 1.8 and gmock 1.7 static libraries.
The source releases for both can be found here:
https://github.com/google/googletest/releases

Everything is set. Just build to get the gtest.lib and gmock.lib files.

If you receive the following error when compiling:

"error C4996: 'std::tr1': warning STL4002: The non-Standard std::tr1
namespace and TR1-only machinery are deprecated and will be REMOVED." 

Right Click on the Project and navigate to 
Properties->Configuration Properties->C/C++->Preprocessor->Preprocessor Definitions and add this entry: _SILENCE_TR1_NAMESPACE_DEPRECATION_WARNING 
