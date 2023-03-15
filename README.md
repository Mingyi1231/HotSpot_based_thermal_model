# HotSpot based thermal model (DistributedThermalModel)
The characterization have done for compute chiplet and interposer temperature, the result are in the "outputs" directory,  or you can run char_thermal_r.py file for another characterization which will take some time, all config files are in "configs" directory named by *.cfg, you can also add some config example in this directory.<br/> 

Run char_thermal_r.py by:<br/>
python3 char_thermal_r.py configs/case1.cfg<br/>

Then we can compute the gird temperature, compute_temp_grid.py is normal serial calculation of interpolation results, compute_temp_parallel.py is Improved parallel computation interpolation results, The running time is reduced by about half. 
<br/>
Compute temperature by:<br/>
python3 compute_temp_grid.py configs/case1.cfg<br/>
python3 compute_temp_parallel.py configs/case1.cfg<br/>
