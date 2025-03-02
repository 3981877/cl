# cl
Mac主机+orbstack_docker_halo_frp_cloudflare_npm实现443证书访问
这个标题看起来有点长，要实现目标一样都少不了，我现在就用我的Mac Mini M4来做演示
### 1 安装配置homebrew 官方地址：https://brew.sh/zh-cn/
### 2 安装orbstack和配置docker环境 官方地址：https://orbstack.dev
### 3 安装配置FRP Github官方地址：https://github.com/fatedier/frp
### 4 安装halo博客 官方地址：https://www.halo.run
### 5 安装NPM反代UI Github项目地址：https://github.com/xiaoxinpro/nginx-proxy-manager-zh

## 做好以上工作，接下来申请一个cloudflare API令牌 

创建令牌
<img width="1250" alt="截屏2025-03-02 10 45 00" src="https://github.com/user-attachments/assets/2df34297-210f-44e4-bee0-e152164eaef0" />
保存Key到本地备用

登陆NPM UI 创建证书 替换成自己刚刚申请的Key <img width="500" alt="截屏2025-03-02 10 51 21" src="https://github.com/user-attachments/assets/78758c41-255c-4d4b-bb28-23590eef5cfc" />

最后添加反代就可以实现本443证书访问
