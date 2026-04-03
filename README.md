# ML_CH_weather_reconstruction

## Ensemble Description

The ensemble of 40 netcdf files can be divided into 4 subgroups with 2 different input data and 5 members each.

Each subgroup has a sligthly different way to calculate the loss functions.

Each subgroup has 5 members, which represents 5 different trainings with slightly different initial weighting.

Each reconstruction withrr0 uses all available data, which is temperature, pressure, pressure tendency (t0 - t-1), weather type and binary wet days (and a few static information).
Reconstruction norr0 is removing the binary wet day information in the training. 

In all reconstructions the 1st of January is missing due to missing pressure tendency information

