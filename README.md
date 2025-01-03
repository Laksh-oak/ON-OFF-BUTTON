# ON-OFF-BUTTON
 <html>

<head>

    <title>On/Off</title>
    <style>
        body {
            background-color: rgb(95, 51, 136);
        }
        
        #outer {
            height: 500px;
            width: 500px;
            border: 2px solid black;
            background-color: rgb(116, 46, 182);
            margin: 20px auto;
            border-radius: 20px;
            text-align: center;
        }
        
        button {
            padding: 10px 30px;
            margin-top: 10px;
            font-weight: bold;
            font-size: 20px;
            color: black;
            border-radius: 50px;
            border: 2px solid red;
            cursor: pointer;
            background-color: rgb(161, 111, 208);
        }
    </style>
</head>

<body>
    <div id="outer">
        <img src="off.png" id="image" width="40%" alt=""><br>
        <button id="button">On/Off</button>
    </div>


    <script>
        const bulb = document.getElementById('image');
        const btn = document.getElementById('button');
        let isOn = false;
        btn.addEventListener('click', () => {
            isOn = !isOn;
            bulb.src = isOn ? 'on.png' : 'off.png';
        });
    </script>

</body>

</html>
