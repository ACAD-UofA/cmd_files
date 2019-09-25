#####################
# New Mac Install
#####################

### New OS or Time Machine transfer
### if clean install:

### Finder
- Preferences/	Show these items on the Desktop -> External disks
				New Finder windows show -> "home" (your name)
				Sidebar -> AirDrop - Applications - "home"
- View/Show Status Bar

### Copy all content of the USB stick/drive to the computer (e.g., /home/Soft)

### Internet
# Connect Wifi, choose UofA, enter login/password when prompted, NO PROXY
# Plug ethernet
- SystPreferences/Network/Ethernet/Configure IPv4 -> Using DHCP with manual address
129.127.100.XX (find available address)
	Advanced/Proxies
www-proxy.adelaide.edu.au	3128
login/password
OK + Apply
# If doens't work (which will happen...) talk to Julien/Bastien

### Shared Drive
Prompt new server connection in Finder/Go/Connect to server (or cmd+k)
smb://uofasciences.ad.adelaide.edu.au/ees/ACAD
(click on "+" to save it as favorite)

### Uni disks/system (this would allow you to access your university storage)
Same process than for the Shared Drive
smb://uofausers3.ad.adelaide.edu.au/users3/a1186063
# 3 in 'users3' = last number of your uni ID

### Printer
Install the Printer Driver "bizhub_C554_108.pkg"
Go to System Preferences/Print&Scan
Add
IP
Line Printer Daemon - LPD
Adress: 10.66.4.43
Print Using: Select Printer Software -> KONICA MINOLTA C554 PS


### System Configuration (Juju's way...)
- SystPreference/Mission Control	-> untick "Automatically rearrange..."
									-> Hot Corners to Mission Control - Desktop - Launchpad - Notification Centre
- Add desktops (Mission Control then pointer at top-right)
- SystPreference/Keyboard/Keyboard Shortcuts/	Full Keyboard Access -> All controls
												Mission Control -> Switch to desktop 1...
- SystPreference/Mouse/	Scroll direction
						Secondary click
- SystPreference/Accessibility -> Enable access for assisive devices


### Software (from the copied file on the computer, not from the USB stick!)
# Copy the content of /ApplicationsToCopy/ directly in your /Applications folder

# Adobe Photoshop/Illustrator...
Use "MasterCollection_CS5_LS1.dmg" to install, and "MasterCollection_CS5_LS1.txt" for the code
DO NOT REGISTER - use the 'skip registration' option

# Microsoft office
Use "SW_DVD5_Office_Mac_Standard_2011_English_MLF_X16-99088.ISO" to install (no code required)
Tick the automatically update option
Do the first update (~20MB), but cancel the following one (Service pack 14.10 ~200MB - it was already copied from the USB stick)
Install "Office2011-1410UpdateEN.dmg"
then "Office2011-1423UpdateEN.dmg"

# Endnote
/Endnote/EndNoteX6.dmg


## A bit more advanced, if you need to use NGS tools, scripts, and the terminal as a routine:

# Command line tools (compilers)
/Apple/command_line_tools_for_xcode_os_x_mountain_lion_April2013.dmg

# Path and bin
copy /Lab/bin_app in ~/ (home) - that contains a batch of precompiled lab soft
create bin if necessary
edit and copy 'bash_profile' in ~/.bash_profile

# Install "/Lab/cutadapt-1.2.1.tar.gz"
Unzip
open terminal
cd in the cutadapt folder, then
python setup.py build
sudo python setup.py install

# R from terminal
install R through MacPorts (see in /MacPorts/cmd_MacPorts.txt)
install required package with following commands (this is the list of the packages I use):

r
install.packages("adegenet", repos='http://cran.us.r-project.org')
install.packages("adephylo", repos='http://cran.us.r-project.org')
install.packages("akima", repos='http://cran.us.r-project.org')
install.packages("ape", repos='http://cran.us.r-project.org')
install.packages("bitops", repos='http://cran.us.r-project.org')
install.packages("caTools", repos='http://cran.us.r-project.org')
install.packages("CircStats", repos='http://cran.us.r-project.org')
install.packages("gdata", repos='http://cran.us.r-project.org')
install.packages("gee", repos='http://cran.us.r-project.org')
install.packages("gplots", repos='http://cran.us.r-project.org')
install.packages("gtools", repos='http://cran.us.r-project.org')
install.packages("igraph", repos='http://cran.us.r-project.org')
install.packages("KernSmooth", repos='http://cran.us.r-project.org')
install.packages("lattice", repos='http://cran.us.r-project.org')
install.packages("lmodel2", repos='http://cran.us.r-project.org')
install.packages("locfit", repos='http://cran.us.r-project.org')
install.packages("MASS", repos='http://cran.us.r-project.org')
install.packages("mclust", repos='http://cran.us.r-project.org')
install.packages("pegas", repos='http://cran.us.r-project.org')
install.packages("phylobase", repos='http://cran.us.r-project.org')
install.packages("phylotools", repos='http://cran.us.r-project.org')
install.packages("phytools", repos='http://cran.us.r-project.org')
install.packages("picante", repos='http://cran.us.r-project.org')
install.packages("plyr", repos='http://cran.us.r-project.org')
install.packages("reshape", repos='http://cran.us.r-project.org')
install.packages("rgl", repos='http://cran.us.r-project.org')
install.packages("scatterplot3d", repos='http://cran.us.r-project.org')
install.packages("sm", repos='http://cran.us.r-project.org')
install.packages("smatr", repos='http://cran.us.r-project.org')

install.packages("inline", repos='http://cran.us.r-project.org')
install.packages("ggplot2", repos='http://cran.us.r-project.org')
install.packages("gam", repos='http://cran.us.r-project.org')
install.packages("Rcpp", repos='http://cran.us.r-project.org')
install.packages("RcppGSL", repos='http://cran.us.r-project.org')
q()


