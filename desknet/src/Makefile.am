# Desknet version 0.1
# Copyright 2014 by John Slayton

# Process this file with automake to produce Makefile.in.
#
# This program is free software; you can redistribute it and/or modify 
# it under the terms of the GNU General Public License as published by 
# the Free Software Foundation; either version 3 of the License, or (at 
# your option) any later version.

# This program is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
# General Public License for more details.

# You should have received a copy of the GNU General Public License 
# along with this program; if not, write to the Free Software Foundation,
# Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA

# Author's address as of 9.30.04 is 260 Sundance Ct, Azusa, CA 91792. */

SHELL = /bin/sh

SUFFIXES: .c .o

bin_PROGRAMS=dnet
dnet_SOURCES=dnet.o

CC=cc

INSTALL=install

srcdir=@srcdir@
prefix=@prefix@
exec_prefix=@exec_prefix@
bindir=@bindir@
datarootdir=@datarootdir@
infodir=@infodir@

AM_CFLAGS = -g
all  :  

dnet$(EXEEXT)  :  dnet.o
	-$(CC) -o dnet -lSDL2 -lrt  -lSDL2_ttf dnet.o $(CFLAGS)
dnet.o : dnet.c
	-$(CC) -c -o dnet.o -O2  ./dnet.c $(CFLAGS)

.PHONEY : $(INSTALL)
$(INSTALL) : dnet 

	-$(INSTALL_PROGRAM) deskplan $(bindir)
	-$(INSTALL_PROGRAM) createkey $(bindir)
	$(INSTALL_DATA) ../doc/desknet.info $(infodir)

	-mkdir $(prefix)/etc

	$(INSTALL_DATA) pass $(prefix)/etc
	$(INSTALL_DATA) net_size $(prefix)/etc

	-mkdir $(prefix)/etc/events
	$(INSTALL_DATA) bufa $(prefix)/etc/events
	$(INSTALL_DATA) bufb $(prefix)/etc/events
	$(INSTALL_DATA) bufc $(prefix)/etc/events
	$(INSTALL_DATA) bufd $(prefix)/etc/events
	$(INSTALL_DATA) bufe $(prefix)/etc/events
	$(INSTALL_DATA) buff $(prefix)/etc/events
	$(INSTALL_DATA) bufg $(prefix)/etc/events
	$(INSTALL_DATA) bufh $(prefix)/etc/events
	$(INSTALL_DATA) bufi $(prefix)/etc/events
	$(INSTALL_DATA) bufj $(prefix)/etc/events
	$(INSTALL_DATA) bufk $(prefix)/etc/events
	$(INSTALL_DATA) bufl $(prefix)/etc/events
	$(INSTALL_DATA) bufm $(prefix)/etc/events
	$(INSTALL_DATA) bufn $(prefix)/etc/events
	$(INSTALL_DATA) bufo $(prefix)/etc/events
	$(INSTALL_DATA) bufp $(prefix)/etc/events
	$(INSTALL_DATA) bufq $(prefix)/etc/events
	$(INSTALL_DATA) bufr $(prefix)/etc/events
	$(INSTALL_DATA) bufs $(prefix)/etc/events
	$(INSTALL_DATA) buft $(prefix)/etc/events
	$(INSTALL_DATA) bufu $(prefix)/etc/events
	$(INSTALL_DATA) bufv $(prefix)/etc/events
	$(INSTALL_DATA) bufw $(prefix)/etc/events
	$(INSTALL_DATA) bufx $(prefix)/etc/events
	$(INSTALL_DATA) bufy $(prefix)/etc/events
	$(INSTALL_DATA) bufz $(prefix)/etc/events
	$(INSTALL_DATA) bufaa $(prefix)/etc/events
	$(INSTALL_DATA) bufab $(prefix)/etc/events
	$(INSTALL_DATA) bufac $(prefix)/etc/events
	$(INSTALL_DATA) bufad $(prefix)/etc/events
	$(INSTALL_DATA) bufae $(prefix)/etc/events
	$(INSTALL_DATA) bufaf $(prefix)/etc/events
	$(INSTALL_DATA) bufag $(prefix)/etc/events
	$(INSTALL_DATA) bufah $(prefix)/etc/events
	$(INSTALL_DATA) bufai $(prefix)/etc/events
	$(INSTALL_DATA) bufaj $(prefix)/etc/events
	$(INSTALL_DATA) bufak $(prefix)/etc/events
	$(INSTALL_DATA) bufal $(prefix)/etc/events
	$(INSTALL_DATA) bufam $(prefix)/etc/events
	$(INSTALL_DATA) bufan $(prefix)/etc/events

	-mkdir $(prefix)/etc/answerkeys
	$(INSTALL_DATA) template $(prefix)/etc/answerkeys
	$(INSTALL_DATA) text1 $(prefix)/etc/answerkeys
	$(INSTALL_DATA) text2 $(prefix)/etc/answerkeys
	$(INSTALL_DATA) text3 $(prefix)/etc/answerkeys
	$(INSTALL_DATA) text4 $(prefix)/etc/answerkeys

	-mkdir $(prefix)/etc/fonts
	-mkdir $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) COPYRIGHT.TXT $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) local.conf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) README.TXT $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) RELEASENOTES.TXT $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraBd.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraBI.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraIt.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraMoBd.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraMoBI.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraMoIt.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraMono.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraSeBd.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) VeraSe.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10
	$(INSTALL_DATA) Vera.ttf $(prefix)/etc/fonts/ttf-bitstream-vera-1.10

	-mkdir -p $(prefix)/com
	-mkdir $(prefix)/com/class1        

	-mkdir $(prefix)/com/class1/names
	$(INSTALL_DATA) teacher $(prefix)/com/class1/names

	-mkdir $(prefix)/com/class1/student
	
	-mkdir $(prefix)/com/class1/files

	-mkdir $(prefix)/com/class1/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class1/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class1/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class1/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class1/settings
	$(INSTALL_DATA) terma $(prefix)/com/class1/settings
	$(INSTALL_DATA) termb $(prefix)/com/class1/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class1/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class1/settings

