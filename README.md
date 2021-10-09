# IMUData
  此程序用来采集安卓手机中的IMU数据，主要包括磁力计，陀螺仪，加速度计三种，启动后每隔一分中保存一次。（文件会保存在根目录IMUData/data下，如果没有自动生成需要手动创建）
  为了保证service能够长时间执行：
  + 1.增加了监听用户锁屏。
  + 2.当锁屏时打开前台广播，解锁时打开后台广播。<br />
  注：因为使用了Notification，当创建通知时，由Oreo中引入的自适应图标可能会引起崩溃。可参考文章https://www.jianshu.com/p/06e04ac55db3
  
![image](https://user-images.githubusercontent.com/34254925/136639361-d4fba75c-ffc3-4ad7-be61-34d46a008b61.png)
![image](https://user-images.githubusercontent.com/34254925/136639385-cb464dad-bd2d-43bd-a34d-82a56e817e20.png)
