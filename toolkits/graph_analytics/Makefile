#**
# * @file
# * @author  Danny Bickson
# * @version 1.0
# *
# * @section LICENSE
# *
# * Copyright [2012] [Carngie Mellon University]
# * 
# * Licensed under the Apache License, Version 2.0 (the "License");
# * you may not use this file except in compliance with the License.
# * You may obtain a copy of the License at
# * 
# * http://www.apache.org/licenses/LICENSE-2.0
# * 
# * Unless required by applicable law or agreed to in writing, software
# * distributed under the License is distributed on an "AS IS" BASIS,
# * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# * See the License for the specific language governing permissions and
# * limitations under the License.

#  Makefile for compiling graphchi collaborative filtering library
#  Written by Danny Bickson
INCFLAGS = -I/usr/local/include/ -I../../src/ -I.
CPP = g++
CXX = g++
CPPFLAGS =  -g -O3 $(INCFLAGS)  -fopenmp -Wall -Wno-strict-aliasing

all: $(patsubst %.cpp, %, $(wildcard *.cpp))

%.out: %.h %.hpp %.cpp 
	$(CPP) $(CPPFLAGS) $<  -o $@

clean:
	touch *.cpp

