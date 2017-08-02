# Performance Analysis

### Recommend using Python in Anaconda for better performance.

## Information

name        |value
------------|-----------
Training Set|MNIST 42000 28x28 gray
Batch Size  |100
Iterations  |2000
forward_times|2601
backward_times|2001
CPU			|i7-4790 CPU @ 3.60GHz

### Python3 in Anaconda

Accuracy: 0.991667

Iter: 2000, Cost: 0.007383

name	|forward_time	|backward_time	|forward_mean	|backward_mean	
--------|---------------|---------------|---------------|---------------
Data	|0.073538	|0.024317	|0.000028	|0.000012
Conv1	|50.427243	|82.105529	|0.019388	|0.041032
pool1	|95.274342	|10.921718	|0.036630	|0.005458
Conv2	|71.583208	|118.194660	|0.027521	|0.059068
pool2	|14.343701	|2.975322	|0.005515	|0.001487
fc3	|9.543055	|15.118490	|0.003669	|0.007555
relu3	|1.383795	|1.082115	|0.000532	|0.000541
pred	|5.047948	|6.669519	|0.001941	|0.003333
loss	|0.458279	|0.177457	|0.000176	|0.000089

### Native Python3

Accuracy: 0.991667

Iter: 2000, Cost: 0.007383

name	|forward_time	|backward_time	|forward_mean	|backward_mean	
--------|---------------|---------------|---------------|---------------
Data	|0.039973	|0.019009	|0.000015	|0.000009
Conv1	|76.094196	|114.764927	|0.029256	|0.057354
pool1	|72.345203	|10.924688	|0.027814	|0.005460
Conv2	|370.081568	|476.961305	|0.142284	|0.238361
pool2	|9.614037	|2.431894	|0.003696	|0.001215
fc3	|83.233347	|85.736211	|0.032001	|0.042847
relu3	|0.765435	|0.561773	|0.000294	|0.000281
pred	|1.098624	|1.267450	|0.000422	|0.000633
loss	|0.276948	|0.102970	|0.000106	|0.000051

### Native Python2

Accuracy: 0.991667

Iter: 2000, Cost: 0.007383

name	|forward_time	|backward_time	|forward_mean	|backward_mean	
--------|---------------|---------------|---------------|---------------
Data	|0.039304	|0.018812	|0.000015	|0.000009
Conv1	|77.984102	|117.541489	|0.029982	|0.058741
pool1	|73.096253	|11.021775	|0.028103	|0.005508
Conv2	|373.498943	|489.150597	|0.143598	|0.244453
pool2	|10.090908	|2.586956	|0.003880	|0.001293
fc3	|83.812420	|86.976251	|0.032223	|0.043466
relu3	|0.766895	|0.567209	|0.000295	|0.000283
pred	|1.100621	|1.267404	|0.000423	|0.000633
loss	|0.278426	|0.091963	|0.000107	|0.000046