# Copyright (c) 2006, 2010, Oracle and/or its affiliates. All rights reserved.
# 
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; version 2 of the License.
# 
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# 
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

INCLUDES = -I$(srcdir)/../include -I$(srcdir)/../mySTL
noinst_PROGRAMS    = benchmark
benchmark_SOURCES  = benchmark.cpp
benchmark_LDADD    = $(top_builddir)/extra/yassl/taocrypt/src/libtaocrypt.la
benchmark_CXXFLAGS = -DYASSL_PURE_C @yassl_thread_cxxflags@
EXTRA_DIST = benchmark.dsp rsa1024.der dh1024.der dsa1024.der make.bat

# Don't update the files from bitkeeper
%::SCCS/s.%
