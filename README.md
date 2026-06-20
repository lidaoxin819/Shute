<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>李道鑫 · 简历 — 方案C 科技紫黑</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@300;400;500;600;700&display=swap');
  *{margin:0;padding:0;box-sizing:border-box}
  body{font-family:'Noto Sans SC',sans-serif;background:#0e0e16;color:#e0e0f0;font-size:13px;line-height:1.6}
  .page{max-width:880px;margin:30px auto;background:#12121e;box-shadow:0 0 60px rgba(120,80,255,.15);min-height:1100px;display:flex;flex-direction:column}
  /* HEADER */
  .header{background:linear-gradient(135deg,#1a1232 0%,#0e1a3a 100%);padding:32px 48px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid rgba(120,80,255,.3);position:relative;overflow:hidden}
  .header::before{content:'';position:absolute;top:-40px;right:-40px;width:180px;height:180px;background:radial-gradient(circle,rgba(120,80,255,.2),transparent 70%);pointer-events:none}
  .header::after{content:'';position:absolute;bottom:-30px;left:200px;width:120px;height:120px;background:radial-gradient(circle,rgba(0,200,255,.1),transparent 70%);pointer-events:none}
  .h-left{display:flex;flex-direction:column;gap:6px;z-index:1}
  .h-name{font-size:32px;font-weight:700;color:#fff;letter-spacing:4px}
  .h-role{font-size:12px;color:#9080d0;letter-spacing:2px}
  .h-tags{display:flex;gap:6px;margin-top:4px}
  .h-tag{background:rgba(120,80,255,.2);border:1px solid rgba(120,80,255,.4);border-radius:12px;padding:2px 10px;font-size:11px;color:#b0a0ff}
  .h-right{display:flex;flex-direction:column;gap:5px;z-index:1;text-align:right}
  .h-contact{font-size:12px;color:#a0a0c0}
  .h-contact span{color:#7060d0}
  /* METRICS BAR */
  .metrics-bar{background:#0d0d1a;border-bottom:1px solid rgba(120,80,255,.2);padding:16px 48px;display:flex;justify-content:space-around}
  .m-item{text-align:center;flex:1;position:relative}
  .m-item:not(:last-child)::after{content:'';position:absolute;right:0;top:20%;height:60%;width:1px;background:rgba(120,80,255,.2)}
  .m-num{font-size:22px;font-weight:700;background:linear-gradient(90deg,#8060ff,#00c8ff);-webkit-background-clip:text;-webkit-text-fill-color:transparent;display:block}
  .m-label{font-size:10.5px;color:#7060a0;letter-spacing:.5px}
  /* BODY */
  .body{display:flex;flex:1;gap:0}
  /* LEFT */
  .left{width:260px;border-right:1px solid rgba(120,80,255,.15);padding:28px 22px;display:flex;flex-direction:column;gap:24px;flex-shrink:0}
  .s-sect{display:flex;flex-direction:column;gap:8px}
  .s-ttl{font-size:10px;font-weight:700;letter-spacing:2.5px;color:#7060d0;padding-bottom:6px;border-bottom:1px solid rgba(120,80,255,.2);display:flex;align-items:center;gap:6px}
  .s-ttl::before{content:'';width:3px;height:3px;background:#8060ff;border-radius:50%;display:inline-block}
  .adv-card{background:rgba(120,80,255,.06);border:1px solid rgba(120,80,255,.15);border-radius:5px;padding:7px 10px;font-size:11.5px;color:#b0a8d8;line-height:1.5}
  .tag-cloud{display:flex;flex-wrap:wrap;gap:4px}
  .tech-tag{background:rgba(0,200,255,.06);border:1px solid rgba(0,200,255,.2);border-radius:3px;padding:2px 7px;font-size:10.5px;color:#60c8ff}
  .cert-tag{background:rgba(120,80,255,.08);border:1px solid rgba(120,80,255,.25);border-radius:3px;padding:2px 7px;font-size:10.5px;color:#a090e8}
  /* RIGHT */
  .right{flex:1;padding:28px 28px;display:flex;flex-direction:column;gap:22px}
  .r-sect{display:flex;flex-direction:column;gap:10px}
  .r-head{display:flex;align-items:center;gap:8px;margin-bottom:2px}
  .r-title{font-size:12.5px;font-weight:700;color:#c0b8e8;letter-spacing:1.5px}
  .r-line{flex:1;height:1px;background:linear-gradient(90deg,rgba(120,80,255,.4),transparent)}
  .summary-p{font-size:12.5px;color:#a0a0c0;line-height:1.85;border-left:2px solid #7060d0;padding-left:12px}
  .summary-p strong{color:#d0c8ff}
  /* EXP */
  .exp-item{border:1px solid rgba(120,80,255,.15);border-radius:8px;padding:13px 15px;background:rgba(120,80,255,.03);display:flex;flex-direction:column;gap:5px;position:relative;overflow:hidden}
  .exp-item::before{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:linear-gradient(180deg,#8060ff,#0090ff)}
  .exp-top{display:flex;justify-content:space-between;align-items:flex-start}
  .ec{font-size:13px;font-weight:700;color:#e0d8ff}
  .er{font-size:11.5px;color:#8060d0;font-weight:600;margin-top:2px}
  .es{font-size:11px;color:#6060a0}
  .edate{font-size:10px;background:rgba(120,80,255,.2);border:1px solid rgba(120,80,255,.3);border-radius:10px;padding:2px 8px;color:#b0a0ff;white-space:nowrap}
  .b-list{margin-top:4px;display:flex;flex-direction:column;gap:3px}
  .b-list li{list-style:none;font-size:12px;color:#a0a0c0;padding-left:13px;position:relative;line-height:1.65}
  .b-list li::before{content:'›';position:absolute;left:0;color:#6050d0;font-size:14px;top:-1px}
  .hl{color:#c0b0ff;font-weight:600}
  /* SKILLS */
  .sk-grid{display:grid;grid-template-columns:1fr 1fr;gap:7px}
  .sk-card{background:rgba(120,80,255,.05);border:1px solid rgba(120,80,255,.15);border-radius:5px;padding:8px 10px}
  .sk-cat{font-size:10px;font-weight:700;color:#7060d0;letter-spacing:1px;margin-bottom:3px}
  .sk-val{font-size:11.5px;color:#9090c0;line-height:1.6}
  .edu-row{background:rgba(120,80,255,.04);border:1px solid rgba(120,80,255,.15);border-radius:6px;padding:10px 14px;display:flex;justify-content:space-between;align-items:center}
  .edu-s{font-size:13px;font-weight:700;color:#d0c8ff}
  .edu-m{font-size:11.5px;color:#7060a0;margin-top:2px}
  .edu-d{font-size:11px;color:#6060a0}
</style>
</head>
<body>
<div class="page">
  <!-- HEADER -->
  <div class="header">
    <div class="h-left">
      <div class="h-name">李道鑫</div>
      <div class="h-role">AI HARDWARE PRODUCT MANAGER</div>
      <div class="h-tags">
        <span class="h-tag">AI 硬件</span>
        <span class="h-tag">消费电子</span>
        <span class="h-tag">项目经理</span>
      </div>
    </div>
    <div class="h-right">
      <div class="h-contact"><span>📱</span> 193-1008-8784</div>
      <div class="h-contact"><span>✉</span> rinck668@163.com</div>
      <div class="h-contact"><span>📍</span> 山东德州 · 26岁</div>
    </div>
  </div>

  <!-- METRICS BAR -->
  <div class="metrics-bar">
    <div class="m-item"><span class="m-num">8+</span><div class="m-label">消费电子新品上市</div></div>
    <div class="m-item"><span class="m-num">10万+</span><div class="m-label">累计产品销量</div></div>
    <div class="m-item"><span class="m-num">100万+</span><div class="m-label">爆款首月销售额</div></div>
    <div class="m-item"><span class="m-num">千万级</span><div class="m-label">生命周期GMV</div></div>
    <div class="m-item"><span class="m-num">99%</span><div class="m-label">京东自营好评率</div></div>
  </div>

  <!-- BODY -->
  <div class="body">
    <!-- LEFT COLUMN -->
    <div class="left">
      <div class="s-sect">
        <div class="s-ttl">个人优势</div>
        <div class="adv-card">4年AI智能硬件完整0→1经验</div>
        <div class="adv-card">跨部门10人+团队管理能力</div>
        <div class="adv-card">用户洞察 × 数据驱动迭代</div>
        <div class="adv-card">海外市场适配 × 多认证体系</div>
        <div class="adv-card">公众号运营，11万+爆款文章</div>
      </div>

      <div class="s-sect">
        <div class="s-ttl">产品工具</div>
        <div class="tag-cloud">
          <span class="tech-tag">Axure</span><span class="tech-tag">墨刀</span>
          <span class="tech-tag">Visio</span><span class="tech-tag">XMind</span>
          <span class="tech-tag">Excel</span><span class="tech-tag">PRD</span>
        </div>
      </div>

      <div class="s-sect">
        <div class="s-ttl">认证资质</div>
        <div class="tag-cloud">
          <span class="cert-tag">CE</span><span class="cert-tag">FCC</span>
          <span class="cert-tag">CCC</span><span class="cert-tag">SRRC</span>
        </div>
      </div>

      <div class="s-sect">
        <div class="s-ttl">产品品类</div>
        <div class="tag-cloud">
          <span class="tech-tag">AI录音卡</span><span class="tech-tag">翻译耳机</span>
          <span class="tech-tag">学习机</span><span class="tech-tag">智能音响</span>
          <span class="tech-tag">会议系统</span>
        </div>
      </div>

      <div class="s-sect">
        <div class="s-ttl">目标市场</div>
        <div class="tag-cloud">
          <span class="cert-tag">北美</span><span class="cert-tag">欧洲</span>
          <span class="cert-tag">日本</span><span class="cert-tag">英国</span><span class="cert-tag">国内</span>
        </div>
      </div>
    </div>

    <!-- RIGHT COLUMN -->
    <div class="right">
      <div class="r-sect">
        <div class="r-head">
          <div class="r-title">/ 职业概述</div>
          <div class="r-line"></div>
        </div>
        <div class="summary-p">具备 <strong>4年AI智能硬件与消费电子产品经验</strong>，完整主导多款产品0→1开发，覆盖AI录音卡、AI翻译耳机、智能音响、学习机、会议系统等品类。擅长产品规划、需求定义、APP协同开发与海外市场适配，曾主导爆款产品首月销售额突破 <strong>100万元</strong>，生命周期销售额达<strong>千万级</strong>。</div>
      </div>

      <div class="r-sect">
        <div class="r-head">
          <div class="r-title">/ 工作经历</div>
          <div class="r-line"></div>
        </div>

        <div class="exp-item">
          <div class="exp-top">
            <div>
              <div class="ec">上海韩创网络科技有限公司</div>
              <div class="er">AI 硬件产品经理</div>
            </div>
            <div class="edate">2026.05 — 至今</div>
          </div>
          <ul class="b-list">
            <li>AI录音卡功能规划与迭代，输出 PRD、原型设计及功能定义</li>
            <li>移动端 APP 迭代，覆盖设备管理、文件管理、AI 转写等模块</li>
            <li>追踪 AI Recorder、PLAUD 等行业竞品，持续竞品研究</li>
          </ul>
        </div>

        <div class="exp-item">
          <div class="exp-top">
            <div>
              <div class="ec">深圳市一呼百应科技有限公司</div>
              <div class="er">产品经理（兼项目经理）</div>
              <div class="es">AI录音卡 · AI翻译耳机 | 北美/欧洲/英国/日本</div>
            </div>
            <div class="edate">2026.01 — 2026.04</div>
          </div>
          <ul class="b-list">
            <li>录音卡二代试产上市，AI翻译耳机开发，完成 <span class="hl">CE/FCC/SRRC/CCC</span> 认证</li>
            <li>带屏录音卡：完成硬件规格、屏幕交互需求与方案规划</li>
            <li>APP <span class="hl">1.5个月</span>完成两个迭代版本，实时转写+AI分析+架构重构</li>
            <li>推进 <span class="hl">13国语言</span>本地化适配，完成产品权益与定价策略</li>
          </ul>
        </div>

        <div class="exp-item">
          <div class="exp-top">
            <div>
              <div class="ec">心喜阅信息咨询有限公司</div>
              <div class="er">产品经理</div>
              <div class="es">智能音响 · 点读笔 · 学习机 · 耳机 | 京东</div>
            </div>
            <div class="edate">2023.04 — 2025.03</div>
          </div>
          <ul class="b-list">
            <li>主导 <span class="hl">7款新产品</span> 0→1，<span class="hl">12周</span>内完成硬件量产</li>
            <li>核心产品 <span class="hl">首月破100万</span>，年出货10万+，总销售额千万级，Top 5</li>
            <li>京东好评率 <span class="hl">99%</span>，管理 <span class="hl">13人</span>团队</li>
          </ul>
        </div>

        <div class="exp-item">
          <div class="exp-top">
            <div>
              <div class="ec">广州保伦电子股份有限公司</div>
              <div class="er">产品专员</div>
              <div class="es">智能无线会议系统 | G端</div>
            </div>
            <div class="edate">2021.12 — 2022.12</div>
          </div>
          <ul class="b-list">
            <li>负责会议系统 V1.5–V2.5 功能迭代，完成会议议程、投票、多屏互动模块</li>
          </ul>
        </div>
      </div>

      <div class="r-sect">
        <div class="r-head">
          <div class="r-title">/ 专业技能</div>
          <div class="r-line"></div>
        </div>
        <div class="sk-grid">
          <div class="sk-card"><div class="sk-cat">产品工具</div><div class="sk-val">Axure · 墨刀 · Visio · XMind</div></div>
          <div class="sk-card"><div class="sk-cat">项目管理</div><div class="sk-val">敏捷 · OEM · 供应链 · 成本控制</div></div>
          <div class="sk-card"><div class="sk-cat">数据分析</div><div class="sk-val">Excel · 数据决策报告输出</div></div>
          <div class="sk-card"><div class="sk-cat">海外合规</div><div class="sk-val">CE · FCC · CCC · SRRC</div></div>
        </div>
      </div>

      <div class="r-sect">
        <div class="r-head">
          <div class="r-title">/ 教育经历</div>
          <div class="r-line"></div>
        </div>
        <div class="edu-row">
          <div><div class="edu-s">桂林旅游学院</div><div class="edu-m">本科 · 电子商务</div></div>
          <div class="edu-d">2018.09 — 2022.06</div>
        </div>
      </div>
    </div>
  </div>
</div>
</body>
</html>
