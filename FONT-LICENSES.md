# Monkey King 字体授权说明

本文用于记录主题预设字体的来源、授权信息与下载入口。

## 用户快速入口（先看这里）

`font-pack-open.zip` 已包含可再分发字体。  
以下字体不包含在开源字体包中，需要从官方渠道下载安装：

| 字体 | 原因 | 官方下载/说明 |
| --- | --- | --- |
| HONOR Sans CN | 官方页面可免费商用，但再分发边界不明确 | <https://www.honor.com/cn/support/content/zh-cn15838783/> |
| MiSans | MiSans License 对再分发有额外限制 | <https://hyperos.mi.com/font/en/download/> |

安装后重启 Obsidian 即可生效（否则主题通过 `local()` 读取系统默认字体）。

## 预设字体映射

| 预设 | 黑体 | 宋体 | 楷体 | 仿宋 |
| --- | --- | --- | --- | --- |
| 花果山 | HONOR Sans CN | 屏显臻宋 | Yozai | 朱雀仿宋（预览测试版） |
| 凌霄宝殿 | MiSans | GenWanMin2 JP | 霞鹜文楷 | 朱雀仿宋（预览测试版） |

## 字体授权清单

| 字体 | 来源 | 授权类型 | 是否可放入“开源字体包” | 官方链接 |
| --- | --- | --- | --- | --- |
| HONOR Sans CN | 荣耀官方字体 | 官方页面注明可免费商用（未明确再分发边界） | 否，建议仅提供官方下载链接 | <https://www.honor.com/cn/support/content/zh-cn15838783/> |
| MiSans | 小米字体 | MiSans License | 否，协议通常限制再次分发字体文件 | <https://hyperos.mi.com/font/en/download/> |
| 霞鹜文楷（LXGW WenKai） | lxgw 开源项目 | SIL Open Font License 1.1 | 可打包（需附 OFL 许可证） | <https://github.com/lxgw/LxgwWenKai> |
| Yozai | lxgw 开源项目 | SIL Open Font License 1.1 | 可打包（需附 OFL 许可证） | <https://github.com/lxgw/yozai-font> |
| 朱雀仿宋 | TrionesType 开源项目 | SIL Open Font License 1.1 | 可打包（需附 OFL 许可证） | <https://github.com/TrionesType/zhuque> |
| GenWanMin2 JP | ButTaiwan 开源项目 | SIL Open Font License 1.1 | 可打包（需附 OFL 许可证） | <https://github.com/ButTaiwan/genwan-font> |
| 屏显臻宋 | [chncwk](https://www.cnprint.org/bbs/member.php?u=208430)修改自思源宋体 | SIL Open Font License 1.1 | 可打包（需附 OFL 许可证） | <https://github.com/adobe-fonts/source-han-serif> |

## 开发者打包提示

发布策略：

1. 发布 `开源字体包`（仅含明确允许再分发的字体）。
2. 对受限字体提供官方安装链接，不打包字体文件。
3. 主题通过 `local()` 读取系统字体，不内置远程下载。

### OFL 字体打包要求

打包 OFL 字体，要至少同时满足：

1. 保留原始版权声明与许可证文件（通常是 `OFL.txt`）。
2. 不得单独售卖字体文件本身。
3. 若修改字体，需按 OFL 规则更名并标注变更。

参考：

- OFL 官方说明: <https://software.sil.org/oflt/>
- OFL FAQ: <https://software.sil.org/oflt/#faq>

## 发布检查清单

- [ ] 已发布 `开源字体包`（仅包含允许再分发字体）
- [ ] 主题发布包中不含未授权字体文件
- [ ] 对 OFL 字体附带许可证文件
- [ ] 对商业字体明确“用户自行安装”

## 兜底字体来源（fallback）

主题回退链中还可能使用：

- Source Han Sans: <https://github.com/adobe-fonts/source-han-sans>
- Source Han Serif: <https://github.com/adobe-fonts/source-han-serif>
- Noto CJK: <https://github.com/notofonts/noto-cjk>
