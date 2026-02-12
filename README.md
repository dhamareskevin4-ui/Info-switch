# Info-switch-KTI
<!DOCTYPE html>
<html>
<head>
  <title>Info Switch</title>
  <style>
    body {
      background: black;
      color: #00ffcc;
      font-family: Arial;
      text-align: center;
      padding-top: 50px;
    }
    .card {
      border: 2px solid #00ffcc;
      padding: 20px;
      margin: auto;
      width: 300px;
      border-radius: 10px;
      box-shadow: 0 0 20px #00ffcc;
    }
    button {
      padding: 10px;
      margin-top: 10px;
      background: #00ffcc;
      border: none;
      cursor: pointer;
      font-weight: bold;
    }
    button:hover{
      background:#00ccaa;
    }
  </style>
</head>
<body>

<div class="card">
  <h2>Switch Lt.2</h2>
  <p><b>IP:</b> 192.168.1.2</p>
  <p><b>Lokasi:</b> Ruang Server Lt.2</p>
  <p><b>Status:</b> Aktif</p>
  <button onclick="emailTech()">Hubungi Teknisi</button>
</div>

<script>
function emailTech(){
  const email = "teknisi@perusahaan.com";
  const subject = "Laporan Kerusakan Switch Lt.2";
  const body = "Halo teknisi,%0D%0ASwitch dengan IP 192.168.1.2 mengalami kendala.%0D%0ALokasi: Ruang Server Lt.2";

  window.location.href = `mailto:${email}?subject=${subject}&body=${body}`;
}
</script>

</body>
</html>
