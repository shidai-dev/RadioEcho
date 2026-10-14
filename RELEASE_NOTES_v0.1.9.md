# Radio Echo v0.1.9

免费 Android `arm64-v8a` 公开预览维护版本，重点改善地图查看、FT8 时间检查和户外快捷频率操作。

## 核心更新

- **通联地图：** 采用大圆短路径和全球取景，细化网格与呼号标签。日志地图围绕本台缩放，支持单指四向拖动；手动拖动后缩放保持当前视野。保留确认状态颜色、图层开关，新增离线海岸线后备底图。
- **FT8 时间与状态：** FT8 工作台新增一键 UTC 同步；已应用的校正偏移不再被误判为剩余时隙误差。真实接收采样证据用于链路就绪状态，避免旧传输统计误报断流。
- **快捷频率：** FT8 增加 `2m / 144.174 MHz` 并修复窄格折行；CW 支持最多 8 个可编辑、可删除且持久化的频点，单行显示并可横向滑动。

## English

- Great-circle QSO paths, global overview, clearer grids and collision-aware labels; log maps support station-centered zoom and single-finger pan. Offline coastlines remain available without online tiles.
- One-tap UTC sync in the FT8 workspace, corrected clock-health evaluation, and receive readiness based on recent audio samples rather than stale transport counters.
- A compact 2m FT8 preset at 144.174 MHz and up to eight persistent, editable CW frequency favorites.

## 验证和限制 / Verification and Limitations

- 510 项自动化测试、TypeScript、正式签名构建及设备保留数据升级验收；最终产物信息见 `RELEASE_MANIFEST.json` 和 `SHA256SUMS.txt`。
- 本台位置由设置中的梅登格推导，不是实时 GPS。日志大数据总览最多绘制 160 个地理分散的代表点/路径，完整记录仍可在列表查询。地图支持单指拖动与按钮缩放，暂不支持双指缩放。
- 传播密集标注、断网切换、2 米空中通联及全部机型组合尚未完成现场验收；不新增未经验证的电台支持承诺。升级前导出配置与完整 ADIF。
- Public build uses the MIT-licensed `ft8_lib` backend. No new radio-driver or decoding-engine implementation is introduced in this release. Dense FT8 reception and continuous automatic QSOs remain field-test areas.
- 本版本仍为 **Pre-release**，发射必须由持证操作员监督。

包名：`cn.bi1rre.radioradioecho`；版本：`0.1.9 (10)`；最低 API 24；目标 API 35。
