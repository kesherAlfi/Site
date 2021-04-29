<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>

    <link rel="stylesheet" href="bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
    <link rel="stylesheet" href="all.css" integrity="sha384-mzrmE5qonljUremFsqc01SB46JvROS7bZs3IO2EmfFsd15uHvIt+Y8vEf7N7fWAU" crossorigin="anonymous">

    <script>
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

            <div class="d-flex justify-content-center mt-3 login_container">
                <button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">קבל אמא</button>
                <span class="aaa"></span>

                <button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">שלח משתמש</button>
                <span class="aaa"></span>

                <button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">קבל משתמש</button>
                <span class="aaa"></span>

                <button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">צלם מסך</button>
                <span class="aaa"></span>

                <button type="button" name="button" class="btn login_btn" onClick="KehilotSamsung('Hello Android!')">הפעל מחדש</button>
            </div>
        </div>
    </div>
</div>
</body>

</html>
