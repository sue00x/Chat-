<div align="center">
<h1>Chat中移小智</h1>

> 基于GPT-SoVITS的智能语音聊天助手

</div>

![alt text](img/image.png)
--
新增无参考音频 直接对话
![alt text](img/image-1.png)

## 功能：

1. **零样本对话** 

3. **跨语言支持** 

4. **WebUI** 


## 安装


### 测试通过的环境

- Python 3.9，PyTorch 2.0.1，CUDA 11
- Python 3.10.13，PyTorch 2.1.2，CUDA 12.3
- Python 3.9，Pytorch 2.2.2，macOS 14.4.1（Apple 芯片）
- Python 3.9，PyTorch 2.2.2，CPU 设备

_注: numba==0.56.4 需要 python<3.11_

### Windows

如果你是 Windows 用户（已在 win>=10 上测试）:
```bash
git clone https://github.com/sue00x/Chat-zyxz.git
```
cd到根目录，添加文件：`ffprobe.exe`, `ffmpeg.exe`。双击 `go-webui.bat` 即可启动 GPT-SoVITS-WebUI。


### Linux

```bash
conda create -n GPTSoVits python=3.9
conda activate GPTSoVits
bash install.sh
```

### macOS

**注：在 Mac 上使用 GPU 训练的模型效果显著低于其他设备训练的模型，所以我们暂时使用CPU进行训练。**

1. 运行 `xcode-select --install` 安装 Xcode command-line tools。
2. 运行 `brew install ffmpeg` 或 `conda install ffmpeg` 安装 FFmpeg。
3. 完成上述步骤后，运行以下的命令来安装本项目：

```bash
conda create -n GPTSoVits python=3.9
conda activate GPTSoVits

pip install -r requirements.txt
```

### 手动安装

#### 安装依赖

```bash
pip install -r requirements.txt
```

#### 安装 FFmpeg

##### Conda 使用者

```bash
conda install ffmpeg
```

##### Ubuntu/Debian 使用者

```bash
sudo apt install ffmpeg
sudo apt install libsox-dev
conda install -c conda-forge 'ffmpeg<7'
```

##### Windows 使用者

下载并将 [ffmpeg.exe](https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/ffmpeg.exe) 和 [ffprobe.exe](https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/ffprobe.exe) 放置在 GPT-SoVITS 根目录下。

项目模型
---
GPT-SoVITS：https://github.com/RVC-Boss/GPT-SoVITS.git



