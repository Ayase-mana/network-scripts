

### L2TP 服务自动安装脚本
- **功能**：一键部署L2TP/IPSec 服务
- **支持系统**：
  - CentOS 7+
  - Debian 9+
  - Ubuntu 18.04+
  - RHEL 7+
  - AlmaLinux 8+
  - Rocky Linux 8+
- **特性**：
  - 自动检测系统环境
  - 智能防火墙配置
  - 用户管理功能
  - 完整的卸载支持
  - 增强的安全配置

## 🚀 快速开始

### 安装L2TP 服务

1. 下载脚本：

```bash
# 国内：
wget https://gitcode.com/ayaya_mana/network-scripts/l2tp_install.sh

# 海外：
wget https://github.com/Ayase-mana/network-scripts/blob/main/l2tp_install.sh

chmod +x l2tp_install.sh
```


2. 运行安装：
```bash
./l2tp_install.sh
```

3. 按照提示完成配置：
   - 设置IP范围（默认：192.168.18.0/24）
   - 设置预共享密钥（PSK）
   - 创建VPN用户账号
   - 选择DNS服务器

### 连接VPN

使用以下信息连接您的VPN：
- **服务器IP**：脚本显示的服务器公网IP
- **预共享密钥**：安装时设置的PSK
- **用户名**：安装时设置的用户名
- **密码**：安装时设置的密码

## ⚠️ 重要提示

1. **防火墙设置**：确保防火墙已开放以下UDP端口：
   - 500
   - 4500
   - 1701

2. **系统要求**：
   - 最少512MB内存
   - 至少1GB可用磁盘空间
   - 支持TUN/TAP的VPS

3. **安全建议**：
   - 使用强密码
   - 定期更新PSK
   - 监控VPN访问日志

## 🔧 脚本管理功能

安装完成后，脚本提供以下管理功能：
- 添加/删除VPN用户
- 列出所有用户
- 显示连接信息
- 更新PSK
- 重启服务
- 查看服务状态
- 完全卸载服务

## 📝 更新日志

### v1.0 (优化版)
- 增强系统兼容性检测
- 改进防火墙自动配置
- 添加SELinux策略支持
- 优化错误处理和日志记录
- 完善卸载功能

## 👥 贡献者

- **原作者**：Teddysun
- **优化者**：ayuya_mana ([CSDN博客](https://blog.csdn.net/weixin_44149170))
