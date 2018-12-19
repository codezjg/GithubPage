---
title: Unity 网络状态判断
date: 2018-10-11 11:58:10
tags: unity,网络
---

Unity 网络状态判断


```
//当网络不可用时 
//如果项目需要耗费的流量比较大，可以通过下面的方法判断，并提示用户
if (Application.internetReachability== NetworkReachability.NotReachable)             
{ 
       //Do sth.
}


//当用户使用WiFi时  
if(Application.internetReachability==NetworkReachability.ReachableViaLocalAreaNetwork)               
{ 
     //Do sth. 
}                 


//当用户使用移动网络时
if(Application.internetReachability==NetworkReachability.ReachableViaCarrierDataNetwork)             
{
      //Do sth.               
}
```