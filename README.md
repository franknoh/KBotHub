# [KBotHub](https://kboteditor.kro.kr)



* nolbo
* franknoh

# 기본양식

```html
<!DOCTYPE html>
<html lang="kr"><head>
	<meta charset="utf-8">
	<title>KBotHub</title>
	<link rel="shortcut icon" type="image/jpg" href="https://kboteditor.kro.kr/img/output-onlinepngtools.ico">
	<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
	<meta property="og:type" content="website">
	<meta property="og:url" content="https://kboteditor.kro.kr/">
	<meta property="og:title" content="KakaotalkBot Hub">
	<meta property="og:description" content="카카오톡 봇 허브입니다.">
	<meta property="og:image" content="https://kboteditor.kro.kr/img/grp_img.jpg">
	<meta name="description" content="봇 허브 입니다">
	<meta name="keywords" content="온라인 메신저봇">
	<script src="https://kboteditor.kro.kr/js/Toast.min.js"></script>
	<link rel="stylesheet" href="https://kboteditor.kro.kr/css/Toast.min.css">
	<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
	<link rel="stylesheet" href="https://kboteditor.kro.kr/fonts/fonts.css">
	<link rel="stylesheet" href="https://uicdn.toast.com/tui.chart/latest/tui-chart.min.css">
	<script src="https://uicdn.toast.com/tui.chart/latest/tui-chart-all.min.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/china.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/japan.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/singapore.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/south-korea.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/taiwan.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/thailand.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/usa.js"></script>
	<script src="https://uicdn.toast.com/tui.chart/latest/maps/world.js"></script>
	<script src="https://cdn.firebase.com/libs/firebaseui/3.5.2/firebaseui.js"></script>
	<link type="text/css" rel="stylesheet" href="https://cdn.firebase.com/libs/firebaseui/3.5.2/firebaseui.css" />
</head>
<body>
	<div class="toastjs-container" role="alert" aria-hidden="true"><div class="toastjs"></div></div>
	<!-- The core Firebase JS SDK is always required and must be listed first -->
	<script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-app.js"></script>

	<!-- TODO: Add SDKs for Firebase products that you want to use https://firebase.google.com/docs/web/setup#available-libraries -->
	<script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-analytics.js"></script>
	<script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-auth.js"></script>
	<script src="https://www.gstatic.com/firebasejs/7.16.1/firebase-firestore.js"></script>

	<script>
	  // Your web app's Firebase configuration
	  var firebaseConfig = {
	    apiKey: "AIzaSyBsvjuWiZBTEoBJWMvih4q7JHH6gmHF1X0",
	    authDomain: "editor-280309.firebaseapp.com",
	    databaseURL: "https://editor-280309.firebaseio.com",
	    projectId: "editor-280309",
	    storageBucket: "editor-280309.appspot.com",
	    messagingSenderId: "836598450292",
	    appId: "1:836598450292:web:35d0ab7d3e13faf7bba921",
	    measurementId: "G-RJNBM8TLLK"
	  };
	  // Initialize Firebase
	  firebase.initializeApp(firebaseConfig);
	
	  firebase.analytics();
	  firebase.auth();
	  // Initialize the FirebaseUI Widget using Firebase.
	  var ui = new firebaseui.auth.AuthUI(firebase.auth());
	</script>
</body>
</html>
```
커스텀 oauth
```javascript
firebase.auth().signInWithCustomToken(token).catch(function(error) {
  // Handle Errors here.
  var errorCode = error.code;
  var errorMessage = error.message;
  // ...
});
```
* 로고

![](https://kboteditor.kro.kr/img/grp_img.jpg)

![](https://kboteditor.kro.kr/img/logo.png)
