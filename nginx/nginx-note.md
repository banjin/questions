1. nginx 常用名令

	(1).查看nginx进程 
		
		ps -ef|grep nginx
		nginx的进程有主进程和工作进程组成
	(2).启动nginx进程 
		
		nginx
	
	(3).平滑启动nginx进程 
		
		kill -HUP `cat /var/run/nginx.pid` 
		或者 
		nginx -s reload
		平滑启动的意思是在不停止nginx的情况下，重启nginx，重新加载配置文件，启动新的工作线程，完美停止旧的工作线程。

 （4）强制停止nginx 
		
		pkill -9 nginx
  (5) 检查对nginx.conf文件的修改是否正确 
  	
  		nginx -t -c /etc/nginx/nginx.conf 或者 nginx -t
  		
   (6) 停止nginx的命令 
   		
   		nginx -s stop
   	(7) 查看nginx的版本信息
   	    
   	    nginx -v
   	(8)  查看完整的nginx的配置信息 
   		
   		nginx -V
   	(9)  查看nignx帮助信息
   	
   		nginx -h
   
   
		
	