# Reg_tracking_studies

## Regional Tracking studies


### Comparing how tracking steps are scaling per step in regional tracking


![](https://codimd.web.cern.ch/uploads/upload_69d4a8430dd94aea71e03909ee2abee5.png)
![](https://codimd.web.cern.ch/uploads/upload_b40b3fbffade8c7fa39107328d5ba0c4.png)
![](https://codimd.web.cern.ch/uploads/upload_836a917073b9dedb27e4f161d745d6f6.png)
![](https://codimd.web.cern.ch/uploads/upload_d1438feb9ef3ed6f3b1a8ca0a2eff162.png)

### With fullscan as reference

![](https://codimd.web.cern.ch/uploads/upload_c831b6154e41f368d9c8eaba5f4fbd4c.png)
![](https://codimd.web.cern.ch/uploads/upload_ae7532d0a4436d49916fc5ca6ed6f117.png)
![](https://codimd.web.cern.ch/uploads/upload_0334b2b07e6646f3af3d01468a578ed0.png)
![](https://codimd.web.cern.ch/uploads/upload_fe330e826701288c1590e8c97e5e6f0c.png)



NOTES:
 - the time measurements here are not very accurrate but the analogy is still representative

### Comparing size of data between regional and full scan

![](https://codimd.web.cern.ch/uploads/upload_3ea8ad1534ec2964b76426bf5e5a06de.png)

### Comparing throughput see https://docs.google.com/spreadsheets/d/1HEPA8pKfdcYvoQpY3U4FQ5dq0dgCLFIV80692f3uEZI/edit?usp=sharing


<img width="904" height="214" alt="image" src="https://github.com/user-attachments/assets/55ad3650-1043-4d59-8689-66de1cfeb257" />



### Notes

- scaling:
    - in fullscan we see clustering and seeding have some linear trends when plotted (size, time) but these are much harder to distinguish in regional tracking
- time:
    - regional tracking seems to give a speedup of around 4.5 times
- throughput:
    - when examining the throughput of the kernels we see that we have 9.98 events/sec for fullscan and 925 events per sec for regional
- size:
    - for example for the same input(around 90 events) we have 5156 clusters and 9 tracks found for regional but 468619 clusters produced and 2537 tracks in fullscan
