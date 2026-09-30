# 国外法律 AI 竞品调研报告（2024–2026）

> 调研对象：面向中国创业者打造「法律 AI 智能体」项目的国外/海外标杆产品
> 调研时间：2026 年 9 月
> 范围：美国、英国、欧洲、印度市场；B 端律所/法务 + C 端消费者两条路线

---

## 核心发现（摘要）

1. **市场格局已分化为三大阵营**：①老牌法律数据巨头（Thomson Reuters Westlaw、RELX LexisNexis）靠自有判例库 + RAG 做「AI 增强版检索」；②原生垂直 AI 创业公司（Harvey、Legora、Spellbook、EvenUp）靠大模型 + 工作流切入，估值在 2025 年集体暴涨；③通用大厂（Microsoft、Google、OpenAI）不做专用法律产品，而是把模型塞进 Office/Workspace，作为「底座」让垂直公司跑在上面。

2. **B 端是唯一被验证的付费市场，C 端"机器人律师"路线已被监管证伪**：DoNotPay 因虚假宣传"AI 律师可替代真人"被美国 FTC 罚款 19.3 万美元并禁止此类宣称，成为行业反面教材。所有跑出来的公司（Harvey、Spellbook、EvenUp）全部服务律所/公司法务，客单价数千到数万美元/年，且强调"AI 辅助律师、不替代律师"。

3. **2025 年是法律 AI 的融资爆发年，估值逻辑从"工具"切换到"Agent 平台"**：Harvey 一年内从 30 亿→50 亿→80 亿美元估值（2025 年 2/6/12 月三轮），ARR 从约 7500 万美元（2025/4）涨到约 1.9 亿美元（2025 年底）；Legora 2025 年 10 月 C 轮 1.5 亿美元估值 18 亿美元；EvenUp E 轮 1.5 亿美元估值 20 亿美元。资本押注的是"能自主跑多步任务的 Agent"，而非聊天框。

4. **数据护城河 > 模型本身**：Harvey 与 LexisNexis（RELX）战略合作拿到判例库使用权；CoCounsel 直接长在 Westlaw 数据里；Legora 主打"训练法律原生模型"而非套壳通用模型。没有合规权威法律语料，再强的模型也会幻觉出假案例——这是法律 AI 的生死线。

5. **技术路线趋同：通用大模型 + 法律领域微调 + RAG 引用回链 + 人机协同**：几乎所有产品都基于 GPT-4/GPT-5、Claude 或 Gemini 做领域微调，叠加私有法律语料检索（RAG），并强制输出可核验的判例/法条引用（citation）。Harvey 与 OpenAI 合作训练了"定制判例模型"，Spellbook 按任务路由 GPT/Claude，Lexis 推出"模型自选"。

6. **"嵌入律师现有工作流"是产品胜负手**：Spellbook 活在 Microsoft Word 里、Luminance 做 Word 插件、Lexis Create+ 进 Word、CoCounsel 绑 Westlaw——律师不愿切换窗口，谁能钻进 Word/Outlook/Teams，谁就拿到日常使用频次。独立网页端产品转化率显著更低。

7. **垂直单点切入再横向扩张是被验证的路径**：EvenUp 只做人身伤害索赔函、Kira 只做 M&A 尽调条款抽取、Spellbook 只做合同起草——先在一个窄场景做到 10 倍效率提升、拿下标杆客户，再扩到相邻领域。Harvey 从律所研究/起草出发，正在向税务、会计扩张。

8. **"AI + 持证律师人工复核"的混合交付模式在合同领域仍是主流，但正被质疑**：Robin AI 等公司养几十名持证律师 + 印度外包标注团队，AI 初稿必须人工签字。这种模式毛利低、增速慢，2025 年已有投资人公开质疑"这到底是不是 AI 公司"。中国创业者需权衡：是做高毛利纯软件，还是做带人工服务的"AI 工作室"。

9. **巨头既当裁判又当运动员**：RELX（LexisNexis 母公司）的风投 REV 同时投了 Harvey、EvenUp；Thomson Reuters Ventures 投了 Spellbook。法律数据巨头通过投资 + 收购把创业公司变成自己生态的插件——Casetext 被 TR 以 6.5 亿美元收购后，独立 CoCounsel 产品已于 2025 年 3 月停用并入 Westlaw。

