# 汽车能量管理系统 (Automotive EMS) Simulink 仿真模型

本项目是一个基于 Simulink 搭建的汽车 EMS（能量管理系统/整车控制策略）简易仿真模型。主要用于模拟和验证车辆在特定工况下的能量分配与控制逻辑。

## 🚗 模型适用场景
* 适用车型: 混合动力汽车 (HEV/PHEV)  
* 核心目标: 优化整车能量分配，维持电池 SOC，提高经济性。

## 🛠 开发环境
* **MATLAB 版本**: MATLAB R2024a
* **依赖工具箱**: Simulink

## 🧩 核心模块说明
本模型主要包含以下几个子系统：
1. **驾驶员模型 (Driver Model)**: 模拟加速/制动踏板信号输入。
2. **EMS 控制策略 (EMS Controller)**: 包含核心的能量分配逻辑，本模型基于规则的控制。
3. **动力电池系统 (Battery System)**: 估算和输出电池 SOC、电压及电流。
4. **燃料电池系统（Fuel Cell System）**: 根据EMS控制策略决定燃料电池释放功率。
5. **车辆动力学 (Vehicle Dynamics)**: 模拟整车纵向行驶阻力与车速计算。

## 🖼 模型总览
<img width="1349" height="711" alt="image" src="https://github.com/user-attachments/assets/9aca61ba-941c-4bf2-8bf7-3fce2162ff56" />


## 🚀 快速开始
1. 克隆或下载本仓库到本地。
2. 在 MATLAB 中，将当前文件夹切换到本仓库目录。
3. 打开模型文件 `EMS_model.slx`。
4. 点击 **Run** 开始仿真，可以通过 Scope 查看车速跟随情况与 SOC 变化曲线。
