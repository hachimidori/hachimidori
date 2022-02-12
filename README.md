
<!DOCTYPE html>
<html>
<head>
<title>Status Hotspot</title>

	<meta http-equiv="refresh" content="60">

	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta content='RingRoad' name='Author' />
<link rel="shortcut icon" type="image/png" href="favicon.png"/>
<link rel="stylesheet" href="css/style.css">
<script type="text/javascript" src="js/custom.js"></script>
<script language="JavaScript">

    function openLogout() {
	if (window.name != 'hotspot_status') return true;
        open('http://kampung.net/logout', 'hotspot_logout', 'toolbar=0,location=0,directories=0,status=0,menubars=0,resizable=1,width=280,height=250');
	window.close();
	return false;
    }

</script>
</head>
<body  >
<main> 
  <div id="header" class="bck-green">
    <div class="header-background-elements">
      <div class="header-circle circle-left"></div>  
      <div class="header-circle circle-right"></div> 
      
      <div class="dashed-shapes">
        <div class="dashed-shape shape-1"></div>
        <div class="dashed-shape shape-2"></div>
        <div class="dashed-shape shape-3"></div>
      </div>
      
      <div class="clouds">
        <div class="cloud-circle circle-1"></div>
        <div class="cloud-circle circle-2"></div>
        <div class="cloud-circle circle-3"></div>
        <div class="cloud-circle circle-4"></div>
        <div class="cloud-circle circle-5"></div>
        <div class="cloud-circle circle-6"></div>
      </div>
    </div>
     <div class="header-menu">
       <div class="u-white"><h4 class="h4" id="WelcomeMessage"></h4></div>
    </div>
    
    <div class="header-user-info">
       <div class="user-picture">
	   <i style="font-size:70px;background: #31708F;border-radius: 50%;margin-top: -10px;" class="icon icon-user-circle-o">&#xf2be;</i>  
	   </div>
      <div class="user-name">
	  
	  <h4 id="user" class="h4" style="margin-top:10px">zycs79</h4>
	  
	  </div>
    </div>
  </div>
<div class="profile-section">
<div class="box" style="padding-top: 10px;">
<span style="background:rgba(0,0,0,0.5);border-radius:3px;padding:10px;color:#fff;">Terhubung <i class="icon icon-globe">&#xe812;</i> : <span id="Terhubung"></span></span>
</div>
<table class="table no-border" style="text-align: center;">
    <tbody>
        <tr>
            <td style="padding-bottom: 0px;">
                <p style="font-size:12px;margin-bottom:0px;"><i class="icon icon-download">&#xe809;</i> Download</p>
            </td>
            <td style="padding-bottom: 0px;">
                <p style="font-size:12px;margin-bottom:0px;"><i class="icon icon-upload">&#xe80a;</i> Upload</p>
            </td>
        </tr>
        <tr>
            <td style="padding-top: 0px;">
                <p style="font-size:18px;margin:0;">189.1 MiB </p>
            </td>
            <td style="padding-top: 0px;">
                <p style="font-size:18px;margin:0;">21.2 MiB </p>
            </td>
        </tr>
    </tbody>
</table>
<table class="table2">
	<tr><td align="right" style="width: 40%;">IP <i class="icon icon-sitemap">&#xf0e8;</i> </td><td>10.10.10.148</td></tr>
    <tr><td align="right">MAC <i class="icon icon-qrcode">&#xe814;</i> </td><td><span id="macAddr">04:D9:F5:4C:73:01</span></td></tr>

    <tr><td align="right">Sisa Kuota <i class="icon icon-battery-3">&#xf241;</i> </td><td>689.5 MiB</td></tr>


	<tr><td align="right">Refresh <i class="icon icon-arrows-cw">&#xe811;</i> </td><td>1m</td></tr>


    <tr><td align="right">Sisa Waktu <i class="icon icon-clock">&#xe80f;</i> </td><td><span id="SisaWaktu"></span></td></tr>


	<tr><td align="right">Expired <i class="icon icon-hourglass-2">&#xf252;</i> </td><td style="padding-top:0px; padding-left:0px;"><iframe id="exp" frameborder="0" scrolling="no" src="about:blank"></iframe></td></tr>

	</table>
	<br />
<form action="http://kampung.net/logout" name="logout" onSubmit="return openLogout()">
<input type="hidden" name="erase-cookie" value="on">

<p style="font-size:10px; text-align:center;margin:5px auto;">Tombol <b>LOG OFF</b> dapat menghentikan akses internet</p>
<button class="btn btn-full btn-merah" type="submit"> <i class="icon icon-off">&#xe813;</i> LOG OFF</button>

</form>
<br />
<div class="box">
<a style="color:#333;" href="http://ringroad.net">Made with <i class="icon icon-heart" style="color:red">&#xe800;</i> for you</a>
</div>
</div>
</main>
<script type="text/javascript">
//get validity
    var usr = document.getElementById('user').innerHTML
    var url = "http://192.168.150.150/status/status.php?name="; // http://ip-server-mikhmon/mikhmonv2/status/status.php?name=
    var SessionName = "RB450G"
    var getvalid = url+usr+"&session="+SessionName
    document.getElementById('exp').src = getvalid;
</script>
<script>
var time = "3h3m42s";
time = time.replace(/w/g,'w ').replace(/d/g,'d ').replace(/h/g,'h ').replace(/m/g,'m ').replace(/s/g,'s ');
waktu = time.replace(/w /g,'Minggu').replace(/d /g,'Hari').replace(/h /g,'Jam').replace(/m /g,'Menit').replace(/s /g,'Detik');
sisawaktu = waktu.replace(/Minggu/g,'Minggu ').replace(/Hari/g,'Hari ').replace(/Jam/g,'Jam ').replace(/Menit/g,'Menit ').replace(/Detik/g,'Detik ');

document.getElementById("SisaWaktu").innerHTML = sisawaktu;  
</script>
<script>
var conn = "1h56m18s";
conn = conn.replace(/w/g,'w ').replace(/d/g,'d ').replace(/h/g,'h ').replace(/m/g,'m ').replace(/s/g,'s ');
Connect = conn.replace(/w /g,'Minggu').replace(/d /g,'Hari').replace(/h /g,'Jam').replace(/m /g,'Menit').replace(/s /g,'Detik');
TimeConnect = Connect.replace(/Minggu/g,'Minggu ').replace(/Hari/g,'Hari ').replace(/Jam/g,'Jam ').replace(/Menit/g,'Menit ').replace(/Detik/g,'Detik ');

document.getElementById("Terhubung").innerHTML = TimeConnect;  
</script>
<script language="javascript">
var Messages = new Date,
    Jams = Messages.getHours();
document.getElementById("WelcomeMessage").innerHTML = 5 <= Jams && Jams <= 11 ? "Selamat Pagi" : 12 <= Jams && Jams <= 15 ? "Selamat Siang" : 15 <= Jams && Jams <= 17 ? "Selamat Sore" : 18 <= Jams && Jams <= 23 ? "Selamat malam" : "Selamat malam menjelang pagi";
</script>
</body>
</html>
