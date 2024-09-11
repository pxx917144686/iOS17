# iOSRealRun-cli-17

## 用法简介

### 前置条件

1. 系统是 `Windows` 或 `MacOS`
2. iPhone 或 iPad 系统版本大于等于 17
3. Windows 需要安装 iTunes
4. 已安装 `Python3` 和 `pip3`
5. **重要**: 只能有一台 iPhone 或 iPad 连接到电脑，否则会出问题

---

### 步骤

1. **克隆本项目到本地并进入项目目录**
   - 打开终端或命令提示符，执行以下命令克隆项目：
     ```shell
     git clone https://github.com/pxx917144686/iOS17/archive/refs/heads/main.zip
     ```
     或者下载 ZIP 文件并解压。

2. **安装依赖**（建议使用虚拟环境）
    ```shell
    pip3 install -r requirements.txt
    ```
    - 如果 `pip3` 无法安装，请使用 `pip` 替代：
      ```shell
      pip install -r requirements.txt
      ```
    - 如果提示没有需要的版本，请尝试不适用国内源。

3. **修改配置和路线文件**  
   - 参考项目文档中的 [使用方法](https://github.com/iOSRealRun/iOSRealRun-cli/blob/main/README.md#%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95) 的第 4、5、7 步，按需修改配置文件。

4. **连接设备**
   - 将 iPhone 或 iPad 连接到电脑并解锁设备。
   - 如果出现 "信任此电脑" 的提示，请点击 **信任**。

5. **启动程序**
   - **Windows 用户**：
     - 以 **管理员身份** 打开终端（cmd 或 PowerShell），进入项目目录后执行：
       ```shell
       python main.py
       ```
   - **macOS 用户**：
     - 打开终端，进入项目目录后执行：
       ```shell
       sudo python3 main.py
       ```
     - 注意：macOS 需要 `sudo` 权限来创建 `tun` 设备，因此需要管理员权限。

6. **检查设备连接**
   - 如果程序提示未检测到设备，请确保：
     1. iTunes 已安装并打开（适用于 Windows 用户）。
     2. 设备已解锁，并在出现提示时选择 **信任**。

7. **终止程序**
   - 使用 `Ctrl + C` 来终止程序，否则设备可能无法恢复正常定位。

8. **恢复定位**
   - 如果设备定位功能未恢复，尝试重启 iPhone 或 iPad。

---

## 常见问题

- **程序无法检测到设备**：确保设备解锁，iTunes 打开，重新运行程序。
- **定位未恢复**：重启 iPhone 或 iPad 可恢复正常。

