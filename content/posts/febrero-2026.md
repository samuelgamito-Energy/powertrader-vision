---
title: "Informe Energético FEBRERO 2026"
date: 2026-03-01
author: "PowerTrader"
tags: ["informe", "mensual", "febrero", "2026"]
categories: ["EnergyVision"]
showToc: false
---

<style>
    :root {
        --bg: #080c14;
        --surface: #0d1420;
        --surface2: #111927;
        --border: rgba(255, 255, 255, 0.07);
        --accent: #00d4ff;
        --accent2: #7c3aed;
        --accent3: #10b981;
        --accent4: #f59e0b;
        --accent5: #ef4444;
        --text: #e2e8f0;
        --text-dim: #64748b;
        --text-muted: #94a3b8;
        --card-glow: 0 0 30px rgba(0, 212, 255, 0.06);
        --radius: 16px;
        --radius-sm: 10px;
    }

    /* Override PaperMod defaults for this post */
    .post-content {
        color: var(--text);
        background: var(--bg);
        font-family: 'Inter', sans-serif;
    }

    .header-inner {
        position: relative;
        z-index: 1;
        background: linear-gradient(135deg, #060b18 0%, #0d1a2e 50%, #060b18 100%);
        border-bottom: 1px solid var(--border);
        padding: 48px 60px 40px;
        border-radius: var(--radius);
        margin-bottom: 24px;
    }

    .header-badge {
        display: inline-flex;
        align-items: center;
        gap: 8px;
        background: rgba(0, 212, 255, 0.08);
        border: 1px solid rgba(0, 212, 255, 0.2);
        color: var(--accent);
        font-size: 11px;
        font-weight: 600;
        letter-spacing: 1.5px;
        text-transform: uppercase;
        padding: 6px 14px;
        border-radius: 100px;
        margin-bottom: 18px;
    }

    .header-inner h1 {
        font-size: 42px;
        font-weight: 800;
        line-height: 1.1;
        background: linear-gradient(135deg, #ffffff 0%, #94c7ff 50%, #00d4ff 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        margin-bottom: 10px;
        border: none !important;
    }

    .header-subtitle {
        font-size: 15px;
        color: var(--text-muted);
        font-weight: 400;
    }

    .header-meta {
        margin-top: 24px;
        display: flex;
        gap: 24px;
        flex-wrap: wrap;
    }

    .meta-pill {
        display: flex;
        align-items: center;
        gap: 7px;
        font-size: 12px;
        color: var(--text-dim);
    }

    .meta-pill span {
        color: var(--text-muted);
        font-weight: 500;
    }

    .section-title {
        font-size: 11px;
        font-weight: 700;
        letter-spacing: 2px;
        text-transform: uppercase;
        color: var(--accent);
        margin-top: 40px;
        margin-bottom: 20px;
        display: flex;
        align-items: center;
        gap: 10px;
    }

    .section-title::after {
        content: '';
        flex: 1;
        height: 1px;
        background: linear-gradient(90deg, rgba(0, 212, 255, 0.3), transparent);
    }

    .post-content h2 {
        font-size: 22px;
        font-weight: 700;
        margin-bottom: 6px;
        color: var(--text);
        border: none !important;
    }

    .section-head p {
        color: var(--text-muted);
        font-size: 13px;
        margin-bottom: 24px;
    }

    .kpi-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 16px;
        margin-bottom: 48px;
    }

    .kpi-card {
        background: var(--surface);
        border: 1px solid var(--border);
        border-radius: var(--radius);
        padding: 22px 24px;
        position: relative;
        overflow: hidden;
    }

    .kpi-label {
        font-size: 11px;
        font-weight: 600;
        letter-spacing: 1px;
        text-transform: uppercase;
        color: var(--text-dim);
        margin-bottom: 10px;
    }

    .kpi-value {
        font-size: 28px;
        font-weight: 800;
        font-family: monospace;
        color: var(--kpi-color, var(--accent));
        line-height: 1;
    }

    .kpi-unit {
        font-size: 13px;
        font-weight: 500;
        color: var(--text-muted);
        margin-top: 4px;
    }

    .kpi-trend {
        margin-top: 12px;
        font-size: 11px;
        display: flex;
        align-items: center;
        gap: 5px;
        color: var(--text-dim);
    }

    .kpi-trend.up { color: var(--accent3); }
    .kpi-trend.down { color: var(--accent5); }

    .chart-grid {
        display: grid;
        gap: 24px;
        margin-bottom: 48px;
    }

    .chart-grid-2 { grid-template-columns: 1fr 1fr; }
    .chart-grid-3 { grid-template-columns: 2fr 1fr; }

    .chart-card {
        background: var(--surface);
        border: 1px solid var(--border);
        border-radius: var(--radius);
        padding: 28px;
    }

    .chart-head {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        margin-bottom: 24px;
    }

    .chart-title { font-size: 15px; font-weight: 700; color: var(--text); }
    .chart-subtitle { font-size: 12px; color: var(--text-dim); margin-top: 2px; }

    .mix-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
        gap: 12px;
        margin-bottom: 48px;
    }

    .mix-card {
        background: var(--surface2);
        border: 1px solid var(--border);
        border-radius: var(--radius-sm);
        padding: 16px 18px;
        position: relative;
        overflow: hidden;
    }

    .table-wrap {
        background: var(--surface);
        border: 1px solid var(--border);
        border-radius: var(--radius);
        overflow-x: auto;
        margin-bottom: 48px;
    }

    table {
        width: 100%;
        border-collapse: collapse;
        font-size: 12px;
    }

    th {
        padding: 12px 14px;
        text-align: right;
        font-weight: 600;
        color: var(--text-dim);
        background: rgba(0, 212, 255, 0.05);
    }

    td {
        padding: 10px 14px;
        text-align: right;
        border-bottom: 1px solid rgba(255, 255, 255, 0.03);
        color: var(--text-muted);
    }

    .insights-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
        gap: 20px;
        margin-bottom: 48px;
    }

    .insight-card {
        background: var(--surface);
        border: 1px solid var(--border);
        border-radius: var(--radius);
        padding: 24px;
    }

    /* Mobile adjustments */
    @media (max-width: 900px) {
        .chart-grid-2, .chart-grid-3 { grid-template-columns: 1fr; }
        .header-inner h1 { font-size: 28px; }
    }