10. **版权/训练数据合规是悬顶之剑**：Anthropic 因用盗版书训练 Claude，2025 年以 15 亿美元和解（美国史上最大版权和解案）。法律 AI 公司训练语料是否侵权、输出是否可被律师作为依据，直接决定产品能否在大律所落地。中国创业者从第一天起就必须解决"数据来源合规 + 引用可追溯"。

11. **定价模式**：成熟产品普遍走企业订阅制，按席位/年签约——CoCounsel 加 Westlaw 约 300–600 美元/用户/月，Westlaw Advantage 约 288 美元/月起，Spellbook 约 108–149 美元/用户/月，SpotDraft 中位客单价约 2.5 万美元/年。几乎没有 C 端低价订阅跑通的（DoNotPay 反例）。

12. **对中国创业者的启示**：①不要做 C 端"替你打官司"的噱头产品，监管风险极高；②从合同审查/法律检索/尽调等 B 端高频痛点切入；③必须解决中国本土法律数据（裁判文书、法规、合同模板）的合规获取；④产品要嵌进律师已用的工具（Word/微信/钉钉/飞书）；⑤"AI 辅助、律师负责"是安全且被验证的话术。

---

## 一、重点产品逐一调研

### 1. Harvey（Harvey AI）—— 法律 AI 领域的绝对头部

- **定位与目标用户**：面向 Am Law 100 顶级律所和财富 500 强法务部的"通用法律 AI 平台"。2022 年由前 O'Melveny 律师 Winston Weinberg 与前 DeepMind 研究员 Gabriel Pereyra 创立，总部旧金山。
- **核心功能**：法律检索、法律文书起草、尽调、合同分析、客户问询；2025 年推出 **Workflow Builder**（让律所自建自动化工作流，如驳回动议、简易判决动议），12 月推出 **Shared Spaces**（团队协作空间）。
- **技术路线**：基于 OpenAI GPT-4 级模型做**法律领域微调**，叠加法律语料检索层；与 OpenAI 合作训练了定制判例模型；2025 年与 **LexisNexis 达成战略合作**获得判例库数据接入。
- **数据来源**：公开判例 + LexisNexis 授权数据 + 客户内部文档 RAG。
- **商业模式与定价**：企业级席位订阅，不公开定价（面向大律所定制）。
- **融资/ARR/客户**：
  - 2025/2 D 轮 3 亿美元（估值 30 亿）；2025/6 E 轮 3 亿美元（Kleiner Perkins + Coatue 领投，估值 50 亿）；2025/12 F 轮 1.6 亿美元（a16z 领投，估值 80 亿）。2025 年内三轮共融资约 7.5 亿美元，累计融资超 10 亿（2026 年估值传至 110 亿）。
  - ARR：约 7500 万美元（2025/4）→ 约 1.9 亿美元（2025 年底）。
  - 客户：2400+ 家、覆盖 70+ 国家；70+ 家 Am Law 100 律所；标杆包括 Paul Weiss、A&O Shearman（原 Allen & Overy）、PwC Legal、KKR。
  - 投资方阵容豪华：Sequoia、Kleiner Perkins、GV、OpenAI Startup Fund、Coatue、a16z、EQT、T. Rowe Price，以及 **RELX（LexisNexis 母公司）风投 REV**。
- **优势与短板**：优势是品牌、客户密度、资金、与 OpenAI/Lexis 的双重绑定；短板是估值极高、需向税务会计等新领域扩张以支撑；作为"套壳"通用模型的公司，面临基础模型厂商（OpenAI/Anthropic 自营）和数据巨头（Westlaw/Lexis）两头挤压的风险。
- **争议**：本身无重大处罚，但身处 AI 训练数据版权诉讼大背景下（Anthropic 15 亿美元和解案），其法律语料使用合规性受关注。
- **可借鉴点**：B 端标杆客户打法（先拿下一家王牌律所做样板）、与数据方/模型方同时结盟、从单点工具扩展为 Agent 工作流平台。**不可照搬**：其烧钱速度和顶级律所客户在中国市场不存在对标。

### 2. Casetext / CoCounsel（Thomson Reuters 旗下）—— 数据巨头收购整合的样本

