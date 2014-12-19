Z3d
===
<html>
<head>
<script src="http://threejs.org/build/three.min.js"></script>
<script src="js/OrbitControls.js"></script>
<script src="js/plot.js"></script>
</head>
<body>
<script type="text/javascript">
var x = [];
var y = [];
var z = [];
var colors = [];

config = {
  size: z,
  color: colors
}

function getCol(){
  var str = '';
  for (var i=0; i<6; i++){
    str += Math.floor(Math.random()*10);
  }
  return str;
}

for (var i=0;i<100;i++){
  x.push(Math.random()*10 - 5);
  y.push(Math.random()*10 - 5);
  z.push(Math.random()*10 - 5);
  colors.push(getCol());
}

plot3d(x,y,z, config);

</script>
</body>
</html>