</style>

<div class="header-inner">
    <div class="header-badge">⚡ Power Trader · EnergyVision</div>
    <h1>Informe Energético FEBRERO 2026</h1>
    <p class="header-subtitle">Análisis de mercado eléctrico peninsular español · Datos mensuales automáticos</p>
    <div class="header-meta">
        <div class="meta-pill">📅 Período: <span>01 FEB – 28 FEB 2026</span></div>
        <div class="meta-pill">📊 Registros: <span>28 días</span></div>
        <div class="meta-pill">🔌 Fuente: <span>OMIE / REE</span></div>
        <div class="meta-pill">📈 Actualizado: <span>01 mar 2026</span></div>
    </div>
</div>

<div class="section-title">Indicadores Clave del Período</div>
<div class="kpi-grid" id="kpi-grid"></div>

<div class="section-head">
    <div class="section-title">Precios de Mercado</div>
    <h2>Evolución OMIE Spot & PVPC</h2>
    <p>Variación diaria del precio en el mercado mayorista (OMIE) y precio regulado (PVPC) durante el mes</p>
</div>
<div class="chart-grid">
    <div class="chart-card">
        <div class="chart-head">
            <div>
                <div class="chart-title">Precios Diarios — OMIE Spot vs PVPC</div>
                <div class="chart-subtitle">€/MWh · Valores diarios</div>
            </div>
        </div>
        <div class="chart-wrapper"><canvas id="chartPrecios" height="100"></canvas></div>
    </div>
</div>

<div class="section-head">
    <div class="section-title">Demanda & Balances</div>
    <h2>Demanda y Saldos de Red</h2>
</div>
<div class="chart-grid chart-grid-2">
    <div class="chart-card">
        <div class="chart-title">Demanda Diaria</div>
        <div class="chart-wrapper"><canvas id="chartDemanda" height="150"></canvas></div>
    </div>
    <div class="chart-card">
        <div class="chart-title">Saldo Interconexiones</div>
        <div class="chart-wrapper"><canvas id="chartSaldo" height="150"></canvas></div>
    </div>
</div>

<div class="section-head">
    <div class="section-title">Mix de Generación</div>
    <h2>Estructura de la Generación Eléctrica</h2>
</div>
<div class="chart-grid chart-grid-3">
    <div class="chart-card">
        <div class="chart-title">Generación por Tecnología</div>
        <div class="chart-wrapper"><canvas id="chartGenStack" height="140"></canvas></div>
    </div>
    <div class="chart-card">
        <div class="chart-title">Distribución Total</div>
        <div class="chart-wrapper"><canvas id="chartDonut" height="200"></canvas></div>
    </div>