- **定位与目标用户**：CoCounsel 是 Thomson Reuters 面向律所/法务的 AI 助手，源自 2023 年以 **6.5 亿美元收购的 Casetext**。
- **核心功能**：法律问答、文书综述、合同审查、法律检索、Deep Research 多步研究代理；2025 年升级为 **CoCounsel Legal**，主打 agentic AI，答案旁附 Westlaw/Practical Law 权威来源引用。
- **技术路线**：最初基于 GPT-4（Casetext 是首个在真实法律任务上跑出 GPT-4 水平的产品）；被收购后深度绑定 Westlaw 数据做 RAG；2025 年收购 Safe Sign Technologies 布局法律专用大模型。
- **数据来源**：Westlaw 判例库、Practical Law 实务指南（TR 自有权威数据，这是最大护城河）。
- **商业模式与定价**：独立 CoCounsel 产品已于 **2025 年 3 月 31 日停用**，全部并入 Westlaw 订阅。第三方估算：CoCounsel 作为 Westlaw 加购约 225 美元/用户/月，含 Westlaw 全套约 300–600 美元/用户/月；Westlaw Advantage（含 Deep Research）约 288.6 美元/月起，CoCounsel Legal 套餐约 551.85 美元/月起。
- **优势与短板**：优势是 Westlaw 独家权威数据、引用可核验、与律所工作流深度集成；短板是被绑死在 Westlaw 生态内、价格昂贵、不买 Westlaw 就用不了。
- **可借鉴点**：**"权威数据 + 强制引用回链"是法律 AI 建立信任的核心**；巨头通过收购把创业公司变成自己产品的 AI 模块——这提示中国创业者，要么自己握有数据，要么随时可能被数据方收编或碾压。

### 3. Lexis+ AI / Protégé（LexisNexis / RELX）—— 另一数据巨头的应对

- **定位与目标用户**：LexisNexis（RELX 旗下）的下一代法律 AI 助手，原名 Lexis+ AI，2025–2026 年升级为 **Lexis+ with Protégé**。
- **核心功能**：法律检索、文书起草、法律分析、结果预测；内置 **Citation Agent** 主动核查引用是否过时/错误；General AI 与 Legal AI 双模式；Lexis Create+ 把助手塞进 Microsoft Word。
- **技术路线**：结合 LexisNexis 自有法律内容 + 实务指南做 RAG；**支持按任务自选模型**（起草、沟通、头脑风暴可切换不同模型），强调"安全隐私设计"的加密环境。
- **数据来源**：LexisNexis 自有判例库（含英国 All England Law Reports 等独家内容）。
- **商业模式与定价**：企业定制报价，第三方估算 Lexis+ 核心检索约 300–500+ 美元/用户/月；法国市场约 125 欧元/月/律师/专题。
- **优势与短板**：优势是与 Harvey 是"竞合关系"——RELX 一边投 Harvey 一边自己做 Protégé，数据在手；短板是产品迭代速度不如创业公司。
- **可借鉴点**：双模式（专业 Legal AI + 通用 General AI）、Citation Agent 自动纠错引用、模型可路由——这些是降低幻觉的工程范式。

### 4. Westlaw Precision / Westlaw Advantage（Thomson Reuters）

- **定位**：TR 旗舰法律检索平台的 AI 升级版。**Westlaw Advantage 于 2025 年 8 月推出**，头条功能是 **Deep Research**——agentic AI 自动制定多步研究计划、迭代执行、产出带正反方论证和透明推理链的研究报告，每条结论链接回 Westlaw 原始/次级法律资料。
- **定价**：Westlaw Edge 约 155.35 美元/月起；Westlaw Advantage 约 288.60 美元/月起；CoCounsel Legal 约 551.85 美元/月起。
- **启示**：连最传统的法律数据库都在从"检索框"转向"自主研究代理"，这是 2025–2026 年整个行业的产品形态方向——从"问答"走向"多步 Agent"。

### 5. DoNotPay —— C 端"机器人律师"的反面教材

- **定位与目标用户**：面向 C 端消费者的"世界首个机器人律师"，主打自动打官司、申诉、消除罚单、生成法律文件。
- **核心功能**：聊天机器人生成法律文书、自动申诉、各类消费者维权流程自动化。
- **技术路线**：通用大模型套壳，**未对输出做任何法律准确性测试，也未雇佣律师**（FTC 调查认定）。
- **争议/监管处罚（关键）**：
  - 2024 年 9 月美国 FTC 起诉其虚假宣传；
  - 2025 年 1 月 16 日 FTC 以 5:0 投票作出最终裁定，2 月 11 日公告：**罚款 19.3 万美元，并禁止其在无证据情况下宣称"AI 律师可替代真人律师"**，还须通知 2021–2023 年所有订阅用户。
