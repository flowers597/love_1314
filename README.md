<!DOCTYPE html>
<html>
<head>
    <style>
        body {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            text-align: center;
            padding: 50px;
            color: white;
        }
        #msg { 
            display: none;
            font-size:24px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>⚠️ 警告：发现未知情感程序</h1>
    <p>正在解码... <span id="progress">0%</span></p>
    <button onclick="showLove()">点击强制运行</button>
    <p id="msg">❤️ 解码完成！错误代码：LOVE-1314<br>——我的香兵</p>

    <script>
        function showLove() {
            let i = 0;
            const timer = setInterval(() => {
                document.getElementById("progress").textContent = i + "%";
                i += 10;
                if (i > 100) {
                    clearInterval(timer);
                    document.getElementById("msg").style.display = "block";
                }
            }, 200);
        }
    </script>
</body>
</html>