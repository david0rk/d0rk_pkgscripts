This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 

This is a collection of scripts i've made for my own personal use. 
They may be useful for other people,  alternatively they could potentially cause problems on certain setups/configurations so USE AT YOUR OWN RISK.


doclean automates apt-get autoclean/autoremove, runs deborphan and removes/purges orphaned packages.  you can create a file named .whitelist of packages you don't want removed.
requires: debian/apt based package management

doupdate automates apt-get upgrade, apt-get update.
requires: same as doclean



lspkg:Generates a list of packages installed on the machine and saves to a specified filename, otherwise (uname -n).pkglist
Usage: lspkg-diff (filename (optional))

lspkg-diff:  compares two lists of packages and generates a list of packages unique to each system.
Usage: ./lspkg-diff system1.pkglist system2.pkglist, Generates (inputfile1).pkgdiff (inputfile2).pkgdiff
