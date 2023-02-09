# 1

Removed divides from collision()

Before:

```
Reynolds number:		9.751927375793E+00
Elapsed Init time:			0.001335 (s)
Elapsed Compute time:			33.191956 (s)
Elapsed Collate time:			0.000001 (s)
Elapsed Total time:			33.193292 (s)
Flat profile:

Each sample counts as 0.01 seconds.
  %   cumulative   self              self     total           
 time   seconds   seconds    calls  Ts/call  Ts/call  name    
 69.55     22.56    22.56                             collision
 15.61     27.63     5.06                             propagate
 14.90     32.46     4.83                             av_velocity
```

After:

```
Reynolds number:		9.757317543030E+00
Elapsed Init time:			0.001019 (s)
Elapsed Compute time:			29.806672 (s)
Elapsed Collate time:			0.000000 (s)
Elapsed Total time:			29.807691 (s)
Flat profile:

Each sample counts as 0.01 seconds.
  %   cumulative   self              self     total           
 time   seconds   seconds    calls  Ts/call  Ts/call  name    
 65.59     19.16    19.16                             collision
 17.78     24.35     5.19                             propagate
 16.72     29.24     4.88                             av_velocity
```