- **可借鉴点（反面）**：①C 端"AI 替你打官司"在监管成熟市场直接违规；②"AI 能力宣称"必须有实证支撑，否则构成虚假宣传；③产品话术必须是"辅助"而非"替代"。**这是中国创业者最该研究的合规红线案例。**

### 6. LawGeex —— 早期合同审查先驱的衰落警示

- **定位**：2014 年创立于特拉维夫，最早一批"按法务 playbook 自动审查/批准合同"的公司，客户曾包括 eBay、HP、White & Case。
- **现状**：2025–2026 年已基本淡出市场（Spellbook 等竞品官网直接称"LawGeex 已不在市场上"），收入、估值、人员均不公开。
- **教训**：**"早"不等于"赢"**。基于传统 NLP/规则的合同审查没能及时拥抱大模型，被 Spellbook 这类原生 LLM 工具取代。技术路线迭代的速度比先发优势更重要。

### 7. Robin AI —— 合同领域的"AI + 人工"混合模式代表

- **定位与目标用户**：英国伦敦的企业合同审查/法律智能平台，面向公司法务和 PE 客户（如 Blue Earth Capital、Alvarez & Marsal 生态）。
- **核心功能**：合同审查、分析、定稿、跨数千份合同的智能检索与问答（Ask / Research 双模式）。
- **技术路线**：AI 自动理解合同条款 + **内部持证律师团队 + 印度外包标注**做人工复核签字，交付"4 小时 turnaround"的高质量结果。
- **融资**：A 轮 1050 万美元（2023/2，Plural）；B 轮 2600 万美元（2024/1，**新加坡淡马锡领投**）；B+ 轮 2500 万美元（2024/11，PayPal Ventures、剑桥大学）。2024 年 9 月在新加坡设亚太总部。
- **优势与争议**：优势是交付质量高、企业客户信任；短板是"AI + 人工重服务"模式毛利低、扩张靠堆人，2025 年有投资人/媒体公开质疑其"远未达到 AI 级增长"（投资人期望 AI 公司是 80%+ 毛利、3–5 倍年增长）。
- **可借鉴点**：中国创业者需决策——是做高毛利纯软件，还是做带律师人工的"AI 工作室"。前者 scalable 但质量难控，后者可信但重。

### 8. Spellbook —— Word 插件路线的高增长样本

- **定位与目标用户**：加拿大多伦多（起家于 St. John's），前身为 Rally Legal。**核心产品是 Microsoft Word 内的合同起草/审查插件**，面向律所和公司法务。
- **核心功能**：Word 内实时起草、自动红线、条款建议、风险标记、对标数千份真实合同做"市场比较"、文书问答。
- **技术路线**：前沿模型栈（GPT + Claude）按任务路由；累计审查 1000 万+合同训练；自助注册、无 demo 墙。
- **融资/ARR/客户**：种子 260 万；A 轮 2000 万（2023/5，Inovia 领投，TR Ventures、Bain 跟投）；**B 轮 5000 万美元（2025/10，Khosla Ventures 领投），投后估值约 3.5 亿美元**，累计融资超 8000 万。ARR：约 2500 万（2025 中）→ 约 5000 万（2025/10）→ 约 8000 万（2026），年增速 230%。客户 4400+ 团队、1500+ 律所。定价约 108–149 美元/用户/月（年付）。
- **可借鉴点**：①钻进 Word 这个律师主战场是最锋利的楔子；②自助 PLG + 高增速能在不拿顶级律所的情况下跑出高 ARR；③"对标真实市场合同"比单纯靠 playbook 更有壁垒。

### 9. EvenUp —— 极窄垂直场景的独角兽

- **定位与目标用户**：只做**人身伤害（personal injury）案件**的 AI——案件评估和赔偿请求函（demand letter）自动生成，面向美国原告律师。
- **融资/估值**：E 轮 1.5 亿美元（2025/10，Bessemer 领投，**REV/RELX**、B Capital、SignalFire、Bain、HarbourVest 等跟投），**估值超 20 亿美元**，累计融资约 3.85 亿美元。
- **可借鉴点**：把一个极窄场景（人身伤害赔偿函）做到极致，也能长成独角兽。垂直深度 > 横向广度。

### 10. Hebbia —— 通用企业知识 AI，法律是其落地场景之一

