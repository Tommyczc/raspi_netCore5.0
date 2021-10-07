# raspi_netCore5.0
1) wget https://download.visualstudio.microsoft.com/download/pr/ce3cef63-ade6-4209-80f0-ac2815c5b282/e4a8b52aacf74d2a7d6d1cf5b9dca438/dotnet-sdk-5.0.401-linux-arm.tar.gz
2) wget https://download.visualstudio.microsoft.com/download/pr/e9d4b012-a877-443c-8344-72ef910c86dd/b5e729b532d7b3b5488c97764bd0fb8e/aspnetcore-runtime-3.0.0-linux-arm.tar.gz
3) mkdir dotnet-arm32
4) tar zxf aspnetcore-runtime-3.0.0-linux-arm.tar.gz -C $HOME/dotnet
5) tar zxf dotnet-sdk-5.0.401-linux-arm.tar.gz -C $HOME/dotnet
6) export DOTNET_ROOT=$HOME/dotnet-arm32
7) export PATH=$PATH:$HOME/dotnet-arm32
8) sudo nano /etc/profile 并且在最后加上 
9#set net core sdk and runtime path
export DOTNET_ROOT=/etc/dotnet-arm32
export PATH=$PATH:/etc/dotnet_arm32
这样就能开机自启了







