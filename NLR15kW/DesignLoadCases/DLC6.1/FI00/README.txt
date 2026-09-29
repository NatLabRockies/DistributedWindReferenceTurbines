For DLC1.1:
I had to use truncate.py to clip files before shutdowns. Then in MExtremes and Mlife I selected the truncated versions of the files, not the original ones.
However, for LoadExtrap I select the original ones. That's why i changethe suffix to .outxxx before running LoadExtrap to the clipped ones.


DLC6.1:
Here the runs require smaller time steps for the yaw fault cases. 
dT=0.001s for most runs, except:

+-90 through +-135: for these I need
>> dT=0.0005s ===> set in the .fst template file. 
>> use UA_Mod=0 for these
>> use Create_DLC6.1FI00_FS_reduced.py for this subset of runs. Also set dT 
>> use local spd_trq.dat which is symmetric about 0. !!
