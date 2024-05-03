# Comparing `tmp/RPICommLink-1.0.2.tar.gz` & `tmp/RPICommLink-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPICommLink-1.0.2.tar", last modified: Thu May  2 08:43:47 2024, max compression
+gzip compressed data, was "RPICommLink-1.0.3.tar", last modified: Fri May  3 20:19:42 2024, max compression
```

## Comparing `RPICommLink-1.0.2.tar` & `RPICommLink-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 08:43:47.506676 RPICommLink-1.0.2/
--rw-rw-rw-   0        0        0      159 2024-05-02 08:43:47.505679 RPICommLink-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 08:43:47.501690 RPICommLink-1.0.2/RPICommLink/
--rw-rw-rw-   0        0        0    14854 2024-05-02 08:43:36.000000 RPICommLink-1.0.2/RPICommLink/rpicommlink.py
-drwxrwxrwx   0        0        0        0 2024-05-02 08:43:47.505679 RPICommLink-1.0.2/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0      159 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 08:43:47.506676 RPICommLink-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      270 2024-05-02 08:26:32.000000 RPICommLink-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 20:19:42.909289 RPICommLink-1.0.3/RPICommLink/
+-rw-rw-rw-   0        0        0    15143 2024-05-03 20:16:24.000000 RPICommLink-1.0.3/RPICommLink/rpicommlink.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     1088 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2024-05-03 20:17:21.000000 RPICommLink-1.0.3/setup.py
```

### Comparing `RPICommLink-1.0.2/RPICommLink/rpicommlink.py` & `RPICommLink-1.0.3/RPICommLink/rpicommlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.data_event.clear()
         self.rpi_port = rpi_port
         self.password = password
         self.target_name = []
         self.connect_device = []
         self.send_server_socket = None
 
-    def open(self, device_name: str = None, max_connect: int = 0, ip: str = None):
+    def open(self, device_name: str = 'default', max_connect: int = 0, ip: str = None):
         """打开_server线程的函数
 
         它使用线程来启动服务器是为了实现非阻塞式的服务器启动。如果直接调用 _server 方法而不使用线程，
         那么在服务器启动过程中，主程序会被阻塞，直到服务器关闭或者达到最大连接数为止。
 
         通过在新的线程中启动服务器，主程序可以继续执行后续的操作，而不必等待服务器启动完成。
         当服务器启动后，它会在后台处理连接请求，而主程序可以继续执行其他任务，
@@ -53,15 +53,15 @@
         它负责创建一个 TCP 套接字，绑定到本机的 IP 地址和指定的端口号，然后在一个无限循环中等待客户端的连接请求。
         当有新的客户端连接时，检查连接数是否已达到最大限制 max_connect。达到最大限制发送给请求连接的客户端‘full’表示已达到最大限制，
 
         未达到最大限制 max_connect时，客户端有100ms的时间来请求加入服务器，请求通过后，将超时时间设置为无，
         并加入当前连接的套接字列表 self.socket_list，同时发送给客户端该设备名字 device_name
         """
         if ip is None:
-            host_ip = socket.gethostbyname(socket.gethostname())
+            host_ip = get_host_ip()
         else:
             host_ip = ip
 
         try:
             server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             host_address = (host_ip, self.rpi_port)
             server_socket.bind(host_address)
@@ -229,30 +229,30 @@
                         self.send_server_socket = sock
                     elif state == 'ny6cz4ln':
                         print(f'\033[91mError:已达到服务器的设备连接上限 \033[0m')
             return
         except Exception:
             return None
 
-    def connect(self, target_name, subnet_ip: str = None):
+    def connect(self, target_name: str= 'default', subnet_ip: str = None):
         """连接到服务器并尝试与指定设备建立连接的函数。
 
         如果无法构建局域网，请自行修改。
 
         获取本地主机的 IP 地址并构建局域网的子网。
         用线程遍历子网中的所有可能 IP 地址，并尝试连接到每个 IP 地址的指定端口。
         在连接成功时，发送密码给服务器端，并接收服务器返回的设备名称和状态。
         打印扫描到的设备名称。
         根据连接状态输出相应的信息。
 
-        :param subnet_ip:子网，IP地址的前三个数，格式为str’xxx.xxx.xx‘
+        :param subnet_ip:子网，IP地址前三个数，格式为str’xxx.xxx.xx‘
         :param target_name: 指定的设备名字
         """
         if subnet_ip is None:
-            local_ip = socket.gethostbyname(socket.gethostname())  # 获取本地主机的IP地址
+            local_ip = get_host_ip()  # 获取本地主机的IP地址
             subnet = '.'.join(local_ip.split('.')[:-1])  # 获取局域网子网
         else:
             subnet = subnet_ip
         port = self.rpi_port  # 要扫描的端口号
         threads = []
         for i in range(1, 255):
             ip = f"{subnet}.{i}"
@@ -283,10 +283,23 @@
         :param msg:发送的信息
         """
         try:
             self.send_server_socket.send(msg.encode('utf-8'))
         except Exception:
             print('\033[91mError:发送失败！请确认是否有连接服务器 \033[0m')
 
+def get_host_ip():
+    """
+    查询本机IP地址
+    :return:本机IP地址
+    """
+    try:
+        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        sock.connect(('8.8.8.8', 80))
+        ip = sock.getsockname()[0]
+        sock.close()
+        return ip
+    except Exception as e:
+        print(e)
 
 if __name__ == "__main__":
     pass
```

