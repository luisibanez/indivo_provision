This is an automation library to build an [Indivo X](http://indivohealth.org/) install from scratch on a rackspace cloud server instance.

[Indivo X Installation Guide](http://wiki.chip.org/indivo/index.php/HOWTO:_install_Indivo_X#Database_Install)

#Prerequisites
* bourne-compatible shell
* python 2.6 or newer

#Dependencies

As long as the prerequisites listed above are already available on your system (any modern Linux or Mac computer will have them),
the code can automatically download and install the rest of its dependencies.

* node.js v0.6 and npm modules as listed in `package.json`

#Installation
* clone this repository to a Mac or Linux computer
* cd into the repository root directory
* ./do setup

#Configuration

* Edit conf.coffee and fill in your rackspace account name
* You do not need to put your API key into the conf file since it is secret. You will be securely prompeted for it when needed.

#Provisioning a new Indivo X server on Rackspace
* cd into the repository root directory
* Run the following "do" commands

  ./do staging provision
  ./do staging user
  ./do staging packages
  ./do staging easyInstall
  ./do staging indivoDB
  ./do staging indivoServer
