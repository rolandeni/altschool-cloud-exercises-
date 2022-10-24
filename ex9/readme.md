# Task 9

### Using the below IP address
+ ### What is the network IP ?
+ ### What is the number of Host ?
+ ### what is the range of IP addresses ?
+ ### what is the Broadcast IP ?
##      **193.16.20.35 / 29**

# Solution
1. The **Network IP** is = 193.16.20.35
2. To find number of Host we need the netmask
   
   *193.16.20.35 / 29*

    *32-29 = 3* 

3 bits are available in the network ip which is represented by 0s

| 11111111. |11111111.| 11111111.| 11111000 |
| --- | --- | --- | --- |
| 255 | 255 | 255 | 248 |
| 193 | 16 | 20 | 35 |

 

convert the last block of 8bits to decimal
 *11111000 = 248*

+ Netmask = 255.255.255.248
+ Then we to find the wildcard

+ **255 -248 = 7**
wildcard = 0.0.0.7

## 3.  To find number of Host 
+ wildcard -1 = 6
+ Number of private host = **6**

## 4. To find broadcast IP
+ wildcard + Network 
+ 7 + 35 = 42
+ Broadcast IP is= **193.16.20.42**

## 5. To find the range of IP 
+ network ip +1 = 193.16.20.36
+ Host Min = 193.16.20.36
+ Host max = broadcast -1= 193.16.20.42 -1
+ Host max = 193.16.20.41
+ The range of IP is
+ *Host Min = 193.16.20.36* to *Host Max = 193.16.20.41*
