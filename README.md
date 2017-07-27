# libsodium最新版本安装教程
yum -y groupinstall "Development Tools"  
wget https://download.libsodium.org/libsodium/releases/LATEST.tar.gz   
tar zxf LATEST.tar.gz  
cd libsodium*  
./configure && make && make install  

# 关联修复  
echo /usr/local/lib > /etc/ld.so.conf.d/usr_local_lib.conf  
ldconfig  