</div>

<div class="section-head">
    <div class="section-title">Energías Renovables</div>
    <h2>Solar y Eólica — Evolución Diaria</h2>
</div>
<div class="chart-grid">
    <div class="chart-card">
        <div class="chart-wrapper"><canvas id="chartRenovables" height="90"></canvas></div>
    </div>
</div>

<div class="section-head">
    <div class="section-title">Resumen por Fuente</div>
    <h2>Generación Total Acumulada</h2>
</div>
<div class="mix-grid" id="mix-grid"></div>

<div class="section-head">
    <div class="section-title">Almacenamiento & Flexibilidad</div>
    <h2>Baterías & Bombeo Hidráulico</h2>
</div>
<div class="chart-grid chart-grid-2">
    <div class="chart-card">
        <div class="chart-title">Consumo Bombeo</div>
        <div class="chart-wrapper"><canvas id="chartBombeo" height="160"></canvas></div>
    </div>
    <div class="chart-card">
        <div class="chart-title">Baterías (Carga/Entrega)</div>
        <div class="chart-wrapper"><canvas id="chartBaterias" height="160"></canvas></div>
    </div>
</div>

<div class="section-head">
    <div class="section-title">Tabla de Datos</div>
    <h2>Resumen Estadístico</h2>
</div>
<div class="table-wrap">
    <table id="summary-table"></table>
</div>

<div class="section-head">
    <div class="section-title">Análisis & Conclusiones</div>
    <h2>Insights del Período</h2>
</div>
<div class="insights-grid" id="insights-grid"></div>

