# frameworks 简介

\[ [English](README.md) | 简体中文 \]

本项目采用顶层仓库（super repository）管理多个子仓库的方式进行组织。通过这种方式，可以更好地管理和维护不同部分的代码库，同时确保每个子仓库的独立性和灵活性。子仓库以 `frameworks` 字段开头。

## 子仓库列表

| 子仓库链接                                                   | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [frameworks_bluetooth](../../../../open-vela/frameworks_bluetooth) | 该仓库旨在为应用程序开发者提供丰富的蓝牙应用编程接口，包括 API 接口层、各种 Services 服务组件层、SAL 协议栈适配层和 HAL 硬件适配层。|
| [frameworks_connectivity_telephony](../../../../open-vela/frameworks_connectivity_telephony) | 该仓库为应用程序提供了一组功能丰富的工具和接口，涵盖网络服务、通话服务、短信服务、数据服务和 SIM 卡服务。通过这些接口，应用开发者无需深入了解 `Telephony` 的内部业务逻辑，只需调用 `API` 即可轻松获取与 `Telephony` 相关的信息，并高效完成应用开发。 |
| [frameworks_graphics_uikit](../../../../open-vela/frameworks_graphics_uikit) | 该仓库基于 `LVGL` 提供了 `video` 等特色组件，并扩展了字体管理机制，同时包含多个基于这些组件的 demo 用例，帮助开发者快速上手。 |
| [frameworks_multimedia_media](../../../../open-vela/frameworks_multimedia_media) | 该仓库提供了用于实现多媒体播放与录制、音频焦点管理、音频策略等关键接口。通过这些接口，开发者可以轻松实现多媒体相关功能。 |
| [frameworks_multimedia_media_pfw](../../../../open-vela/frameworks_multimedia_media_pfw) | 该仓库为通用状态机框架，提供接口给音频策略模块使用。 |
| [frameworks_runtimes_services_brightness](../../../../open-vela/frameworks_runtimes_services_brightness) | 该仓库提供亮度控制功能，支持根据环境光自动调节屏幕亮度，并允许用户手动调整亮度，同时实时修改控制曲线。 |
| [frameworks_runtimes_services_am](../../../../open-vela/frameworks_runtimes_services_am) | 该仓库实现了 `openvela` 在多应用框架下的应用程序生命周期管理，包括活动的创建、启动、暂停、恢复和销毁。 |
| [frameworks_runtimes_services_pm](../../../../open-vela/frameworks_runtimes_services_pm) | 该仓库实现了 `openvela` 在多应用框架下的应用包管理功能，包括安装、卸载和查询。 |
| [frameworks_runtimes_services_system_server](../../../../open-vela/frameworks_runtimes_services_system_server) | 该仓库实现了 `openvela` 在多应用框架下启动和管理多个系统服务的功能，包括应用管理、包管理、窗口管理和亮度管理服务。 |
| [frameworks_runtimes_services_wm](../../../../open-vela/frameworks_runtimes_services_wm) | 该仓库实现了 `openvela` 在多应用框架下的窗口管理功能，包括输入、输出和显示管理等能力。 |
| [frameworks_runtimes_services_xmsdemo](../../../../open-vela/frameworks_runtimes_services_xmsdemo) | 该仓库提供了 `openvela` 在多应用框架下的应用开发 demo，适合初学者和开发者快速上手。 |
| [frameworks_runtimes_typescript_ts2native](../../../../open-vela/frameworks_runtimes_typescript_ts2native) | 该仓库提供了 `openvela` 中将 `TypeScript` 转换为 `Native` 代码的核心框架和示例。 |
| [frameworks_runtimes_typescript_ts2wasm](../../../../open-vela/frameworks_runtimes_typescript_ts2wasm) | 该仓库是 `openvela` 中将 `TypeScript` 语言转换为 `Wasm` 字节码的核心框架和示例，旨在提高 `TypeScript` 的运行性能。 |
| [frameworks_runtimes_wasm](../../../../open-vela/frameworks_runtimes_wasm) | 该仓库提供了 `openvela` Wasm 运行时环境的部分示例和扩展 API 实现，使用该框架可以快速将系统的能力导入到 Wasm 运行时环境中。 |
| [frameworks_security](../../../../open-vela/frameworks_security) | 该仓库主要包含了 `openvela TEE（Trusted Execution Environment）` 默认的安全应用 `TA（Trusted Application）` 和 `CA（Client Application）` 实现。 |
| [frameworks_security_optee_vela](../../../../open-vela/frameworks_security_optee_vela) | 该仓库提供了兼容 `openvela` 内核的 `OPTEE（Open Portable Trusted Execution Environment）` 框架实现，使用 `OPTEE` 框架可以快速接入 `openvela` 系统，无需了解 `openvela` 架构层的细节。 |
| [frameworks_system_binder](../../../../open-vela/frameworks_system_binder) | 该仓库提供了 `Binder` 各种场景的示例、性能测试程序，以及 `C` 语言版本的实现，旨在支持 `Binder` 的学习和开发。 |
| [frameworks_system_charger](../../../../open-vela/frameworks_system_charger) | 该仓库提供了 `openvela` 充电服务，用于监控和管理电池充电过程，包括温控、限流和停复充等场景，确保电池安全快速充电。 |
| [frameworks_system_healthd](../../../../open-vela/frameworks_system_healthd) | 该仓库提供了 `openvela` 电池信息监控服务，通过 `battery_state` 主题向外发布，供应用通过 `uORB` 框架订阅。 |
| [frameworks_system_ota](../../../../open-vela/frameworks_system_ota) | 该仓库主要包含 `OTA` 实现和 `AVB` 验签实现。 |
| [frameworks_system_topics](../../../../open-vela/frameworks_system_topics) | 该仓库提供了 `openvela` 常用 `topic` 的定义，包括系统、连接和虚拟传感器等，支持通过 `uORB` 框架进行发布和订阅。 |
| [frameworks_system_utils](../../../../open-vela/frameworks_system_utils) | 该仓库包含了系统基础组件和服务，包括 `gdbus`、`kvdb`、`trace` 和 `uv` 等。 |
| [frameworks_system_utils_uv](../../../../open-vela/frameworks_system_utils_uv) | 该仓库实现了 `libuv` 风格的数据库和网络等接口，便于将这些能力集成到基于 `libuv` 的异步应用程序中。 |
| [frameworks_system_vibrator](../../../../open-vela/frameworks_system_vibrator) | 该框架旨在为各种设备提供强大的振动功能，通过可自定义的振动模式、幅度和强度提升用户体验，并支持跨核 API 调用以控制振动器设备。 |