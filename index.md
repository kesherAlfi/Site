<!DOCTYPE html>
<html lang="en">

<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	<title>Document</title>

	<!--Bootsrap 4 CDN-->
	<link rel="stylesheet" href="bootstrap.min.css"
		integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

	<!--Fontawesome CDN-->
	<link rel="stylesheet" href="all.css"
		integrity="sha384-mzrmE5qonljUremFsqc01SB46JvROS7bZs3IO2EmfFsd15uHvIt+Y8vEf7N7fWAU" crossorigin="anonymous">
	<!--Custom styles-->
	<style>
		body,
		html {
			margin: 0;
			padding: 0;
			height: 100%;
		}
		
		.user_card {
			height: 100%;
			width: 100%;
			margin-top: auto;
			margin-bottom: auto;
			position: relative;
			display: flex;
			justify-content: center;
			flex-direction: column;
		}

		.brand_logo_container {
			margin-left:auto;
			margin-right:auto;
			height: 300px;
			width: 300px;
		}

		.brand_logo {
			height: 280px;
			width: 280px;
		}
		
		a {
		  text-decoration: none;
		}
		
		.aaa{
			width: 24px;
		}
	</style>
	
	<script type="text/javascript">
	
	
    function showAndroidToast(text) {
        KehilotSamsung.showToast(text);
    }
    
     function getImei() {
        var imei = KehilotSamsung.getImei();
	showAndroidToast(imei)
    }
    
     function getUserName() {
        var userName = KehilotSamsung.getUserName();
	showAndroidToast(userName)
    }
    
     function sendUserName(place, userName) {
        KehilotSamsung.saveUserName(place, userName);
    }
    
     function showAndroidToast() {
        KehilotSamsung.showToast("בדיקה");
    }
    
    </script>
</head>

<body>
	<div class="container h-100">
		<div class="d-flex justify-content-center h-100">
			<div class="user_card">
				<div class="d-flex justify-content-center">
					<div class="brand_logo_container">
						<img src="kehilot-logo.png" class="brand_logo" alt="Logo">
					</div>
				</div>
				<div class="d-flex justify-content-center mt-3 login_container">
				  אנו חווים כרגע בעיית תקשורת, נחזור לפעילות בהקדם האפשרי
				</div>
					
				<div class="d-flex justify-content-center mt-3 login_container">
					<button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">קבל אמא</button>
										<span class="aaa">           </span>

					<button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">שלח משתמש</button>
										<span class="aaa">           </span>

					<button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">קבל משתמש</button>
										<span class="aaa">           </span>

					<button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">צלם מסך</button>
										<span class="aaa">           </span>

					<button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">הפעל מחדש</button>
				</div>
			</div>
		</div>
	</div>
</body>

</html>