# **************

	-mkdir $(prefix)/com/class2        
	-mkdir $(prefix)/com/class2/names
	$(INSTALL_DATA) teacher $(prefix)/com/class2/names
	-mkdir $(prefix)/com/class2/files
	-mkdir $(prefix)/com/class2/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class2/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class2/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class2/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class2/settings
	$(INSTALL_DATA) terma $(prefix)/com/class2/settings
	$(INSTALL_DATA) termb $(prefix)/com/class2/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class2/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class2/settings
	-mkdir $(prefix)/com/class2/student
        
# ***************

	-mkdir $(prefix)/com/class3        
	-mkdir $(prefix)/com/class3/names
	$(INSTALL_DATA) teacher $(prefix)/com/class3/names
	-mkdir $(prefix)/com/class3/files
	-mkdir $(prefix)/com/class3/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class3/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class3/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class3/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class3/settings
	$(INSTALL_DATA) terma $(prefix)/com/class3/settings
	$(INSTALL_DATA) termb $(prefix)/com/class3/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class3/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class3/settings
	-mkdir $(prefix)/com/class3/student
        
# *****************

	-mkdir $(prefix)/com/class4        
	-mkdir $(prefix)/com/class4/names
	$(INSTALL_DATA) teacher $(prefix)/com/class4/names
	-mkdir $(prefix)/com/class4/files
	-mkdir $(prefix)/com/class4/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class4/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class4/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class4/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class4/settings
	$(INSTALL_DATA) terma $(prefix)/com/class4/settings
	$(INSTALL_DATA) termb $(prefix)/com/class4/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class4/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class4/settings
	-mkdir $(prefix)/com/class4/student

