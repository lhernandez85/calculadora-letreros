<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
  <meta name="theme-color" content="#1e293b">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <title>Cotizador Letreros</title>
  <style>
    * { box-sizing: border-box; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; margin: 0; padding: 0; }
    body { background: #0f172a; color: #f8fafc; padding: 18px; display: flex; justify-content: center; min-height: 100vh; }
    .card { background: #1e293b; width: 100%; max-width: 430px; border-radius: 18px; padding: 22px; box-shadow: 0 10px 30px rgba(0,0,0,0.5); border: 1px solid #334155; }
    h1 { font-size: 1.35rem; font-weight: 700; margin-bottom: 18px; text-align: center; color: #38bdf8; letter-spacing: -0.5px; }
    .unit-selector { display: flex; background: #0f172a; border-radius: 10px; padding: 4px; margin-bottom: 18px; border: 1px solid #334155; }
    .unit-selector button { flex: 1; border: none; background: transparent; color: #94a3b8; padding: 9px; border-radius: 8px; font-weight: 600; cursor: pointer; transition: all 0.2s; font-size: 0.9rem; }
    .unit-selector button.active { background: #38bdf8; color: #0f172a; }
    .field { margin-bottom: 14px; }
    label { display: block; font-size: 0.85rem; color: #94a3b8; margin-bottom: 6px; font-weight: 500; }
    input { width: 100%; background: #0f172a; border: 1px solid #334155; border-radius: 10px; color: #fff; padding: 12px; font-size: 1.05rem; outline: none; transition: border-color 0.2s; }
    input:focus { border-color: #38bdf8; }
    .grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
    .results { margin-top: 18px; background: #0f172a; border-radius: 12px; padding: 16px; border: 1px solid #334155; }
    .res-row { display: flex; justify-content: space-between; align-items: center; padding: 8px 0; border-bottom: 1px solid #1e293b; font-size: 0.95rem; }
    .res-row:last-child { border-bottom: none; }
    .res-row.highlight { font-size: 1.25rem; font-weight: 700; color: #4ade80; padding-top: 10px; margin-top: 4px; border-top: 1px solid #334155; }
    .area-badge { font-weight: 700; color: #38bdf8; }
    
    .actions { display: flex; flex-direction: column; gap: 10px; margin-top: 18px; }
    .btn-wsp { background: #25d366; color: #0b2914; border: none; border-radius: 10px; padding: 13px; font-size: 1rem; font-weight: 700; display: flex; align-items: center; justify-content: center; gap: 8px; cursor: pointer; transition: opacity 0.2s; }
    .btn-wsp:active { opacity: 0.85; }
    .btn-wsp svg { width: 20px; height: 20px; fill: currentColor; }
    .btn-clean { background: transparent; border: 1px solid #475569; color: #94a3b8; padding: 10px; border-radius: 10px; font-weight: 600; cursor: pointer; }
    .btn-clean:active { background: #334155; }
  </style>
</head>
<body>

<div class="card">
  <h1>Calculadora de Letreros</h1>

  <div class="unit-selector">
    <button id="btnM" class="active" onclick="setUnit('m')">Metros (m)</button>
    <button id="btnCm" onclick="setUnit('cm')">Centímetros (cm)</button>
  </div>

  <div class="grid">
    <div class="field">
      <label id="lblAncho" for="ancho">Ancho (m)</label>
      <input type="number" id="ancho" placeholder="Ej: 2.0" step="any" inputmode="decimal" oninput="calcular()">
    </div>
    <div class="field">
      <label id="lblAlto" for="alto">Alto (m)</label>
      <input type="number" id="alto" placeholder="Ej: 1.0" step="any" inputmode="decimal" oninput="calcular()">
    </div>
  </div>

  <div class="grid">
    <div class="field">
      <label for="cantidad">Cantidad</label>
      <input type="number" id="cantidad" value="1" min="1" step="1" inputmode="numeric" oninput="calcular()">
    </div>
    <div class="field">
      <label for="precio">Valor m² ($)</label>
      <input type="number" id="precio" placeholder="Ej: 18000" step="any" inputmode="numeric" oninput="calcular()">
    </div>
  </div>

  <div class="results">
    <div class="res-row">
      <span>Superficie total</span>
      <span class="area-badge" id="resArea">0.00 m²</span>
    </div>
    <div class="res-row">
      <span>Neto</span>
      <span id="resNeto">$0</span>
    </div>
    <div class="res-row">
      <span>IVA (19%)</span>
      <span id="resIva">$0</span>
    </div>
    <div class="res-row highlight">
      <span>Total</span>
      <span id="resTotal">$0</span>
    </div>
  </div>

  <div class="actions">
    <button class="btn-wsp" onclick="enviarWhatsApp()">
      <svg viewBox="0 0 24 24">
        <path d="M12.031 2C6.5 2 2 6.5 2 12.031c0 1.954.562 3.844 1.625 5.469L2 22l4.656-1.594A10.01 10.01 0 0 0 12.03 22c5.531 0 10.031-4.5 10.031-10.031S17.562 2 12.031 2zm0 18.25c-1.688 0-3.344-.469-4.781-1.344l-.344-.219-2.781.938.938-2.688-.219-.344a8.21 8.21 0 0 1-1.344-4.562c0-4.562 3.719-8.281 8.281-8.281 4.562 0 8.281 3.719 8.281 8.281 0 4.562-3.719 8.281-8.281 8.281zm4.531-6.188c-.25-.125-1.469-.719-1.688-.812-.219-.094-.375-.125-.531.125-.156.25-.625.812-.781.969-.125.156-.281.188-.531.062s-1.062-.391-2.031-1.25a7.73 7.73 0 0 1-1.406-1.75c-.156-.25 0-.406.125-.531.094-.125.219-.312.344-.469.094-.156.125-.25.188-.406.062-.156.031-.312-.031-.438-.062-.125-.531-1.281-.719-1.75-.188-.469-.375-.406-.531-.406h-.438c-.156 0-.438.062-.656.312-.219.25-.844.812-.844 2 0 1.188.875 2.344 1 2.5.125.156 1.719 2.625 4.156 3.688.594.25 1.062.406 1.438.531.625.188 1.188.156 1.625.094.5-.062 1.469-.594 1.688-1.188.219-.594.219-1.094.156-1.188-.062-.094-.219-.156-.469-.281z"/>
      </svg>
      Compartir por WhatsApp
    </button>
    <button class="btn-clean" onclick="limpiar()">Limpiar campos</button>
  </div>
</div>

<script>
  let currentUnit = 'm';

  function setUnit(unit) {
    currentUnit = unit;
    document.getElementById('btnM').className = unit === 'm' ? 'active' : '';
    document.getElementById('btnCm').className = unit === 'cm' ? 'active' : '';
    document.getElementById('lblAncho').textContent = `Ancho (${unit})`;
    document.getElementById('lblAlto').textContent = `Alto (${unit})`;
    calcular();
  }

  function formatMoney(num) {
    return '$' + Math.round(num).toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".");
  }

  function getCalculatedData() {
    let w = parseFloat(document.getElementById('ancho').value) || 0;
    let h = parseFloat(document.getElementById('alto').value) || 0;
    let cant = parseInt(document.getElementById('cantidad').value) || 1;
    if (cant < 1) cant = 1;

    const precio = parseFloat(document.getElementById('precio').value) || 0;

    const wM = currentUnit === 'cm' ? w / 100 : w;
    const hM = currentUnit === 'cm' ? h / 100 : h;

    const areaUnitaria = wM * hM;
    const areaTotal = areaUnitaria * cant;
    const neto = areaTotal * precio;
    const iva = neto * 0.19;
    const total = neto + iva;

    return { w, h, wM, hM, unit: currentUnit, cant, precio, areaUnitaria, areaTotal, neto, iva, total };
  }

  function calcular() {
    const data = getCalculatedData();

    if (data.cant > 1) {
      document.getElementById('resArea').textContent = `${data.areaTotal.toFixed(2)} m² (${data.areaUnitaria.toFixed(2)} m² c/u)`;
    } else {
      document.getElementById('resArea').textContent = `${data.areaTotal.toFixed(2)} m²`;
    }

    document.getElementById('resNeto').textContent = formatMoney(data.neto);
    document.getElementById('resIva').textContent = formatMoney(data.iva);
    document.getElementById('resTotal').textContent = formatMoney(data.total);
  }

  function limpiar() {
    document.getElementById('ancho').value = '';
    document.getElementById('alto').value = '';
    document.getElementById('cantidad').value = '1';
    document.getElementById('precio').value = '';
    calcular();
  }

  function enviarWhatsApp() {
    const data = getCalculatedData();

    if (data.total <= 0) {
      alert("Por favor ingresa las medidas y el valor antes de compartir.");
      return;
    }

    const detalleCantidad = data.cant > 1 ? `\n• Cantidad: ${data.cant} unidades\n• Sup. total: ${data.areaTotal.toFixed(2)} m²` : '';

    const mensaje = 
`*COTIZACIÓN DE LETRERO*
--------------------------------
• Medidas: ${data.w} x ${data.h} ${data.unit}
• Superficie c/u: ${data.areaUnitaria.toFixed(2)} m²${detalleCantidad}
• Valor m²: ${formatMoney(data.precio)}
--------------------------------
• *Neto:* ${formatMoney(data.neto)}
• *IVA (19%):* ${formatMoney(data.iva)}
• *TOTAL:* ${formatMoney(data.total)}
--------------------------------
Quedamos atentos a cualquier consulta.`;

    const url = `https://api.whatsapp.com/send?text=${encodeURIComponent(mensaje)}`;
    window.open(url, '_blank');
  }
</script>

</body>
</html>