<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
<script>
    (function() {
        const data = JSON.parse('{\x22omie\x22:[24.575625000000002,13.834062500000002,32.74177083333334,17.219479166666662,6.303854166666665,9.391874999999999,6.854791666666666,5.924270833333334,20.951041666666658,4.6946875,4.227916666666666,5.701249999999999,4.4163541666666655,2.1300000000000003,1.5535416666666668,4.40125,26.781875,18.243749999999995,14.870208333333332,28.382083333333338,29.105416666666674,22.210208333333338,34.8246875,28.246458333333333,29.904270833333342,27.380833333333353,20.100729166666667,14.501458333333332],\x22demanda\x22:[635767.1749999998,759383.7250000001,776846.94,792490.1590000001,768020.583,749766.2000000001,672508.45,631825.1,749234.5500000002,746909,738462.063,722698.1249999999,730471.5449999998,638637.3,608187.542,718782.275,718409.418,724752.825,719541.859,718859.7600000002,633408.615,585948.8749999999,688190.799,699738.7500000001,701358.3489999999,695069.282,692432.9020000001,606349.5430000001],\x22saldo\x22:[-11410.925000000001,-21522.1,-15908.55,-26179.474999999995,-30016.349999999995,-35285.825000000004,-40293.299999999996,-45356.57500000001,-31161.575,-29263.125,-29599.524999999994,-40539.7,-27288.375,-57673.17499999998,-72484.45,-54867.45,-71406.275,-75494.75,-83172.075,-64363.225,-12966.175,-8510.724999999999,18242.574999999997,807.9500000000023,15158.824999999999,26124.35,9684.674999999996,-48771.32499999999],\x22baleares\x22:[-3650,-4572.6,-4533,-4762,-4660.125,-4459,-3696,-3231.8,-4071.4,-4014,-4035.6,-3334.6,-4043.6,-3443.6,-3076,-3867,-3506.2,-3479.8,-3467.6,-3372.6,-3254.2,-3143.5,-3371.65,-3394.2,-3420,-3473,-3464,-3213],\x22bombeo\x22:[-34688.799999999996,-45559.57499999999,-33680.175,-36764.85,-47822.183000000005,-41550.675,-40055.775,-41276.4,-30827.775,-37591.125,-28677.4,-32470.15,-29947.1,-36833.15,-38799.825,-34194.700000000004,-27249.649999999998,-30368.024999999994,-31572.483,-26602.25,-35936.775,-33458,-28386.15000000001,-25147.850000000006,-24566.950000000008,-24283.774999999998,-29828.675,-35798.175],\x22cargaBat\x22:[-199,-196,-280,-66,-11,-254,-472,-11,-487,-259,-459,-206,-201,-12,-5,-206,-226,-322,-106,-15,-181,-33,-2,-153,-361,-88,-5,-318],\x22entregaBat\x22:[0,2,40,36,28,0,0,0,8,0,0,0,56,1,0,15,28,144,2,12,8,0,2,36,108,23,1,15],\x22hibrid\x22:[1962.4999999999998,5137.35,4010.9,4135.799999999999,4283.650000000001,4061.5250000000005,3344.9250000000006,2568.1499999999996,3376.2999999999997,5377.875,4960.075,3446.3,5052.149999999999,3508.7999999999997,2899.6750000000006,4172.075,3419.375,4649.775,4201.75,4071.0499999999997,1925.1579999999997,1158.5249999999999,2184.5,2466.9249999999997,3189.1749999999997,3013.95,3380.4499999999994,3932.5000000000005],\x22pvpc\x22:[92.41583333333334,126.38458333333335,129.16624999999996,120.08708333333334,120.27583333333332,117.96666666666665,73.65249999999999,77.96125,128.19958333333332,117.64999999999999,120.4995833333333,122.2183333333333,119.69083333333333,81.61375,86.51041666666664,125.77041666666666,137.52208333333334,126.18749999999999,127.49000000000001,136.0533333333333,98.80749999999999,103.61,143.36708333333334,136.94291666666666,143.6575,139.37000000000003,136.95624999999998,95.37333333333333],\x22nuclear\x22:[160790.975,160785.30000000002,170112.47500000003,170110.72499999998,164616.42500000005,152235.82499999998,151853.65000000002,145211.95000000004,137708.35,137641.30000000002,137387.79999999996,138055.25000000003,137691.04999999996,137529.92500000005,137651.65000000005,137662,137729.6,132700.67500000002,130834.22499999998,134355.375,137885.70000000004,137690.77500000005,138058.44999999995,137781.8,138024.87499999997,137733.42500000002,136246.19999999995,136189.87500000006],\x22hidUGH\x22:[138875.925,135428.65,153253.77499999997,157394.77500000002,162076.45,161795.05000000002,176381.875,169920.4,173459.29999999996,142889.45,125546.067,116318.3,117996.39999999998,104815.475,94151.19999999998,100783.09999999999,141835.92500000002,133905.95,127727.1,151298.17500000002,154108.95100000003,137528.75,153271.31600000002,154975.6,151747.55000000002,138814.45,136414.376,125872.6],\x22hidNoUGH\x22:[21746.824999999993,22222.025,23913.35,24550.500000000004,22249.800000000003,21649.85,21186.700000000004,19252.975,20584.15,21455.525,21676.318999999996,20201.45,22264.875,19402.575,19343.650000000005,20252.249999999996,23237.649999999998,23975.6,22232.149999999998,24792.45,25810.925000000003,24339.600000000002,25150.100000000002,24642.625,25239.150000000005,25278.749999999993,24457.75,21947.925000000003],\x22turbBom\x22:[18981.875,16753.55,21038.350000000002,15932.6,12186.591999999999,15593.825,18947.275,17704.45,15390.125,11679.600000000002,13607.1,15268.65,13387.675000000001,14874.875000000002,9998.35,12590.775000000001,13792.95,15457.5,10402.949999999999,15672.460000000001,12625.784,11185.225,15325.900000000001,18088.500000000004,13313.275,13831.407,12641.925,12359.849999999999],\x22ccomb\x22:[67169.92499999999,64891.77500000001,77255.69999999998,65552.02500000001,63253.850000000006,54648.075000000004,50179.225000000006,50014.20000000002,66084.67499999999,55420.45,57507.1,59289.77500000001,52721.57499999999,60172.200000000004,66973.84999999999,68438.34999999999,80623.375,65158.525000000016,74163.30000000002,83991.45,76539.875,82756.40000000001,94802.15000000001,84492.025,99069.166,88469.82500000001,82738.97500000002,73095.34999999999],\x22eolica\x22:[191031.25000000003,325021.47500000003,270000.055,349228.692,331619.799,313032.35,259845.8,216478.65,299755.2,369433.5249999999,363375.402,320842.85000000003,334721.353,270087.95,261399.325,358891.49999999994,261239.943,309995.89999999997,305599.075,196875.4,60595.99799999999,36410.67500000001,38916.70800000001,96135.275,90381.62499999999,72285.625,117600.91799999999,119755.268],\x22cogen\x22:[22196.075,22260.225000000002,24249.160000000003,22785.100000000006,19954.074999999997,20001.2,19271.65,18852.875,22169.65,20494.850000000002,19449.075000000004,20068.774999999994,19312.341999999997,16471.100000000002,16550.9,18048.15,23063.425,23520.575000000004,22706.725,26507.2,24564.675,23605.574999999997,25759.2,25952.750000000004,27367.374999999993,27419.924999999996,24950.075000000004,21618.2],\x22residuos\x22:[3184.8250000000003,3218.6,3094.35,2324.425,2414.75,3009.4749999999995,4027.975000000001,3669.8749999999995,3644.25,3269.775,3740.6499999999996,3462.9750000000004,3327.5,3634.1249999999995,3421.3000000000006,3327.4999999999995,3210.874999999999,3348.525,3699.475,3728.475,3489.925,3305.150000000001,3317.5750000000003,3634.3500000000004,4051.875,4015.85,3964.9749999999995,4201.525000000001],\x22otrasRen\x22:[9196.875,10284.6,10410.25,10887.117000000002,9552.800000000001,8774.974999999999,7635.125,7632.925000000002,7966.325,8026.799999999999,7342.900000000001,6586.625000000001,6771.55,5872.975,6042.542,6220.050000000001,6673.449999999998,7795.050000000001,8033.141999999999,8758.249999999998,8616.974,8069.549999999999,9816.325,10936.35,10948.483,10929.225000000002,10655.524999999998,11014.374999999998],\x22solarFV\x22:[45955.15,61564.025,76684.54999999999,38429.925,59812.09999999999,76529.7,43902.025,68574.27500000002,64891.62499999999,43725.249999999985,45641.97499999999,99896.2,74970.62499999999,98223.375,97266.44999999998,82831.89999999998,120926.775,106652.125,125104.94999999998,150695.875,156817.05000000002,143599.19999999998,173233.05,148686.92500000002,137169.95,153558.95,145891.083,145105.85],\x22solarTerm\x22:[632.75,305.825,633.575,228.97499999999997,441.79999999999995,844.6,158.475,518.675,354.4,515.5,593.55,2125.625,497.9750000000001,6509.124999999998,7479.65,1731.4,4009.2999999999993,2414.275,8711.275000000001,12565.500000000002,13873.225000000002,14740.849999999997,14902.249999999998,13362.875000000002,7870.775,13398.125,10070.474999999999,12526.7]}');
        const labels = Array.from({ length: 28 }, (_, i) => String(i + 1).padStart(2, '0'));

        const sum = arr => arr.reduce((a, b) => a + b, 0);
        const avg = arr => sum(arr) / arr.length;
        const min = arr => Math.min(...arr);
        const max = arr => Math.max(...arr);
        const fmt = (n, d = 0) => n.toLocaleString('es-ES', { minimumFractionDigits: d, maximumFractionDigits: d });

        Chart.defaults.color = '#64748b';
        Chart.defaults.borderColor = 'rgba(255,255,255,0.05)';

        // Simple helper for cards
        const kpiGrid = document.getElementById('kpi-grid');
        const kpis = [
            { label: 'Precio Medio OMIE', value: fmt(avg(data.omie), 2), unit: '€/MWh', color: '#00d4ff' },
            { label: 'Precio Medio PVPC', value: fmt(avg(data.pvpc), 2), unit: '€/MWh', color: '#7c3aed' },
            { label: 'Demanda Media', value: fmt(avg(data.demanda) / 1000, 1), unit: 'GWh/día', color: '#f59e0b' },
            { label: 'Eólica Total', value: fmt(sum(data.eolica) / 1000, 0), unit: 'GWh', color: '#10b981' },
            { label: 'Solar FV Total', value: fmt(sum(data.solarFV) / 1000, 0), unit: 'GWh', color: '#f59e0b' }
        ];

        kpis.forEach(k => {
            kpiGrid.innerHTML += `
                <div class="kpi-card" style="--kpi-color:${k.color}">
                    <div class="kpi-label">${k.label}</div>
                    <div class="kpi-value">${k.value}</div>
                    <div class="kpi-unit">${k.unit}</div>
                </div>`;
        });

        // Charts initialization
        const baseOptions = { responsive: true, plugins: { legend: { display: false } } };

        new Chart(document.getElementById('chartPrecios'), {
            type: 'line',
            data: {
                labels,
                datasets: [
                    { label: 'PVPC', data: data.pvpc, borderColor: '#7c3aed', tension: 0.4 },
                    { label: 'OMIE', data: data.omie, borderColor: '#00d4ff', tension: 0.4 }
                ]
            },
            options: baseOptions
        });

        new Chart(document.getElementById('chartDemanda'), {
            type: 'line',
            data: {
                labels,
                datasets: [{ label: 'Demanda', data: data.demanda.map(v => v / 1000), borderColor: '#f59e0b', tension: 0.4, fill: true }]
            },
            options: baseOptions
        });

        new Chart(document.getElementById('chartSaldo'), {
            type: 'bar',
            data: {
                labels,
                datasets: [{ label: 'Saldo', data: data.saldo.map(v => v / 1000), backgroundColor: data.saldo.map(v => v > 0 ? '#10b981' : '#ef4444') }]
            },
            options: baseOptions
        });

        new Chart(document.getElementById('chartDonut'), {
            type: 'doughnut',
            data: {
                labels: ['Eólica', 'Solar FV', 'Nuclear', 'Hidro', 'C.Comb.', 'Otros'],
                datasets: [{
                    data: [sum(data.eolica), sum(data.solarFV), sum(data.nuclear), sum(data.hidUGH), sum(data.ccomb), sum(data.cogen)],
                    backgroundColor: ['#10b981', '#f59e0b', '#6366f1', '#00d4ff', '#ef4444', '#fbbf24']
                }]
            },
            options: { responsive: true, plugins: { legend: { position: 'bottom' } } }
        });

        new Chart(document.getElementById('chartRenovables'), {
            type: 'line',
            data: {
                labels,
                datasets: [
                    { label: 'Eólica', data: data.eolica.map(v => v / 1000), borderColor: '#10b981', tension: 0.4 },
                    { label: 'Solar FV', data: data.solarFV.map(v => v / 1000), borderColor: '#f59e0b', tension: 0.4 },
                    { label: 'Hidro', data: data.hidUGH.map(v => v / 1000), borderColor: '#00d4ff', tension: 0.4 }
                ]
            },
            options: baseOptions
        });

        // Insights and Mixed Grid logic would go here, simplified for now
        const mixGrid = document.getElementById('mix-grid');
        const sources = [
            { name: 'Eólica', total: sum(data.eolica), color: '#10b981' },
            { name: 'Solar FV', total: sum(data.solarFV), color: '#f59e0b' },
            { name: 'Nuclear', total: sum(data.nuclear), color: '#6366f1' },
            { name: 'Ciclo Comb.', total: sum(data.ccomb), color: '#ef4444' }
        ];

        sources.forEach(s => {
            mixGrid.innerHTML += `
                <div class="mix-card">
                    <div class="mix-src" style="color:${s.color}">${s.name}</div>
                    <div class="mix-total">${fmt(s.total/1000, 0)} GWh</div>
                </div>`;
        });

        // Summary Table
        const tbl = document.getElementById('summary-table');
        tbl.innerHTML = `<thead><tr><th>Variable</th><th>Mín</th><th>Máx</th><th>Media</th></tr></thead>
            <tbody>
                <tr><td>OMIE (€/MWh)</td><td>${fmt(min(data.omie),2)}</td><td>${fmt(max(data.omie),2)}</td><td>${fmt(avg(data.omie),2)}</td></tr>
                <tr><td>PVPC (€/MWh)</td><td>${fmt(min(data.pvpc),2)}</td><td>${fmt(max(data.pvpc),2)}</td><td>${fmt(avg(data.pvpc),2)}</td></tr>
                <tr><td>Demanda (GWh)</td><td>${fmt(min(data.demanda)/1000,0)}</td><td>${fmt(max(data.demanda)/1000,0)}</td><td>${fmt(avg(data.demanda)/1000,0)}</td></tr>
            </tbody>`;
            
        // Final Insights
        const insGrid = document.getElementById('insights-grid');
        const insights = [
            { icon: '📉', title: 'Precios Bajos', text: `El mercado marcó mínimos de ${fmt(min(data.omie),2)} €/MWh.` },
            { icon: '⚡', title: 'Renovables', text: `La suma de Eólica+Solar+Hidro cubrió una parte fundamental de la demanda.` },
            { icon: '🔋', title: 'Almacenamiento', text: `Actividad intensa de bombeo y baterías en horas de precios valle.` }
        ];

        insights.forEach(i => {
            insGrid.innerHTML += `
                <div class="insight-card">
                    <div class="insight-icon">${i.icon}</div>
                    <div class="insight-title">${i.title}</div>
                    <div class="insight-text">${i.text}</div>
                </div>`;
        });
    })();
</script>
