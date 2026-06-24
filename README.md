# Spot Machine Costing Skill

一个用于服务器现货机器成本核算的 Mavis skill 模板。

它适用于用户提供服务器图片、品牌、数量、采购或交易信息后，由 agent 写入指定电子表格，识别配置摘要，基于标准价库拆分配置差异成本，并补齐核算公式的工作流。

## 特点

- 通过表头语义动态定位列，不绑定固定列字母。
- 从标准价库读取价格，不把价格硬编码到 skill。
- 对配置、价格、字段位置不确定时写 `待确认`，避免猜测。
- 支持规则变更后的回归检查，日常新增机器只做自动核对。

## 安装

将 `skills/spot-machine-costing` 复制到你的 Mavis agent skills 目录，例如：

```bash
cp -R skills/spot-machine-costing ~/.mavis/agents/main/skills/
```

## 隐私说明

本仓库不包含任何私有工作簿链接、公司身份、客户信息、供应商信息或采购数据。
