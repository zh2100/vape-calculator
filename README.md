# 电子烟油配方计算器

一个专业的电子烟油配方计算工具，支持尼古丁浓度计算、PG/VG比例调配、香精配比等功能。基于Flutter开发，支持Web端和移动端使用。

## ✨ 主要功能

- 🧮 **精确计算** - 烟油配方精确计算，支持毫升和滴数显示
- 🎯 **尼古丁调配** - 支持不同浓度尼古丁基液的计算
- ⚖️ **PG/VG比例** - 自定义PG/VG比例，支持MaxVG模式
- 🌸 **香精配比** - 多种香精组合，支持不同PG/VG比例香精
- 💾 **配方保存** - 本地保存常用配方，方便重复使用
- 📱 **移动优化** - 响应式设计，完美适配手机和平板
- 🔄 **PWA支持** - 可安装到桌面，支持离线使用

## 🚀 在线使用

访问在线版本：[https://zh2100.github.io/vape-calculator](https://你的用户名.github.io/vape-calculator)

### PWA安装
- **Android**: 在Chrome中访问网站，点击"添加到主屏幕"
- **iOS**: 在Safari中访问网站，点击分享按钮 → "添加到主屏幕"

## 🛠️ 本地开发

### 环境要求
- Flutter SDK 3.0+
- Chrome浏览器（用于Web开发）

### 快速启动
```bash
# 克隆项目
git clone https://github.com/你的用户名/vape-calculator.git
cd vape-calculator

# 安装依赖
flutter pub get

# 启动开发服务器
flutter run -d chrome
```

### 批处理脚本（Windows）
项目提供了便捷的批处理脚本：

- `启动应用.bat` - 完整启动流程，包含环境检查
- `快速启动.bat` - 快速启动，适合日常开发
- `清理重启.bat` - 清理缓存后重新启动
- `构建静态文件.bat` - 构建生产版本

## 📦 构建部署

### Web版本构建
```bash
# 构建Web版本
flutter build web

# 构建相对路径版本（用于GitHub Pages）
flutter build web
# 然后修改 build/web/index.html 中的 base href 为 "./"
```

### GitHub Pages部署
1. 运行构建脚本生成静态文件
2. 将 `build/web` 文件夹内容上传到GitHub仓库
3. 在仓库设置中启用GitHub Pages
4. 访问 `https://你的用户名.github.io/仓库名`

详细部署指南请参考：[手动GitHub部署指南.md](手动GitHub部署指南.md)

## 📱 移动端使用

### 方案一：Web版本（推荐）
- 直接在手机浏览器中访问
- 支持PWA安装，获得原生应用体验
- 自动更新，无需手动维护

### 方案二：原生应用
```bash
# Android
flutter build apk

# iOS（需要Mac环境）
flutter build ios
```

详细移动端部署指南：[手机使用完整指南.md](手机使用完整指南.md)

## 🧪 测试

### 运行测试
```bash
# 运行所有测试
flutter test

# 运行特定测试
flutter test test/services/calculator_service_test.dart

# 生成覆盖率报告
flutter test --coverage
```

### 测试覆盖
- 单元测试：计算逻辑、数据模型
- Widget测试：UI组件功能
- 集成测试：完整用户流程

详细测试指南：[测试指南.md](测试指南.md)

## 📖 使用说明

### 基本操作
1. **输入参数** - 设置目标体积、尼古丁浓度、PG/VG比例
2. **添加香精** - 选择香精类型和浓度
3. **生成配方** - 点击计算按钮获得详细配方
4. **保存配方** - 将常用配方保存到本地

### 计算示例
**目标配方**: 100ml, 6mg尼古丁, 30%PG/70%VG, 草莓5% + 香草3%

**计算结果**:
- 尼古丁基液(36mg): 16.67ml (583滴)
- PG溶剂: 5.33ml (187滴)
- VG溶剂: 70.00ml (2450滴)
- 草莓香精: 5.00ml (175滴)
- 香草香精: 3.00ml (105滴)

## 🔧 故障排除

### 常见问题
- **构建失败**: 检查Flutter版本，运行 `flutter doctor`
- **页面空白**: 检查base href路径设置
- **数据丢失**: 检查浏览器存储设置，避免使用隐私模式
- **PWA无法安装**: 确保使用HTTPS访问

详细故障排除：[使用说明.md](使用说明.md)

## 🤝 贡献

欢迎提交Issue和Pull Request！

### 开发流程
1. Fork项目
2. 创建功能分支
3. 提交更改
4. 创建Pull Request

### 代码规范
- 遵循Dart代码规范
- 添加必要的测试
- 更新相关文档

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🙏 致谢

- Flutter团队提供的优秀框架
- 社区贡献的各种插件和工具
- 所有测试用户的反馈和建议

## 📞 联系方式

- 项目地址: [GitHub](https://github.com/你的用户名/vape-calculator)
- 问题反馈: [Issues](https://github.com/你的用户名/vape-calculator/issues)

---

**免责声明**: 本工具仅供计算参考，请根据实际情况调整配方。使用电子烟产品请遵守当地法律法规。
