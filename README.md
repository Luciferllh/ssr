# ssr( support ipv6)
## 使用方法<br>
### 1.系统选择<br>
  centos6 / debian9(推荐）<br>
  debian9：自带bbr加速<br>
  centos6：centos7防火墙配置比较麻烦，没有bbr加速需要手动安装<br>
#### 2.下载并赋予可执行权限<br>
  <code>sudo -i</code><br>
  <code>wget https://raw.githubusercontent.com/Luciferllh/ssr/master/shadowsocksR.sh && chmod +x shadowsocksR.sh</code> <br>
#### 3.安装<br>
  <code>./shadowsocksR.sh</code><br>
#### 4.查看和修改配置信息<br>
  查看<code>cat /etc/shadowsocks.json</code><br>
  修改(需要vi编辑器知识)<code>vi /etc/shadowsocks.json</code><br> 
 
## 安装bbr 
<code>sudo -i</code><br>
<code>wget -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/YankeeBBR/master/bbr.sh && bash bbr.sh install</code><br>

## centos7防火墙关闭方法
<code>iptables -F</code><br>
<code>systemctl stop firewalld</code><br>
<code>systemctl disable firewalld</code><br>
<code>vim /etc/selinux/config</code>修改SELINUX=disabled<br>
<img src='https://img2018.cnblogs.com/blog/1510548/201903/1510548-20190329032810766-849768581.png' height='200px' width='600px'></img>
<code>reboot</code><br>
