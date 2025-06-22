# VOYAGER AUTO BOT - 自动化任务机器人

一个专为与 Voyager 平台交互而设计的自动化任务机器人。该机器人帮助自动化每日任务完成和宝箱开启活动，以积累 Voyager 积分和奖励。

## 注册

- 链接：[Voyager Platform](https://voyager.preview.craft-world.gg/)

## 功能特性

- 自动化任务执行
- 自动开启每日宝箱
- 支持多个钱包
- 为高级用户提供代理支持
- 实时日志记录和状态更新
- 自动令牌刷新
- 24小时循环执行

## 安装

### 前置要求

- Node.js (v14 或更高版本)
- npm 或 yarn 包管理器

### 设置

1. 克隆仓库：

```bash
git clone https://github.com/jessdy/Voyager-Bot-Jad.git
cd Voyager-Bot-Jad
```

2. 安装依赖：

```bash
npm install
```

3. 创建 `pk.txt` 文件到项目根目录并添加您的私钥：

```
privateKey1
privateKey2
privateKey3
# 根据需要添加更多
```

4. （可选）如果您想使用代理，创建一个 `proxies.txt` 文件并每行添加一个代理：

```
socks5://username:password@host:port
http://username:password@host:port
# 根据需要添加更多
```

## 使用方法

启动机器人：

```bash
npm start
```

或

```bash
node voyager.js
```

### 控制说明

启动时会询问是否使用代理，输入 `y` 使用代理，`n` 直连。机器人会自动处理所有配置的账号，完成任务后等待24小时再次执行。

## 工作原理

1. 机器人使用以太坊签名对每个钱包进行身份验证
2. 自动获取并完成可用的日常任务
3. 自动开启每日宝箱获取奖励
4. 系统记录当前积分、任务状态和用户信息
5. 机器人会在需要时自动刷新令牌并跟踪每个钱包的状态

## 安全注意事项

- 永远不要分享您的 `pk.txt` 文件或私钥
- 此机器人在本地运行，不会将您的私钥发送到任何外部服务器
- 所有签名都使用 ethers.js 库在本地创建

## 故障排除

如果您遇到任何问题：

1. 确保您的私钥格式正确
2. 检查您的代理（如果使用）是否正常工作
3. 确保您有稳定的互联网连接
4. 查看控制台输出以获取详细的错误信息

## 免责声明

此机器人仅供教育目的提供。使用风险自负。开发者不对使用此软件可能产生的任何潜在风险（包括但不限于经济损失）承担责任。

## 捐赠支持

如果您觉得这个项目对您有帮助，可以通过以下地址进行捐赠支持项目开发：

- **EVM (以太坊/BSC/Polygon等)**: `0xD6611773079e022B4E403a5DF8152Cda9fA9B11f` 或 `jessdy.eth`
- **Solana**: `EEG8sYSWaU7S9c1NPKvkzWXZbfutvoRaR7sNtqrA22ru`
- **Bitcoin**: `bc1pv5xfcrvqadltd9vj83k7lshtz9vj4caj2uldj8d87e6f4c4p5unqh9um6q`

您的支持是我们持续改进和维护项目的动力！🙏