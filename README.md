# onekeyos-restore
One Key VPS (KVM only) OS reload (Ubuntu,CentOS,Debian)


USAGE:

    bash InstallNET.sh      -d/--debian [dist-name]
                            -u/--ubuntu [dist-name]
                            -c/--centos [dist-version]
                            -v/--ver [32/i386|64/amd64]
                            --ip-addr/--ip-gate/--ip-mask
                            -apt/-yum/--mirror
                            -dd/--image
                            -a/-m

# dist-name：发行版本代号
# dist-version：发行版本号
# -apt/-yum/--mirror：使用定义镜像
# -a/-m：询问是否能进入VNC自行操作。-a 为不提示(一般用于全自动安装)，-m 为提示。

Default Password: MoeClub.org

#使用默认镜像全自动安装 Debian 8 x64
bash InstallNET.sh -d 8 -v 64 -a

#使用自定义镜像全自动安装 CentOS 6.9 x64
bash InstallNET.sh -c 6.9 -v 64 -a --mirror 'http://mirror.centos.org/centos'