# ******************

	-mkdir $(prefix)/com/class5        
	-mkdir $(prefix)/com/class5/names
	$(INSTALL_DATA) teacher $(prefix)/com/class5/names
	-mkdir $(prefix)/com/class5/files
	-mkdir $(prefix)/com/class5/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class5/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class5/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class5/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class5/settings
	$(INSTALL_DATA) terma $(prefix)/com/class5/settings
	$(INSTALL_DATA) termb $(prefix)/com/class5/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class5/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class5/settings
	-mkdir $(prefix)/com/class5/student
        
# ****************

	-mkdir $(prefix)/com/class6        
	-mkdir $(prefix)/com/class6/names
	$(INSTALL_DATA) teacher $(prefix)/com/class6/names
	-mkdir $(prefix)/com/class6/files
	-mkdir $(prefix)/com/class6/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class6/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class6/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class6/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class6/settings
	$(INSTALL_DATA) terma $(prefix)/com/class6/settings
	$(INSTALL_DATA) termb $(prefix)/com/class6/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class6/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class6/settings
	-mkdir $(prefix)/com/class6/student
        
# ********************

	-mkdir $(prefix)/com/class7        
	-mkdir $(prefix)/com/class7/names
	$(INSTALL_DATA) teacher $(prefix)/com/class7/names
	-mkdir $(prefix)/com/class7/files
	-mkdir $(prefix)/com/class7/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class7/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class7/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class7/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class7/settings
	$(INSTALL_DATA) terma $(prefix)/com/class7/settings
	$(INSTALL_DATA) termb $(prefix)/com/class7/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class7/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class7/settings
	-mkdir $(prefix)/com/class7/student
        
# *********************

	-mkdir $(prefix)/com/class8        
	-mkdir $(prefix)/com/class8/names
	$(INSTALL_DATA) teacher $(prefix)/com/class8/names
	-mkdir $(prefix)/com/class8/files
	-mkdir $(prefix)/com/class8/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class8/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class8/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class8/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class8/settings
	$(INSTALL_DATA) terma $(prefix)/com/class8/settings
	$(INSTALL_DATA) termb $(prefix)/com/class8/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class8/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class8/settings
	-mkdir $(prefix)/com/class8/student
        
# ********************

	-mkdir $(prefix)/com/class9        
	-mkdir $(prefix)/com/class9/names
	$(INSTALL_DATA) teacher $(prefix)/com/class9/names
	-mkdir $(prefix)/com/class9/files
	-mkdir $(prefix)/com/class9/settings
	$(INSTALL_DATA) addpoints $(prefix)/com/class9/settings
	$(INSTALL_DATA) divpoints $(prefix)/com/class9/settings
	$(INSTALL_DATA) mulpoints $(prefix)/com/class9/settings
	$(INSTALL_DATA) subpoints $(prefix)/com/class9/settings
	$(INSTALL_DATA) terma $(prefix)/com/class9/settings
	$(INSTALL_DATA) termb $(prefix)/com/class9/settings
	$(INSTALL_DATA) type_line $(prefix)/com/class9/settings
	$(INSTALL_DATA) win_score $(prefix)/com/class9/settings
	-mkdir $(prefix)/com/class9/student
        
.PHONEY   : uninstall
uninstall :
	rm -r -f $(prefix)/com/class1
	rm -r -f $(prefix)/com/class2
	rm -r -f $(prefix)/com/class3
	rm -r -f $(prefix)/com/class4
	rm -r -f $(prefix)/com/class5
	rm -r -f $(prefix)/com/class6
	rm -r -f $(prefix)/com/class7
	rm -r -f $(prefix)/com/class8
	rm -r -f $(prefix)/com/class9
	rm -r -f $(prefix)/etc/fonts
	rm -r -f $(prefix)/etc/pass
	rm -r -f $(prefix)/etc/net_size
	rm -r -f $(prefix)/etc/answerkeys
	rm -r -f $(prefix)/etc/events
	rm -f $(bindir)/deskplan
	rm -f $(bindir)/dnet
	rm -f $(bindir)/createkey
	rm -f $(infodir)/deskplan.info
