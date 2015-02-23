Welcome to the log4z wiki!  
# Introduction:    

Log4z is an open source C++ lightweight & cross platform log library.   
It provides in a C++ application log and trace debug function for 7*24h service program.  
Support 64/32 of debian, redhat, centos, suse, windows.   

I changed this API using VC++ style.


# Feature:  
    
1. MIT open source license,very liberal.  
   
2. Cross Platform Linux & Windows, Lightweight  only one cpp sourse file one header file.  
     
3. Multi-Logger Output, Rolling File, Priority Filter, Thread Safe.  
     
4. Screen Display Log with Different Color.  
   
5. Support format-style and stream-style write log.  
   
6. Support configure from file and hot update, or can direct fast work without any config.  
   

# The  Log File  
The output log file through a configuration file or when the program starts a flexible configuration   

### File Name Format:   
LogName_YearMonthDayHourMinute_ProcessID_BlockNumber.log    

***   
E:\GITHUB\LOG4Z\PROJECT\BIN  
│──advanced_test.exe  
│──config.cfg  
│──fast_test.exe  
│──stress_test.exe  
│  
├─AdvacedLog  
│──│───FileConfig_2013100921_003852_000.log  
│──│───FileConfig_2013101313_005920_000.log  
│  
├─log  
│──│──advanced_test_2013100921_003852_000.log  
│──│──advanced_test_2013101313_005920_000.log    
│──│──fast_test_2013100921_003855_000.log  
│──│──fast_test_2013101313_006160_000.log  
│──│──stress_test_2013101313_007196_000.log  
│──│  
│──└─2013_10  
│─────│────Dynamic_2013100921_003852_000.log  
│─────│────Dynamic_2013101313_005920_000.log  
│  
└─Stress  
───│────NetWork_2013101313_007196_000.log  
───│────NetWork_2013101313_007196_001.log  
───│────NetWork_2013101313_007196_002.log  
───│────NetWork_2013101313_007196_003.log  
───│────NetWork_2013101313_007196_004.log  
***  
### 日志内容[Log Content]  
![fast_output_linux.png](https://raw.github.com/zsummer/wiki-pic/master/log4z/fast_output_linux.png)  
![fast_output_windows.png](https://raw.github.com/zsummer/wiki-pic/master/log4z/fast_output_windows.png)  

# How To Use Log4z  
![hellow_world.png](https://raw.github.com/zsummer/wiki-pic/master/log4z/hellow_world.png)  

# How to compile  
### Directly Using The Way 直接使用:    
Add files log4z.cpp log4z.h and compile together in the existing projects  
把文件 log4z.cpp log4z.h添加到已有项目中并一起编译.  
### Make Library To Use   
**In Windows:**  
`Open and compile log4z/vc2005/log4z.vcproj`  
**In Linux :**   
`cd log4z/g++`   
`cmake .`   
`make`   

#About The Author  
Original Author: YaweiZhang  
└-- Revised by : SunMi Kang

GitHub: https://github.com/zsummer  
