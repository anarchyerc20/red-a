<html>
<head>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>

<script defer="">

function copy() {
  let textarea = document.getElementById("maintext");
  textarea.select();
  document.execCommand("copy");
}

function convertToRedA() {
  var txt = document.getElementById('maintext').value;
  var newtxt = txt.replaceAll("a","🅰");


  var newtxt2 = newtxt.replaceAll("A","🅰");

  document.getElementById('maintext').value = newtxt2;
}

</script>

</head>
<body>


<div id='container' style='width:600px; border:1px solid black;'>
    <textarea id="maintext" style='border-style:none none dashed none; border-color:black; width:100%; display:block;box-sizing:border-box;border-width:1px; margin-bottom:1px;'></textarea>
    <div style='width:100%; box-sizing:border-box; height:35px;padding:5px;'>
      <a href="" class="btn btn-github" onclick="convertToRedA()">CONVERT TO RED 🅰️s</a>
      <a href="" class="btn btn-github"  onclick="copy()"  />Copy</a>
    </div>
</div>

</body>

</html>
