# web_bookmark
bookmark_share

-----------------------------------------------------------------------------------------------------


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="">
<meta name="author" content="">
<link rel="icon" href="../../favicon.ico">

<title>Bookie - 북마크 공유 플랫폼</title>

<!-- Bootstrap core CSS -->
<link href="css/bootstrap.min.css" rel="stylesheet">

<!-- Custom styles for this template -->
<link href="jumbotron-narrow.css" rel="stylesheet">

<!-- Just for debugging purposes. Don't actually copy these 2 lines! -->
<!--[if lt IE 9]><script src="../../assets/js/ie8-responsive-file-warning.js"></script><![endif]-->
<script src="js/ie-emulation-modes-warning.js"></script>

<!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
<!--[if lt IE 9]>
<script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
<script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
<![endif]-->


<SCRIPT LANGUAGE="JavaScript">
//<!-- Begin
function move_box(an, box) {
var cleft = 40;
var ctop = -20;
var obj = an;

box.style.left = cleft + '%';
ctop += an.offsetHeight + 8;
if (document.body.currentStyle &&
document.body.currentStyle['marginTop']) {
ctop += parseInt(
document.body.currentStyle['marginTop']);
}
box.style.top = ctop + '%';
}

function show_hide_box(an, width, height, borderStyle) {
var href = an.href;
var boxdiv = document.getElementById(href);

if (boxdiv != null) {
if (boxdiv.style.display=='none') {
move_box(an, boxdiv);
boxdiv.style.display='block';
} else
boxdiv.style.display='none';
return false;
}

boxdiv = document.createElement('div');
boxdiv.setAttribute('id', href);
boxdiv.style.display = 'block';
boxdiv.style.position = 'absolute';
boxdiv.style.width = width + 'px';
boxdiv.style.height = height + 'px';
boxdiv.style.border = borderStyle;
boxdiv.style.backgroundColor = '#fff';

var contents = document.createElement('iframe');
contents.scrolling = 'no';
contents.frameBorder = '0';
contents.style.width = width + 'px';
contents.style.height = height + 'px';
contents.src = href;

boxdiv.appendChild(contents);
document.body.appendChild(boxdiv);
move_box(an, boxdiv);

return false;
}
//  End -->
</script>

</head>

<body>

<div class="container">
<div class="header">
<nav>
<ul class="nav nav-pills pull-right">

<li role="presentation"><a href="signup.html" onClick="return show_hide_box(this,300,350)">Sign up</a></li>
<li role="presentation"><a href="signin.html" onClick="return show_hide_box(this,300,250)">Sign in</a></li>
</ul>
</nav>
<h1 class="text-muted"><a href="index.html">Bookie</a></h1>
</div>

<h4 class="text-center"><br><br><br>개인이 가지고 있는 알찬 인터넷 북마크 정보,<br><br>
서로 공유하면 지식을 빨리 쉽게 배울 수 있습니다.<br><br><br><br></h4>


<div class="jumbotron">
<p class="lead"><h4>지금 검색해보세요!</h4><br></p>

<p><form class="navbar-form" role="search">
<div class="form-group">
<input type="search" class="form-control" placeholder="Search">
<button type="button" class="btn btn-lg btn-success" onclick="location.href='search.html'">검색</button>
</div>
</form></p>
</div>

<div class="jumbotron">
<h4>북마크를 업로드하고 다운로드 받으세요!</h4>    <br><br>
<a href="http://localhost:3000/" class="btn btn-lg btn-success" role="button">업로드하기</a>
</div>

<div class="jumbotron">
<h4>북마크를 확인하세요 </h4>    <br><br>
<form action="/Users/hakyongseo/Downloads/bookmarks_18. 12. 6..html" method="post" enctype="multipart/form-data">
<input type="file" name="profile">
<a href="/Users/hakyongseo/Downloads/web_bookmark-master/concu/hash.html" class="btn btn-lg btn-success" role="button">BlockChain Check</a>
<input type="submit" a href="/Users/hakyongseo/Downloads/bookmarks_18.\ 12.\ 6..html" >
</div>


<footer class="footer">
<p>&copy; Company 2018</p>
</footer>

</div> <!-- /container -->


<!-- IE10 viewport hack for Surface/desktop Windows 8 bug -->
<script src="js/ie10-viewport-bug-workaround.js"></script>
<input type="button" value="signup" onclick="showPopup();" />
</body>
</html>
