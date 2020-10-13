<p style="font-size:36px">Egert-Yako Poom</p>

<p>Date/Time: <span id="datetime"></span></p>

<script>
var dt = new Date();
document.getElementById("datetime").innerHTML = (("0"+(dt.getMonth()+1)).slice(-2)) +"/"+ (("0"+dt.getDate()).slice(-2)) +"/"+ (dt.getFullYear()) +" "+ (("0"+dt.getHours()+1).slice(-2)) +":"+ (("0"+dt.getMinutes()+1).slice(-2));
</script>

var gmtDateTime = moment.utc("2015-10-24 20:00", "YYYY-MM-DD HH")
var local = gmtDateTime.local().format('YYYY-MMM-DD h:mm A');