- **定位**：由 George Sivulka（前 OpenAI/Airbnb）创立，主打"面向金融/咨询/法律的企业知识 AI 平台"，定位偏通用 RAG/Agent 而非法律原生。
- **融资**：B 轮 1.3 亿美元（a16z 领投）。
- **与法律关系**：官方案例库中含法律（Legal）场景，但同时覆盖信贷、并购咨询等。对中国创业者的启示：通用企业知识助手可横向切法律，但纯法律场景仍需法律专用数据与引用能力。

### 11. Legora —— 法律原生模型的瑞典黑马

- **定位与目标用户**：总部斯德哥尔摩、YC 出身，2025 年 3 月进军美国。定位为"协作式法律 AI 平台"，帮律师审查、研究、起草。
- **技术路线**：**主打"训练法律原生模型"而非在通用模型上套壳**，以此对标 Westlaw/Lexis。
- **融资/估值**：早期累计 3500 万+（Benchmark、Redpoint、SV Angel、YC）；**C 轮 1.5 亿美元（2025/10/30，Bessemer 领投，ICONIQ、General Catalyst、Benchmark、YC 跟投），估值 18 亿美元**。第三方（Sacra）估计其 2026 年 ARR 约 2 亿美元、估值约 56 亿美元、年增速高达 1500%+（注：该增速为第三方估算，数字激进需谨慎看待）。
- **可借鉴点**：在数据巨头之外，仍有人靠"法律原生模型 + 极速增长"拿到天价融资——说明市场相信"垂直专用模型"叙事。

### 12. Luminance —— 欧洲 M&A 尽调老牌

- **定位**：伦敦创立，由剑桥数学家研发"Legal-Grade AI"，面向企业法务和 M&A 尽调，客户含 Slaughter and May。
- **核心功能**：异常检测、条款分类、合同审查、自主合同谈判；Word 插件嵌入谈判流程。
- **融资**：C 轮 7500 万美元（2025/2，Point72 Ventures 领投）。
- **优势**：在高风险跨境交易、异常条款识别上口碑强。

### 13. Kira Systems（Litera 旗下）—— 合同条款抽取的金标准

- **定位**：现属文档工作流厂商 **Litera**，是大规模 M&A 尽调、合同条款抽取的老牌标准工具。
- **核心数据**：被 **64% 的 Am Law 100 律所**使用；1400+ 预训练 smart fields，条款抽取准确率 90%+。
- **特点**：擅长跨数千份合同批量抽取控制权变更、转让、终止等条款，但不做红线/匿名化。是"传统 ML/NLP 时代"的代表，仍靠规模化尽调场景存活。

### 14. Eigen Technologies —— 金融导向的文档 AI

- **定位**：伦敦公司，强在金融服务业（银行、保险）的文档智能，合同/合规文档审查为副线。
- **特点**：NLP/ML 抽取，更偏企业风控而非律所前台，适合了解"法律 AI 向金融合规溢出"的路径。

### 15. SpotDraft —— 印度走出的 CLM 出海样本

- **定位**：印度班加罗尔创立（现总部纽约），AI 原生合同生命周期管理（CLM），面向公司法务。
- **核心功能**：VerifAI 合同审查、Word 红线、**端侧（on-device）AI 审查**（数据不出设备）。
- **融资**：B 轮 5400 万美元（2025/2，Vertex Growth Singapore、Trident 领投）；2026/1 获高通风投 800 万美元战略加码，累计融资约 9200 万美元。第三方估计 ARR 约 2000–4000 万美元，中位客单价约 2.5 万美元/年，年处理 100 万+合同。
- **可借鉴点**：印度团队用"英语普通法合同 + 低成本工程 + 新加坡资本"成功出海欧美——这对中国创业者是重要参照：**出海比死守国内合规市场可能更快跑通**。

### 16. 大厂动向（Microsoft / Google / OpenAI）

- **Microsoft（Copilot for Legal）**：不做专用法律产品，而是把 GPT 系列（后加入 Claude Sonnet/Opus）装进 Word/Outlook/Teams/SharePoint，推出面向律所的 Copilot for Legal，**约 30 美元/用户/月（在 M365 订阅之上加购）**。案例：荷兰 Loyens & Loeff 两个月内部署 1600 人、活跃率 94%、记录超 100 万次提问；日本 Vanguard Lawyers Tokyo 邮件起草时间砍半。
- **Google（Gemini）**：无专用法律产品，靠 Gemini for Workspace（AI Pro 约 19.99 美元/月）嵌入 Docs/Gmail/Drive，凭超长上下文（100 万–200 万 token）处理大文档。律师按习惯选用，无法律专用数据。
- **OpenAI**：不直接卖法律产品，但通过 **OpenAI Startup Fund 投资 Harvey**，并与 Harvey 合作训练定制判例模型；ChatGPT Enterprise 被大量律所自发使用。OpenAI 是法律 AI 的"模型底座供应方"。
- **大厂启示**：通用大厂是"模型 + 办公套件"的底座层，不会替你做法律语料和行业工作流——这正是垂直创业公司的生存空间，但也意味着一旦大厂与 Westlaw/Lexis 深度合作，独立创业公司会被挤压。

