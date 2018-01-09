# OSARIS
### Open Source SAR Investigation System
OSARIS provides a framework to process large stack of synthetic aperture radar (SAR) data in High Performance Computing (HPC) environments.

### REQUIREMENTS:
1. A working installation of GMT5SAR, further info and installation instructions at
   http://gmt.soest.hawaii.edu/projects/gmt5sar/wiki
2. A working SLURM environment, further info and installation instructions at
   https://slurm.schedmd.com/   

### DOWNLOAD / INSTALLATION
Clone the OSARIS repository:
git clone https://github.com/cryotools/osaris.git

### PREPARATION
- Provide DEM data. You may use the DEM generator: 
  http://topex.ucsd.edu/gmtsar/demgen/

- In the OSARIS folder, copy configuration templates to config folder
> cp ./templates/config.template ./config/_my_study_.config
> cp ./templates/GMTSAR.template ./config/GMTSAR_my_study_.config

- Edit new config files to fit your needs and local configuration.
  See comments in template files for details.

- Make sure .sh files are executable (chmod +x <filename>)


### LAUNCH
Go to the OSARIS folder. Launch your run with
./osaris.sh ./config/_my_config_.config


### Acknowledgements
Thanks to Ziyadin Cakir who supported the conception of OSARIS with thoughtful comments and by sharing scripts.