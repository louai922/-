<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اقتباسات ملهمة</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
            direction: rtl;
            overflow: hidden;
        }
        .container {
            text-align: center;
            background-color: #fff;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            max-width: 600px;
            margin: 20px;
        }
        h1 {
            color: #ff6f61;
            font-size: 2.5em;
            margin-bottom: 20px;
        }
        #quote {
            font-size: 1.5em;
            color: #333;
            margin-bottom: 30px;
            line-height: 1.6;
        }
        button {
            background-color: #6ab04c;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 25px;
            transition: background-color 0.3s, transform 0.2s;
        }
        button:hover {
            background-color: #218c74;
            transform: scale(1.05);
        }
        .animation {
            animation: fadeIn 1s ease-in-out;
        }
        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }
        @media (max-width: 600px) {
            h1 {
                font-size: 2em;
            }
            #quote {
                font-size: 1.2em;
            }
            button {
                padding: 10px 20px;
                font-size: 1em;
            }
        }
    </style>
</head>
<body>
    <div class="container animation">
        <h1>اقتباسات ملهمة</h1>
        <p id="quote">اضغط على الزر للحصول على اقتباس ملهم!</p>
        <button onclick="getNewQuote()">اقتباس جديد</button>
    </div>
    <script>
        const quotes = [
            "كن التغيير الذي تريد أن تراه في العالم.",
            "النجاح ليس غياب العقبات، بل الشجاعة للمضي قدمًا رغم وجودها.",
            "كل يوم هو فرصة جديدة لتحقيق أحلامك.",
            "الإيمان بالنفس هو أول خطوة نحو النجاح.",
            "لا تستسلم، فالأشياء العظيمة تأتي مع الصبر."
        ];

        function getNewQuote() {
            const quoteElement = document.getElementById('quote');
            const randomIndex = Math.floor(Math.random() * quotes.length);
            quoteElement.textContent = quotes[randomIndex];
            quoteElement.classList.remove('animation');
            void quoteElement.offsetWidth;
            quoteElement.classList.add('animation');
        }
    </script>
</body>
</html>
كن انت