---

## 国外竞品功能矩阵对比表

| 产品 | 定位/目标用户 | 核心功能 | 技术路线 | 商业模式/定价 | 融资或 ARR | 优势/短板 |
|---|---|---|---|---|---|---|
| **Harvey** | 顶级律所/500强法务通用法律 AI | 检索、起草、尽调、合同、Workflow Builder、Shared Spaces | GPT-4 级法律微调 + RAG，与 OpenAI 合训判例模型，接 Lexis 数据 | 企业席位订阅（不公开） | F 轮后估值 80 亿美元；ARR 约 1.9 亿（2025 底）；2400+ 客户 | 优势：品牌/客户/资金/双绑模型与数据；短板：估值高、两头受压 |
| **CoCounsel（TR）** | Westlaw 系律所 | 问答、综述、合同审查、Deep Research | GPT-4 + Westlaw 数据 RAG，收购 Safe Sign 做法律 LLM | 并入 Westlaw，加购约 225–640 美元/用户/月 | 2023 年收购 Casetext 6.5 亿美元 | 优势：权威数据+引用；短板：绑死 Westlaw、贵 |
| **Lexis+ Protégé（RELX）** | LexisNexis 系律所/法务 | 检索、起草、Citation Agent、Word 集成 | Lexis 数据 RAG + 模型可路由 | 企业定制，约 300–500+ 美元/用户/月 | RELX 旗下；并战投 Harvey/EvenUp | 优势：自有数据；短板：迭代偏慢 |
| **Westlaw Advantage** | 律所法律检索 | Deep Research 多步研究代理 | Agentic AI + Westlaw 数据 | 约 288.6 美元/月起 | TR 内部产品 | 优势：从检索转向 Agent；短板：生态封闭 |
| **DoNotPay** | C 端消费者 | 自动申诉、生成法律文书 | 通用大模型套壳，无测试无律师 | C 端订阅 | 被 FTC 罚 19.3 万美元（2025） | 反面教材：虚假宣传"替代律师"被监管 |
| **LawGeex** | 公司法务合同审批 | 按 playbook 自动审合同 | 传统 NLP/规则 | 已基本退出市场 | 客户曾含 eBay/HP | 教训：未及时拥抱大模型而衰落 |
| **Robin AI** | 企业法务/PE 合同 | 合同审查、智能检索问答 | AI + 内部持证律师 + 印度外包复核 | 企业订阅 | B+ 轮累计约 6100 万美元；淡马锡投资 | 优势：质量可信；短板：重服务、毛利低 |
| **Spellbook** | 律所/法务合同起草 | Word 内起草、红线、风险标记、市场对标 | GPT/Claude 任务路由，1000 万+合同 | 自助订阅 108–149 美元/用户/月 | B 轮 5000 万（Khosla），估值 3.5 亿；ARR 约 5000 万–8000 万 | 优势：钻进 Word、PLG 高增长；短板：单点 |
| **EvenUp** | 人身伤害原告律师 | 案件评估、赔偿请求函 | 垂直领域 AI | 企业订阅 | E 轮 1.5 亿，估值 20 亿+ | 优势：极窄场景做到独角兽；短板：场景窄 |
| **Legora** | 律师审查/研究/起草 | 协作式法律研究与文书 | 法律原生模型（非套壳） | 企业订阅 | C 轮 1.5 亿，估值 18 亿 | 优势：原生模型叙事、增速快；短板：第三方数据激进 |
| **Luminance** | 跨境 M&A/企业法务 | 异常检测、条款审查、自主谈判 | 剑桥 Legal-Grade AI + Word 插件 | 企业订阅 | C 轮 7500 万（Point72） | 优势：高风险交易口碑；短板：欧洲为主 |
| **Kira（Litera）** | 大所 M&A 尽调 | 大规模条款抽取 | 传统 ML，1400+ smart fields | 企业订阅 | 隶属 Litera | 优势：64% AmLaw100、抽取准；短板：不做红线 |
| **Eigen** | 金融/保险文档智能 | 合规文档抽取审查 | NLP/ML | 企业订阅 | 未披露 | 优势：金融强；短板：非律所前台 |
| **SpotDraft** | 公司法务 CLM | 合同全生命周期、端侧审查 | AI 原生 CLM、on-device | 客单约 2.5 万美元/年 | B 轮 6200 万（含高通），累计约 9200 万 | 优势：印度出海范本、端侧隐私；短板：无诉讼场景 |
| **Microsoft Copilot Legal** | M365 生态律所 | Word/Outlook 文书、合同比对、综述 | GPT + Claude，租户数据 RAG | 30 美元/用户/月（加购） | 微软内部 | 优势：办公套件入口；短板：无法律数据 |
| **Google Gemini** | Workspace 生态 | 长文档处理、起草综述 | Gemini 超长上下文 | AI Pro 19.99 美元/月 | 谷歌内部 | 优势：超长上下文；短板：无法律专用能力 |
| **OpenAI** | 底座/被律所自发使用 | ChatGPT Enterprise | 自研前沿模型 | 企业订阅 | 投资 Harvey、合训模型 | 优势：底座；短板：不做行业应用 |

