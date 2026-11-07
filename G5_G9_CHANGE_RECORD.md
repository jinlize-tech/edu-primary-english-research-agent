# G5/G9 产品修改记录

- 产品编号：$(@{number=44; product_id=JLZ-EDU-AG-009; chinese_name=小学英语教研; english_name=Primary English Research Agent; repository_name=edu-primary-english-research-agent; repository_url=https://github.com/jinlize-tech/edu-primary-english-research-agent; product_type=Agent; category_code=03; category=03 教学教研中心; description=小学英语词汇、语法、阅读及教学设计。; target_users=System.Object[]; core_input=教材版本、年级、单元、词汇语法阅读主题、课标要求与学情; main_output=语言目标、知识结构、教学活动、练习建议、评价标准和易错点; product_risk=语法/用法准确性、超纲和年龄不适配; dedup_label=需要明确差异化; dedup_note=与禾苗老师平台区分：小学英语专项教研，不生成完整课件和素材平台。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：小学英语教研
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：小学英语词汇、语法、阅读及教学设计。
- 主要风险：语法/用法准确性、超纲和年龄不适配
- 去重边界：与禾苗老师平台区分：小学英语专项教研，不生成完整课件和素材平台。

- 先核对学段、学科、教材版本、课程标准和既有教学资料，防止版本错配。
- 把学习目标、活动、练习、评价和作业建立可追踪对应关系。
- 区分知识、能力、过程方法和素养目标，并按认知层级与难度检查覆盖。
- 对题目、答案、评分标准和教学结论标注来源及人工复核要求。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
