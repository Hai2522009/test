<!DOCTYPE html>
<html>
<head>
    <title>Trang web của tôi</title>
    <style>
    body{
        background-color: #FFFFE0; /* Thay đổi hình nền */
        text-align: center;
        font-family: Arial, sans-serif;
        color: rgb(88, 77, 77);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100vh;
    }
    h1{
        font-size: 3em;
        color: #ED9B40;
    }
    p{
        font-size: 2em;
    }
    .button-container {
        display: flex;
        justify-content: center;
        gap: 20px;
    }
    button{
        background-color: #FF69B4;
        border: none;
        color: white;
        padding: 15px 32px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        margin: 4px 2px;
        cursor: pointer;
        border-radius: 12px;
        position: relative; /* Thay đổi từ absolute sang relative */
        transition: transform 0.3s;
    }
    </style>
</head>
<body>
    <h1>Ngọc dễ thương không?</h1>
    <div class="button-container">
        <button id="yesButton" onclick="A1()">hong :))</button>
        <button id="noButton" onmouseover="A2()">Siuuu dễ thương</button> <!-- Thay đổi từ onclick sang onmouseover -->
    </div>
</body>

<script type="text/javascript">
    function A1()
    {
        alert("Ngọc xinh gái")
    }
    function A2()
    {
        var noButton = document.getElementById("noButton");
        var x = Math.floor(Math.random() * window.innerWidth / 2); /* Giới hạn giá trị ngẫu nhiên của x */
        var y = Math.floor(Math.random() * window.innerHeight / 2); /* Giới hạn giá trị ngẫu nhiên của y */
        noButton.style.left = x + 'px';
        noButton.style.top = y + 'px';
    }
</script>
</html>