---

## 对中国创业者的可借鉴点与不可照搬之处（汇总）

**可借鉴：**
- 切入 B 端（律所/企业法务），话术用"AI 辅助律师"而非"替代律师"，规避 DoNotPay 式监管风险。
- 从极窄高频场景（合同审查、尽调、类案检索、文书起草）单点打透，再横向扩张。
- 产品必须嵌入律师已有工具（Word/微信/飞书/钉钉），不要做独立大而全网页。
- 建立合规法律数据护城河 + 强制引用可追溯，解决幻觉问题。
- 工程上做 RAG + 领域微调 + 模型路由 + 引用核查 Agent。
- 可参考印度 SpotDraft 路径，考虑用中文法律场景能力出海（东南亚普通法/涉外合同）。

**不可照搬：**
- 不要做 C 端"AI 替你打官司"的噱头产品（监管与伦理红线）。
- Harvey/Legora 那种"套壳基础模型 + 天价估值"建立在美元风投和 Am Law 客户之上，中国市场缺顶级律所付费土壤，不能照搬烧钱换估值逻辑。
- Westlaw/Lexis 那种"自有百年法律数据库"在中国不存在直接对应（裁判文书公开政策已收紧），数据获取路径需重新设计。
- 美国按席位 300–600 美元/月的高定价在国内难以直接复制，需探索适合国内付费意愿的定价。

---

## 参考来源

[1] Andreessen Horowitz Leads $160M Investment in Harvey（Harvey 官方博客，2025-12-04）- https://www.harvey.ai/blog/andreessen-horowitz-leads-dollar160m-investment-in-harvey

[2] Harvey Raises $300M Series E Co-led by Kleiner Perkins and Coatue（Harvey 官方博客，2025-06-23）- https://www.harvey.ai/blog/harvey-raises-series-e

[3] Harvey raises $300 million at $5 billion valuation（Fortune，2025-06-23）- https://fortune.com/2025/06/23/harvey-raises-300-million-at-5-billion-valuation-to-be-legal-ai-for-lawyers-worldwide/

[4] Harvey raises $160m at $8bn valuation + launches Shared Spaces（Legal IT Insider，2025-12-04）- https://legaltechnology.com/2025/12/04/harvey-raises-160m-at-8bn-valuation-launches-shared-spaces-interview/

[5] Harvey 公司页：2400+ 客户、70+ 国家（Harvey 官网，2026-09 更新）- https://www.harvey.ai/company

[6] CoCounsel Legal 产品页（Thomson Reuters，2025-12 更新）- https://legal.thomsonreuters.com/en/products/cocounsel-legal

[7] Casetext AI Is Gone: How Its Technology Now Powers Thomson Reuters' CoCounsel（CapisTech，2026-07-27）- https://capistech.net/casetext-ai-cocounsel-thomson-reuters/

[8] CoCounsel 定价演变（UsagePricing，2026-06 更新）- https://www.usagepricing.com/blueprint/cocounsel

