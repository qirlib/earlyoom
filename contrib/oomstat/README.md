# oomstat

oomstat is a very simple tool that prints available
memory, free swap and memory pressure (PSI) information
every 100ms.

Example output with `tail -f /dev/zero` started in the
background is pasted below, more examples are available
in the text files in this directory.


```
$ ./oomstat

     | /proc/meminfo     | /proc/pressure/memory
Time | MemAvail SwapFree | some avg10 full avg10
   s |      MiB      MiB |    %     %    %     %
     -                   -                      
 0.0 |    17596        0 |    0     0    0     0
 0.1 |    17349        0 |    0     0    0     0
 0.2 |    17099        0 |    0     0    0     0
 0.3 |    16847        0 |    0     0    0     0
 0.4 |    16595        0 |    0     0    0     0
 0.5 |    16346        0 |    0     0    0     0
 0.6 |    16105        0 |    0     0    0     0
 0.7 |    15855        0 |    0     0    0     0
 0.8 |    15604        0 |    0     0    0     0
 0.9 |    15353        0 |    0     0    0     0
 1.0 |    15102        0 |    0     0    0     0
 1.1 |    14851        0 |    0     0    0     0
 1.2 |    14601        0 |    0     0    0     0
 1.3 |    14351        0 |    0     0    0     0
 1.4 |    14100        0 |    0     0    0     0
 1.5 |    13850        0 |    0     0    0     0
 1.6 |    13619        0 |    0     0    0     0
 1.7 |    13370        0 |    0     0    0     0
 1.8 |    13123        0 |    0     0    0     0
 1.9 |    12872        0 |    0     0    0     0
 2.0 |    12621        0 |    0     0    0     0
 2.1 |    12370        0 |    0     0    0     0
 2.2 |    12121        0 |    0     0    0     0
 2.3 |    11871        0 |    0     0    0     0
 2.4 |    11622        0 |    0     0    0     0
 2.5 |    11373        0 |    0     0    0     0
 2.6 |    11122        0 |    0     0    0     0
 2.7 |    10872        0 |    0     0    0     0
 2.8 |    10621        0 |    0     0    0     0
 2.9 |    10369        0 |    0     0    0     0
 3.0 |    10121        0 |    0     0    0     0
 3.1 |     9871        0 |    0     0    0     0
 3.2 |     9620        0 |    0     0    0     0
 3.3 |     9369        0 |    0     0    0     0
 3.4 |     9121        0 |    0     0    0     0
 3.5 |     8873        0 |    0     0    0     0
 3.6 |     8625        0 |    0     0    0     0
 3.7 |     8374        0 |    0     0    0     0
 3.8 |     8124        0 |    0     0    0     0
 3.9 |     7872        0 |    0     0    0     0
 4.0 |     7621        0 |    0     0    0     0
 4.1 |     7371        0 |    0     0    0     0
 4.2 |     7123        0 |    0     0    0     0
 4.3 |     6884        0 |    0     0    0     0
 4.4 |     6646        0 |    0     0    0     0
 4.5 |     6409        0 |    0     0    0     0
 4.6 |     6171        0 |    0     0    0     0
 4.7 |     5933        0 |    0     0    0     0
 4.8 |     5696        0 |    0     0    0     0
 4.9 |     5461        0 |    0     0    0     0
 5.0 |     5222        0 |    0     0    0     0
 5.1 |     4984        0 |    0     0    0     0
 5.2 |     4748        0 |    0     0    0     0
 5.3 |     4510        0 |    0     0    0     0
 5.4 |     4275        0 |    0     0    0     0
 5.5 |     4038        0 |    0     0    0     0
 5.6 |     3788        0 |    1     0    1     0
 5.7 |     3565        0 |   28     0   15     0
 5.8 |     3334        0 |   25     0   21     0
 5.9 |     3100        0 |   24     0   20     0
 6.0 |     2807        0 |   32     0   25     0
 6.1 |     2574        0 |   39     1   30     0
 6.2 |     2404        0 |   29     1   26     0
 6.3 |     2191        0 |    1     1    0     0
 6.4 |     1875        0 |   12     1    8     0
 6.5 |     1724        0 |   59     1   51     0
 6.6 |     1550        0 |   39     1   31     0
 6.7 |     1344        0 |   30     1   27     0
 6.8 |     1181        0 |   10     1    7     0
 6.9 |      945        0 |   31     1   22     0
 7.0 |      773        0 |   58     1   51     0
 7.1 |      599        0 |   46     1   39     0
 7.2 |      360        0 |   37     1   30     0
 7.3 |      268        0 |   60     1   50     0
 7.4 |      149        0 |   45     1   34     0
 7.5 |       86        0 |   47     1   40     0
 7.6 |        8        0 |   54     1   36     0
 7.7 |        0        0 |   94     1   54     0
 7.8 |        0        0 |  107     1   94     0
 7.9 |      107        0 |  109     1   53     0
 8.1 |     4801        0 |   52     1   36     0
 8.2 |    10339        0 |    8     9    3     6
 8.3 |    15634        0 |    0     9    0     6
 8.4 |    19168        0 |    0     9    0     6
 8.5 |    20197        0 |    0     9    0     6
 8.6 |    20194        0 |    0     9    0     6
 8.7 |    20193        0 |    0     9    0     6
 8.8 |    20193        0 |    0     9    0     6
 8.9 |    20193        0 |    0     9    0     6
 9.0 |    20193        0 |    0     9    0     6
 9.1 |    20193        0 |    0     9    0     6
 9.2 |    20192        0 |    0     9    0     6
 9.3 |    20192        0 |    0     9    0     6
 9.4 |    20192        0 |    0     9    0     6
 9.5 |    20192        0 |    0     9    0     6
 9.6 |    20180        0 |    0     9    0     6
 9.7 |    20180        0 |    0     9    0     6
 9.8 |    20180        0 |    0     9    0     6
 9.9 |    20169        0 |    0     9    0     6
10.0 |    20169        0 |    0     9    0     6
```