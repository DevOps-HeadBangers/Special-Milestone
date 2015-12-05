Special Milestone - Flame Monkey
============================


For the Special Milestone we built **Flame Monkey**

It generates flame graphs to help visualize long chains of test method calls.

We used the same Target App that was used in Milestone 3. 
Two test files for file upload **test1.js** (containing multiple test functions ) and **test2.js** were used.

>**Login to root**

> ssh root @ XXX.XXX.XXX.XXX

Once the droplet is up, the next step is to check whether the port is available

> ps -aux | grep "node"

If in case anything is running use **kill** (followed by port number) to end it.

>**To run the first test case**

> node --perf-basic-prof test2.js

Once this completes, it will show the number of test cases that ran followed by number of cases that were successful. 

Wait for 30-40s.

>**Run server.js**

> nodejs server.js

Once the server spins up , open browser and check for the server by typing 
XXX.XXX.XXX.XXX:(port no.)

In our case the port number was 3000 and root address was 104.131.193.51

Next download the flame graph for this test case by going to the address 
> XXX.XXX.XXX.XXX:(port no.)/test2

Repeat the same process by running test1.js.

The flamegraph will be available at :
> XXX.XXX.XXX.XXX:(port no.)/test1

All the test case commands are included in **runSpecial.sh**

It can be run by
> sh runSpecial.sh

**Note** : Once you have logged into the the root and in your repo make sure to do a 

> nvm use v0.12.7

Since it needs the latest version of node to run the **perf** command.

----------

The screencast for the special milestone: [Special Milestone](https://youtu.be/IkMs9yg_56s)