[9] Westlaw 套餐定价页（Thomson Reuters，2025-12 更新）- https://legal.thomsonreuters.com/en/c/westlaw/plans-and-pricing

[10] CoCounsel and Westlaw Advantage / Deep Research（AI Pro Playbook，2026-08）- https://aiproplaybook.com/tools/cocounsel

[11] Lexis+ with Protégé 产品页（LexisNexis UK，2026-09 更新）- https://www.lexisnexis.co.uk/products/lexis-plus-protege

[12] LexisNexis Citation Agent / 模型自选（LexisNexis Canada 公告）- https://www.lexisnexis.co.uk/solutions/legal-ai.html

[13] FTC Finalizes Order with DoNotPay（EIN Presswire，2025-02-12）- https://www.einpresswire.com/article/785165788/ftc-finalizes-order-with-donotpay

[14] FTC Fines DoNotPay Over Misleading 'Robot Lawyer' Claims（Slashdot，2025-02-11）- https://tech.slashdot.org/story/25/02/11/1932223/

[15] DoNotPay Alternatives 2026 / FTC 案细节（AI Lawyer，2026-09 更新）- https://ailawyer.pro/blog/donotpay-alternatives

[16] Spellbook raises $50M Series B led by Khosla Ventures（BetaKit，2025-10-09）- https://betakit.com/spellbook-raises-50-million-usd-series-b-led-by-khosla-ventures/

[17] Spellbook 公司数据：ARR/客户/估值（Sacra，2026-09 更新）- https://sacra.com/c/spellbook/

[18] Spellbook Teardown：ARR/客户/定价（OpenAIToolsHub，2026-05）- https://www.openaitoolshub.org/ai-product-research/spellbook

[19] Legora $150M Series C at $1.8B valuation（Legora 官方博客，2025-10-30）- https://legora.com/blog/series-c

[20] Legora 公司数据（Sacra，2026-09 更新）- https://sacra.com/c/legora/

[21] EvenUp Series E / 估值 20 亿（Sacra，2026-09 更新）- https://sacra.com/c/evenup/

[22] EvenUp 融资历程（AI Wiki，2026-07 更新）- https://aiwiki.ai/wiki/evenup

[23] Robin AI 融资历程（AI Wiki，2026-08 更新）- https://aiwiki.ai/wiki/robin_ai/edit

[24] APAC AI LegalTech: Robin/SpotDraft/Spellbook 对比（Amafi Advisory，2026-04-23）- https://amafiadvisory.com/industries/ai-legal/apac-ai-legal-players-2026

[25] SpotDraft Secures $54M Series B（SpotDraft 官方，2025-02-12）- https://www.spotdraft.com/blog/spotdraft-secures-54-million-to-lead-ai-contract-lifecycle-management

[26] SpotDraft Secures $8M from Qualcomm Ventures（Business Wire，2026-01-26）- https://www.businesswire.com/news/home/20260126696119/en/

[27] Luminance $75M Series C（Parsers VC 汇总，2025-02）- https://parsers.vc/startup/spotdraft.com/

[28] Due Diligence AI Comparison：Kira/Luminance/Eigen（AI Wiki，2026-06-05）- https://www.artificial-intelligence-wiki.com/industry-ai/ai-in-legal-services/due-diligence-ai-comparison/

[29] Hebbia raises $130M Series B led by a16z（Hebbia 官网）- https://www.hebbia.com/

[30] Microsoft Copilot vs ChatGPT Enterprise for Law Firms（AI Vortex，2026-04-29）- https://www.aivortex.io/legal/compare/microsoft-copilot-vs-chatgpt-enterprise-law-firms/

[31] Loyens & Loeff 部署 M365 Copilot 1600 人案例（Microsoft，2026-01-05）- https://www.microsoft.com/en/customers/story/26450-loyens-and-loeff-microsoft-defender-for-cloud

[32] Anthropic pays authors $1.5 billion to settle copyright lawsuit（AP News，2025-09-05）- https://apnews.com/article/anthropic-copyright-authors-settlement-training-f294266bc79a16ec90d2ddccdf435164

[33] Harvey 技术与客户：fine-tuned GPT-4 + Lexis 合作（AI Wiki / AI Pulled，2026 更新）- https://aipulled.com/news/llms-in-law-harvey-spellbook-accuracy.html

[34] Legal AI Market 2026: Who Owns What（AI Vortex，2026-04-17）- https://www.aivortex.io/legal/guides/legal-ai-market-2026-landscape
