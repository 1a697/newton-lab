<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>牛顿环实验综合平台</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Segoe UI", "Microsoft YaHei", sans-serif;
        }

        :root {
            --main-color: #4169E1;
            --light-color: #f0f5ff;
            --dark-color: #1a2035;
            --accent: #ff7b00;
            --text: #333;
            --shadow: 0 8px 32px rgba(0,0,0,0.15);
            --radius: 16px;
            --transition: all 0.3s ease;
        }

        body {
            overflow-x: hidden;
            color: var(--text);
        }

        .page {
            display: none;
            min-height: 100vh;
            width: 100%;
            padding: 2rem;
        }
        .page.active {
            display: block;
        }

        /* 首页 */
        #home {
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: #fff;
            text-align: center;
            overflow: hidden;
            background: #050818;
        }
        .bg-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: -1;
        }
        .home-wrap {
            animation: fadeUp 1s ease-out;
        }
        @keyframes fadeUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .home-title {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1.2rem;
            text-shadow: 0 0 20px rgba(100,150,255,0.6);
        }
        .home-subtitle {
            font-size: 1.4rem;
            color: #b8c8f0;
            margin-bottom: 1rem;
        }
        .home-desc {
            font-size: 1.2rem;
            opacity: 0.9;
            margin-bottom: 4rem;
            max-width: 750px;
            line-height: 1.8;
        }
        .btn-group-home {
            display: flex;
            gap: 2rem;
            flex-wrap: wrap;
            justify-content: center;
        }
        .main-btn {
            padding: 1.3rem 3rem;
            font-size: 1.15rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 600;
            min-width: 220px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            color: #fff;
        }
        .btn-theory {
            background: linear-gradient(135deg, #36d1dc 0%, #5b86e5 100%);
        }
        .btn-demo {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        .btn-calc {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
        }
        .main-btn:hover {
            transform: translateY(-8px) scale(1.03);
            box-shadow: 0 12px 30px rgba(0,0,0,0.3);
        }

        /* 导航栏 */
        .nav-bar {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background: #fff;
            padding: 1rem 2rem;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            margin-bottom: 2rem;
        }
        .nav-title {
            font-size: 1.5rem;
            font-weight: 600;
            color: var(--main-color);
        }
        .back-btn {
            padding: 0.6rem 1.5rem;
            background: var(--main-color);
            color: #fff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
        }
        .back-btn:hover {
            background: #3057c4;
        }

        /* 原理页 */
        #theory {
            background: var(--light-color);
        }
        .theory-container {
            max-width: 900px;
            margin: 0 auto;
            background: #fff;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            padding: 2rem;
            line-height: 1.8;
        }
        .theory-section {
            margin-bottom: 2rem;
        }
        .theory-section h3 {
            color: var(--main-color);
            margin-bottom: 1rem;
            font-size: 1.3rem;
            border-left: 4px solid var(--main-color);
            padding-left: 10px;
        }
        .formula-box {
            background: #f0f5ff;
            padding: 1rem;
            border-radius: 8px;
            margin: 1rem 0;
            text-align: center;
            font-size: 1.2rem;
        }
        .step-list {
            background: #e8f4ff;
            padding: 1rem 1.5rem;
            border-radius: 8px;
            line-height: 2;
        }
        .warning-list {
            background: #fff5f5;
            padding: 1rem;
            border-radius: 8px;
            border-left: 4px solid #ff7b00;
        }

        /* 演示页（光路图 + 放大牛顿环） */
        #demo {
            background: #0f1424;
        }
        .demo-container {
            display: grid;
            grid-template-columns: 3fr 1fr;
            gap: 1.5rem;
            max-width: 1400px;
            margin: 0 auto;
        }
        .light-path-view {
            background: rgba(0,0,0,0.4);
            border-radius: var(--radius);
            padding: 1rem;
        }
        .light-path-canvas {
            width: 100%;
            height: 600px;
            background: #0a1022;
            border-radius: 12px;
        }
        .right-panel {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }
        .ring-view-card {
            background: #fff;
            border-radius: var(--radius);
            padding: 1rem;
            text-align: center;
        }
        .ring-title {
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .ring-canvas {
            width: 100%;
            height: 260px;
            border-radius: 50%;
            background: #fff;
        }
        .control-card {
            background: #fff;
            border-radius: var(--radius);
            padding: 1.5rem;
        }
        .control-title {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }
        .slider-item {
            margin-bottom: 1rem;
        }
        .slider-item label {
            display: block;
            margin-bottom: 0.5rem;
        }
        input[type="range"] {
            width: 100%;
            height: 6px;
            accent-color: var(--main-color);
        }
        .mode-group {
            display: flex;
            gap: 0.5rem;
            margin-top: 0.5rem;
        }
        .mode-btn {
            flex: 1;
            padding: 0.6rem;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }
        .mode-btn.active {
            background: var(--main-color);
            color: #fff;
        }
        .reset-btn {
            width: 100%;
            padding: 0.8rem;
            background: var(--accent);
            color: #fff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 1rem;
        }
        /* 计算页 */
        #calc {
            background: var(--light-color);
        }
        .calc-container {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 2rem;
        }
        .input-card {
            background: #fff;
            border-radius: var(--radius);
            padding: 1.5rem;
        }
        .input-item {
            margin-bottom: 1rem;
        }
        .input-item label {
            display: block;
            margin-bottom: 0.5rem;
        }
        .input-item input {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 8px;
        }
        .calc-btn {
            width: 100%;
            padding: 0.9rem;
            background: var(--main-color);
            color: #fff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
        }
        .result-area {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }
        .result-card {
            background: #fff;
            border-radius: var(--radius);
            padding: 1.5rem;
        }
        .result-title {
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }
        .result-content {
            line-height: 2;
            background: #f8f9ff;
            padding: 1rem;
            border-radius: 8px;
            white-space: pre-wrap;
        }
        .chart-wrap {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
        }
        .chart-card {
            background: #fff;
            border-radius: var(--radius);
            padding: 1rem;
            min-height: 280px;
        }

        @media (max-width: 900px) {
            .demo-container, .calc-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

<!-- 首页 -->
<div id="home" class="page active">
    <canvas class="bg-canvas" id="bgCanvas"></canvas>
    <div class="home-wrap">
        <h1 class="home-title">牛顿环实验平台</h1>
        <p class="home-subtitle">等厚干涉 · 物理仿真实验系统</p>
        <p class="home-desc">观察牛顿环干涉现象，自动计算曲率半径、不确定度与误差</p>
        <div class="btn-group-home">
            <button class="main-btn btn-theory" onclick="switchPage('theory')">📚 实验原理与注意事项</button>
            <button class="main-btn btn-demo" onclick="switchPage('demo')">🔬 仪器动画演示</button>
            <button class="main-btn btn-calc" onclick="switchPage('calc')">📊 数据计算分析</button>
        </div>
    </div>
</div>

<!-- 原理页（公式修复 + 实验步骤） -->
<div id="theory" class="page">
    <div class="nav-bar">
        <div class="nav-title">实验原理与注意事项</div>
        <button class="back-btn" onclick="switchPage('home')">返回首页</button>
    </div>
    <div class="theory-container">
        <div class="theory-section">
            <h3>一、实验原理</h3>
            <p>牛顿环是由光的等厚干涉产生的。平凸透镜与平板玻璃之间形成空气薄膜，入射光在上下表面反射后发生干涉，形成同心圆环。</p>
            <div class="formula-box">
                曲率半径公式：<br>
                R = (Dₘ² - Dₙ²) / [4λ(m-n)]
            </div>
            <p>λ = 589.3 nm（钠黄光波长）</p>
        </div>

        <div class="theory-section">
            <h3>二、实验步骤（完整版）</h3>
            <div class="step-list">
                1. 打开实验仪器，调节钠光灯与读数显微镜，使视场明亮均匀。<br>
                2. 调节显微镜焦距，使牛顿环清晰，中心暗斑位于视场中央。<br>
                3. 调节十字叉丝方向与显微镜移动方向平行。<br>
                4. 从第15级暗环开始，单向移动显微镜，依次测量各级暗环左右坐标。<br>
                5. 计算各级暗环直径 D = |x右 - x左|。<br>
                6. 使用逐差法处理数据，计算透镜曲率半径 R。<br>
                7. 计算不确定度，完成实验数据处理与误差分析。
            </div>
        </div>

        <div class="theory-section">
            <h3>三、注意事项</h3>
            <div class="warning-list">
                <ul>
                    <li>测量时显微镜必须单向移动，禁止回程误差。</li>
                    <li>中心暗斑不测量，从第5级以上环纹开始测量。</li>
                    <li>保持光学元件清洁，无灰尘、指纹。</li>
                    <li>数据处理必须使用逐差法，提高精度。</li>
                </ul>
            </div>
        </div>
    </div>
</div>

<!-- 演示页（光路图 + 放大牛顿环） -->
<div id="demo" class="page">
    <div class="nav-bar">
        <div class="nav-title">牛顿环实验仪器仿真演示</div>
        <button class="back-btn" onclick="switchPage('home')">返回首页</button>
    </div>
    <div class="demo-container">
        <div class="light-path-view">
            <canvas class="light-path-canvas" id="lightPathCanvas"></canvas>
        </div>
        <div class="right-panel">
            <div class="ring-view-card">
                <div class="ring-title">🔬 放大牛顿环图样</div>
                <canvas class="ring-canvas" id="ringCanvas"></canvas>
            </div>
            <div class="control-card">
                <h3 class="control-title">实验参数调节</h3>
                <div class="slider-item">
                    <label>光源模式</label>
                    <div class="mode-group">
                        <button class="mode-btn active" id="whiteBtn">白光干涉</button>
                        <button class="mode-btn" id="monoBtn">单色光</button>
                    </div>
                </div>
                <div class="slider-item">
                    <label>光强：<span id="iVal">1.00</span></label>
                    <input type="range" id="iSlider" min="0.2" max="2" step="0.01" value="1">
                </div>
                <div class="slider-item">
                    <label>曲率半径 R：<span id="rVal">1.00</span> m</label>
                    <input type="range" id="rSlider" min="0.2" max="3" step="0.01" value="1">
                </div>
                <button class="reset-btn" onclick="resetDemo()">重置参数</button>
            </div>
        </div>
    </div>
</div>

<!-- 计算页 -->
<div id="calc" class="page">
    <div class="nav-bar">
        <div class="nav-title">实验数据计算 & 不确定度分析</div>
        <button class="back-btn" onclick="switchPage('home')">返回首页</button>
    </div>
    <div class="calc-container">
        <div class="input-card">
            <h3 class="control-title">实验数据录入</h3>
            <div class="input-item">
                <label>暗环级数 k</label>
                <input type="text" id="kInput" value="10 11 12 13 14 15 16 17 18 19">
            </div>
            <div class="input-item">
                <label>暗环直径 Dk (mm)</label>
                <input type="text" id="dInput" value="5.632 5.786 5.935 6.081 6.225 6.366 6.505 6.641 6.775 6.907">
            </div>
            <div class="input-item">
                <label>仪器误差 Δ仪 (mm)</label>
                <input type="text" id="errInput" value="0.004">
            </div>
            <button class="calc-btn" onclick="doCalculate()">开始计算</button>
        </div>
        <div class="result-area">
            <div class="result-card">
                <h3 class="result-title">计算结果</h3>
                <div class="result-content" id="calcResult">请输入数据后点击计算</div>
            </div>
            <div class="chart-wrap">
                <div class="chart-card"><canvas id="c1"></canvas></div>
                <div class="chart-card"><canvas id="c2"></canvas></div>
                <div class="chart-card"><canvas id="c3"></canvas></div>
                <div class="chart-card"><canvas id="c4"></canvas></div>
            </div>
        </div>
    </div>
</div>

<script>
    // 页面切换
    function switchPage(id) {
        document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
        document.getElementById(id).classList.add('active');
        if (id === 'demo') {
            initDemo();
            drawLightPath();
            drawRing();
        }
    }

    const LAMBDA = 589.3e-9;
    let charts = []; // 存储所有图表实例，用于销毁
    let demo = { R:1, I:1, white:true };

    // 首页背景
    const bg = document.getElementById('bgCanvas');
    const bgCtx = bg.getContext('2d');
    function resize() { bg.width=innerWidth; bg.height=innerHeight; }
    window.addEventListener('resize', resize);
    resize();

    function drawBg() {
        const w=bg.width, h=bg.height;
        bgCtx.clearRect(0,0,w,h);
        for(let i=40;i>0;i--){
            let r=Math.sqrt(i*LAMBDA*1e3)*800;
            bgCtx.beginPath();
            bgCtx.arc(w/2,h/2,r,0,Math.PI*2);
            bgCtx.strokeStyle=`hsla(${(i/40)*360},100%,65%,0.6)`;
            bgCtx.lineWidth=4;
            bgCtx.stroke();
        }
        requestAnimationFrame(drawBg);
    }
    drawBg();

    // 演示页：光路图 + 放大牛顿环
    let pathCtx, ringCtx;
    function initDemo() {
        const pathC = document.getElementById('lightPathCanvas');
        const ringC = document.getElementById('ringCanvas');
        pathCtx = pathC.getContext('2d');
        ringCtx = ringC.getContext('2d');
        pathC.width = pathC.offsetWidth;
        pathC.height = pathC.offsetHeight;
        ringC.width = 260;
        ringC.height = 260;
    }

    // 绘制牛顿环光路图
    function drawLightPath() {
        if(!document.getElementById('demo').classList.contains('active')) {
            requestAnimationFrame(drawLightPath);
            return;
        }
        const W=pathCtx.canvas.width, H=pathCtx.canvas.height;
        pathCtx.clearRect(0,0,W,H);

        // 底板
        pathCtx.fillStyle='#333';
        pathCtx.fillRect(0.1*W,0.8*H,0.8*W,0.1*H);
        // 平板玻璃
        pathCtx.fillStyle='#a0c4ff';
        pathCtx.fillRect(0.2*W,0.75*H,0.6*W,0.04*H);
        // 平凸透镜
        pathCtx.fillStyle='rgba(180,220,255,0.6)';
        pathCtx.beginPath();
        pathCtx.ellipse(0.5*W,0.65*H,0.25*W,0.12*H,0,0,Math.PI);
        pathCtx.fill();
        // 光路
        pathCtx.strokeStyle='#ff0';
        pathCtx.lineWidth=2;
        pathCtx.setLineDash([5,5]);
        pathCtx.beginPath();
        pathCtx.moveTo(0.5*W,0.1*H);
        pathCtx.lineTo(0.5*W,0.75*H);
        pathCtx.stroke();
        pathCtx.setLineDash([]);

        // 牛顿环（光路图内）
        for(let i=40;i>0;i--){
            let r=Math.sqrt(i*LAMBDA*demo.R)*4000;
            pathCtx.beginPath();
            pathCtx.arc(0.5*W,0.75*H,r,0,Math.PI*2);
            pathCtx.lineWidth=4*demo.I;
            pathCtx.strokeStyle=demo.white?`hsla(${(i/40)*360},100%,60%,${demo.I})`:`rgba(255,230,100,${Math.abs(Math.cos(i*Math.PI))*demo.I})`;
            pathCtx.stroke();
        }
        requestAnimationFrame(drawLightPath);
    }

    // 放大牛顿环
    function drawRing() {
        const W=260, H=260;
        ringCtx.clearRect(0,0,W,H);
        for(let i=45;i>0;i--){
            let r=Math.sqrt(i*LAMBDA*demo.R)*5000;
            if(r>120) continue;
            ringCtx.beginPath();
            ringCtx.arc(130,130,r,0,Math.PI*2);
            ringCtx.lineWidth=5*demo.I;
            ringCtx.strokeStyle=demo.white?`hsla(${(i/45)*360},100%,60%,${demo.I})`:`rgba(255,220,80,${Math.abs(Math.cos(i*Math.PI))*demo.I})`;
            ringCtx.stroke();
        }
    }

    // 交互
    const iSlider=document.getElementById('iSlider');
    const rSlider=document.getElementById('rSlider');
    const iVal=document.getElementById('iVal');
    const rVal=document.getElementById('rVal');
    iSlider.oninput=e=>{ demo.I=+e.target.value; iVal.textContent=demo.I.toFixed(2); drawRing(); };
    rSlider.oninput=e=>{ demo.R=+e.target.value; rVal.textContent=demo.R.toFixed(2); drawRing(); };
    document.getElementById('whiteBtn').onclick=()=>{ demo.white=true; drawRing(); };
    document.getElementById('monoBtn').onclick=()=>{ demo.white=false; drawRing(); };
    function resetDemo(){ demo={R:1,I:1,white:true}; iSlider.value=1; rSlider.value=1; iVal.textContent="1.00"; rVal.textContent="1.00"; drawRing(); }

    // 数学工具函数
    function mean(a){ return a.reduce((s,x)=>s+x,0)/a.length; }
    function std(a){ let m=mean(a); return Math.sqrt(mean(a.map(x=>(x-m)**2))); }
    // 最小二乘拟合 y=kx+b
    function linearFit(xArr,yArr){
        const n = xArr.length;
        let sumX=0,sumY=0,sumXY=0,sumXX=0;
        for(let i=0;i<n;i++){
            sumX += xArr[i];
            sumY += yArr[i];
            sumXY += xArr[i]*yArr[i];
            sumXX += xArr[i]*xArr[i];
        }
        const k = (n*sumXY - sumX*sumY) / (n*sumXX - sumX*sumX);
        const b = (sumY - k*sumX)/n;
        // 计算R²
        const yAvg = mean(yArr);
        let ssTot=0,ssRes=0;
        for(let i=0;i<n;i++){
            const yFit = k*xArr[i]+b;
            ssTot += (yArr[i]-yAvg)**2;
            ssRes += (yArr[i]-yFit)**2;
        }
        const r2 = 1 - ssRes/ssTot;
        return {k,b,r2};
    }

    // 计算主函数 + 绘图（新增库加载检测）
    function doCalculate(){
        // 检测Chart.js是否加载
        if (typeof Chart === 'undefined') {
            document.getElementById('calcResult').textContent = "❌ 错误：图表库Chart.js加载失败，请联网后重试";
            return;
        }

        // 销毁旧图表，防止重叠
        charts.forEach(c=>c.destroy());
        charts = [];

        let k=document.getElementById('kInput').value.split(/\s+/).map(Number);
        let d=document.getElementById('dInput').value.split(/\s+/).map(Number);
        let err=+document.getElementById('errInput').value;
        const D2 = d.map(v=>v*v);
        let n=Math.floor(k.length/2);
        let Rlist=[];
        for(let i=0;i<n;i++){
            let dm=d[i+n], dn=d[i];
            Rlist.push((dm**2-dn**2)*1e-6/(4*LAMBDA*(k[i+n]-k[i])));
        }
        let Ravg=mean(Rlist);
        let ua=std(Rlist)/Math.sqrt(n);
        let ub=err*1e-3/Math.sqrt(3);
        let ur=Math.hypot(ua,ub);
        let relErr = ur/Ravg*100;

        // 最小二乘拟合 D² = k*m + b
        const fit = linearFit(k,D2);
        const fitY = k.map(m=>fit.k*m + fit.b);

        // 输出文字结果
        let s=`==== 牛顿环实验计算结果 ====
波长 λ = 589.3 nm
仪器误差 = ${err.toFixed(4)} mm
最小二乘拟合斜率 k = ${fit.k.toFixed(4)} mm²
决定系数 R² = ${fit.r2.toFixed(6)}

逐差分组计算曲率半径：
${Rlist.map((v,i)=>`第${i+1}组 R = ${v.toFixed(4)} m`).join('\n')}

平均曲率半径 R = ${Ravg.toFixed(4)} m
A类不确定度 ua = ${ua.toFixed(4)} m
B类不确定度 ub = ${ub.toFixed(5)} m
合成不确定度 uR = ${ur.toFixed(4)} m
相对不确定度 = ${relErr.toFixed(2)} %

最终结果：R = ${Ravg.toFixed(4)} ± ${ur.toFixed(4)} m`;
        document.getElementById('calcResult').textContent=s;

        // 图表1：D² - m 散点+拟合直线（核心最小二乘图）
        const ctx1 = document.getElementById('c1').getContext('2d');
        const chart1 = new Chart(ctx1,{
            type:'scatter',
            data:{
                datasets:[
                    {label:'实验数据 D²-m',data:k.map((val,i)=>({x:val,y:D2[i]})),pointRadius:6,backgroundColor:'#4169E1'},
                    {label:'拟合直线',type:'line',data:k.map((val,i)=>({x:val,y:fitY[i]})),borderColor:'#ff7b00',borderWidth:2,pointRadius:0}
                ]
            },
            options:{responsive:true,maintainAspectRatio:false,plugins:{title:{display:true,text:`D²-m 线性拟合 R²=${fit.r2.toFixed(4)}`}},scales:{x:{title:{display:true,text:'级数 m'}},y:{title:{display:true,text:'D² (mm²)'}}}}
        });
        charts.push(chart1);

        // 图表2：各组逐差R柱状图
        const ctx2 = document.getElementById('c2').getContext('2d');
        const chart2 = new Chart(ctx2,{
            type:'bar',
            data:{labels:Rlist.map((_,i)=>`组${i+1}`),datasets:[{label:'各组R值(m)',data:Rlist,backgroundColor:'#36d1dc'}]},
            options:{responsive:true,maintainAspectRatio:false,plugins:{title:{display:true,text:'逐差分组曲率半径'}}}
        });
        charts.push(chart2);

        // 图表3：直径D随级数变化曲线
        const ctx3 = document.getElementById('c3').getContext('2d');
        const chart3 = new Chart(ctx3,{
            type:'line',
            data:{labels:k,datasets:[{label:'暗环直径D(mm)',data:d,borderColor:'#764ba2',fill:false}]},
            options:{responsive:true,maintainAspectRatio:false,plugins:{title:{display:true,text:'D-k 变化曲线'}}}
        });
        charts.push(chart3);

        // 图表4：残差分布图（D²实测 - D²拟合）
        const residual = D2.map((val,i)=>val-fitY[i]);
        const ctx4 = document.getElementById('c4').getContext('2d');
        const chart4 = new Chart(ctx4,{
            type:'bar',
            data:{labels:k,datasets:[{label:'拟合残差',data:residual,backgroundColor:'#f5576c'}]},
            options:{responsive:true,maintainAspectRatio:false,plugins:{title:{display:true,text:'拟合残差分布'}}}
        });
        charts.push(chart4);
    }

    // 自动执行首页
    switchPage('home');
</script>
</body>
</html>
