# edfmex from https://github.com/HukLab/edfmex
A mex file to load edf files into a Matlab struct

Copy edfapi.framework to /Library/Frameworks

In Matlab, change directory to source directory, and then do:

makeHeader
mex edfmex.cpp CXXFLAGS="\$CXXFLAGS -I/Library/Frameworks/edfapi.framework/Headers" LDFLAGS="\$LDFLAGS -framework edfapi"
