   $ wget https://mirrors.tuna.tsinghua.edu.cn/apache/rocketmq/4.7.1/rocketmq-all-4.7.1-bin-release.zip
   
   99  cd /usr/local/
   
  102  sudo mkdir rocketmq
  
  103  sudo apt install git
  
  104  cd rocketmq/
  
  105  git clone https://github.com/apache/rocketmq-externals.git

 217  java -jar target/rocketmq-console-ng-1.0.1.jar --rocketmq.config.namesrvAddr='192.168.1.10:9876'
    
    
 240  nohup  bin/mqnamesrv &
      
 241  nohup bin/mqbroker -n localhost:9876 &
