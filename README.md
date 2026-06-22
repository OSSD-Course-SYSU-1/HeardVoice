# HeardVoice - 鸿蒙语音助手

基于 sherpa-onnx 的 HarmonyOS 本地语音识别应用。

## 项目来源

- **原始仓库**: [k2-fsa/sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx)
- **基础工程**: harmony-os/SherpaOnnxVadAsr
- **开源协议**: Apache-2.0

## 功能特性

- 🎤 本地语音识别（VAD + ASR）
- 🌐 支持中文/英文/日文/韩文/粤语自动检测
- 📁 支持文件识别和麦克风录音
- 🔒 完全本地运行，无需网络

## 技术栈

- HarmonyOS / OpenHarmony
- ArkTS / ArkUI
- sherpa_onnx 三方库

## 核心模块说明

| 文件 | 功能 |
|------|------|
| Index.ets | 主页面 UI，包含文件识别、麦克风录音、帮助三个标签页 |
| NonStreamingAsrWithVadWorker.ets | Worker 线程，执行语音识别逻辑 |
| NonStreamingAsrModels.ets | 模型配置，支持 23 种语音识别模型 |
| Permission.ets | 动态申请麦克风权限 |

