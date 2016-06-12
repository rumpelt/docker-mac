# Docker on Mac
Follow following steps on MAC to use docer
1. On mac, you need to create Linux virtual box image. This is required becuase docker server/daemon run on linux kernel only. Use the followin command to create this
 
  $ docker-machine create --driver virtualbox ashwanir

You might need to disable VPN (If your machine is behind VPN)

2. Get the docker machine environment variable, with following command
   $ docker-machine env ashwanir

3. You need to set these environment variables so as to correctly configure your docker daemon
   $ eval "$(docker-machine env ashwanir)"

4. Test docker with following command
   $  docker run hello-world
 You shoul see hello world message
