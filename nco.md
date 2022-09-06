Before reading your netCDF into Vapor, you'll need to do a bit of post-processing. This is because netCDF has a nasty habit of flipping your x and z axes
in a way that is not straightforward to fix beforehand. To remedy this, you'll need a package called NCO.

To install NCO with conda:

```
conda update --all
conda install -c conda-forge nco
```

Then, write a simple bash script along the lines of:

```
fname='YOUR_FILE.nc'
start_time=$(date +%s)
ncpdq -a z,x $fname -O $fname 
end_time=$(date +%s)
echo "done. time elapsed: $(($end_time - $start_time))"
```

This script will use a NCO command called ncpdq to transpose the x and z axes back to where they should be. If you use your filename as the input and output, the file will be overwritten with the correct axes. 
