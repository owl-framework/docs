Benchmarks
==========

```
ab -c 40 -n 15000 http://owl.ab.dmtry.me/users
This is ApacheBench, Version 2.3 <$Revision: 1638069 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking owl.ab.dmtry.me (be patient)
Completed 1500 requests
Completed 3000 requests
Completed 4500 requests
Completed 6000 requests
Completed 7500 requests
Completed 9000 requests
Completed 10500 requests
Completed 12000 requests
Completed 13500 requests
Completed 15000 requests
Finished 15000 requests


Server Software:        nginx
Server Hostname:        owl.ab.dmtry.me
Server Port:            80

Document Path:          /users
Document Length:        779 bytes

Concurrency Level:      40
Time taken for tests:   0.922 seconds
Complete requests:      15000
Failed requests:        0
Total transferred:      13980000 bytes
HTML transferred:       11685000 bytes
Requests per second:    16273.45 [#/sec] (mean)
Time per request:       2.458 [ms] (mean)
Time per request:       0.061 [ms] (mean, across all concurrent requests)
Transfer rate:          14811.38 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.1      0       2
Processing:     0    2   2.1      2     101
Waiting:        0    2   2.1      2     101
Total:          1    2   2.1      2     101

Percentage of the requests served within a certain time (ms)
  50%      2
  66%      2
  75%      3
  80%      3
  90%      3
  95%      4
  98%      6
  99%      9
 100%    101 (longest request)
```

```
ab -c 20 -n 15000 http://owl.ab.dmtry.me/users
This is ApacheBench, Version 2.3 <$Revision: 1638069 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking owl.ab.dmtry.me (be patient)
Completed 1500 requests
Completed 3000 requests
Completed 4500 requests
Completed 6000 requests
Completed 7500 requests
Completed 9000 requests
Completed 10500 requests
Completed 12000 requests
Completed 13500 requests
Completed 15000 requests
Finished 15000 requests


Server Software:        nginx
Server Hostname:        owl.ab.dmtry.me
Server Port:            80

Document Path:          /users
Document Length:        779 bytes

Concurrency Level:      20
Time taken for tests:   0.957 seconds
Complete requests:      15000
Failed requests:        0
Total transferred:      13980000 bytes
HTML transferred:       11685000 bytes
Requests per second:    15679.60 [#/sec] (mean)
Time per request:       1.276 [ms] (mean)
Time per request:       0.064 [ms] (mean, across all concurrent requests)
Transfer rate:          14270.89 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    0   0.0      0       0
Processing:     0    1   1.0      1      21
Waiting:        0    1   1.0      1      21
Total:          0    1   1.0      1      21

Percentage of the requests served within a certain time (ms)
  50%      1
  66%      1
  75%      1
  80%      2
  90%      2
  95%      3
  98%      4
  99%      5
 100%     21 (longest request)
```

```
ab -c 300 -n 25000 http://owl.ab.dmtry.me/users
This is ApacheBench, Version 2.3 <$Revision: 1638069 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking owl.ab.dmtry.me (be patient)
Completed 2500 requests
Completed 5000 requests
Completed 7500 requests
Completed 10000 requests
Completed 12500 requests
Completed 15000 requests
Completed 17500 requests
Completed 20000 requests
Completed 22500 requests
Completed 25000 requests
Finished 25000 requests


Server Software:        nginx
Server Hostname:        owl.ab.dmtry.me
Server Port:            80

Document Path:          /users
Document Length:        779 bytes

Concurrency Level:      300
Time taken for tests:   1.305 seconds
Complete requests:      25000
Failed requests:        4698
   (Connect: 0, Receive: 0, Length: 4698, Exceptions: 0)
Non-2xx responses:      4698
Total transferred:      20382542 bytes
HTML transferred:       16595126 bytes
Requests per second:    19163.42 [#/sec] (mean)
Time per request:       15.655 [ms] (mean)
Time per request:       0.052 [ms] (mean, across all concurrent requests)
Transfer rate:          15257.78 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    7  81.4      0    1002
Processing:     0    8   4.7      7     212
Waiting:        0    8   4.7      7     212
Total:          1   15  81.5      7    1024

Percentage of the requests served within a certain time (ms)
  50%      7
  66%      8
  75%      9
  80%     11
  90%     15
  95%     17
  98%     20
  99%     23
```
