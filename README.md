# GEOF348 Linux/Cyclone/GREB cheatsheet

This repository contains some of the most useful commands for Linux/Cyclone/GREB for the GEOF348 assignents and modeling project. Class exercises are under the cheatsheet or in their respective files. 


## General useful commands
This includes some of the most common console commands to use cyclone/linux.

**Note, when anything is written between [], do not include [] in the command line.**

Connecting to cyclone
```
ssh [uib username]@cyclone2.gfi.uib.no
```

copy file from local to cyclone
```
scp “[file path]" [uib username]@cyclone2.gfi.uib.no:~/geof348/[target dir]
``` 
copy multiple files from local to cyclone
```
scp -r “[dir]" [uib username]@cyclone2.gfi.uib.no:~/geof348/[target dir]
```

Copy single file within cyclone
```
cp [path] [target path] 
``` 

Copy all files in a directory to another cyclone directory
```
cp -a [dir]/. [target dir] 		
```


launch jupyter 
```
conda activate dynpie3
tmux new python 
jupyter-lab --no-browser --ip='cyclone2.gfi.uib.no' --port 8904
```

open a .sh or .csh file (from working directory where the file is)
```
vi [filename]
```

run a .sh or .csh file (from working directory where the file is)
```
./[filename]
```

If you get 'permission denied' when running files
```
chmod 744 *
```

convert greb output to netCDF4
```
cdo -f nc import_binary [filename.ctl] [filename.nc]
```






Folder with some cmip5 data 
```
cd /Data/gfi/scratch/geof348_term/shared_data/cmip5/${modelname}/${expname}/atmos/6hrPlev/r1i1p1/va
```

Check diff between two files
```
diff run.greb.decon_mean_climate.csh run.greb.decon_mean_climate_modwinds.csh
```



dummy line
```
cp greb.mean.decon.exp-11111111111_rcp85_modwinds.nc ~/geof348/exercise3
```




## Exercise 0: Setting up Cyclone



## Exercise 1: GREB First steps



## Exercise 2: SSP Scenarios and experiments



## Exercise 3: Imposing different windfields



## Exercise 4: Anomalies and CMIP6






