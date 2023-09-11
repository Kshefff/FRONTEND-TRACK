<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ksheff</title>
    <style>

        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        header {
            background-color: #007bff;
            color: #fff;
            padding: 10px;
            text-align: center;
        }

        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        img[data-testid="slackDisplayImage"] {
            display: block;
            margin: 0 auto;
            max-width: 200px;
            border-radius: 50%;
        }

        p[data-testid="slackUserName"],
        p[data-testid="currentDayOfTheWeek"],
        p[data-testid="currentUTCTime"],
        p[data-testid="myTrack"] {
            text-align: center;
        }

        p[data-testid="slackUserName"] {
            font-size: 24px;
            font-weight: bold;
        }

        p[data-testid="currentDayOfTheWeek"],
        p[data-testid="currentUTCTime"],
        p[data-testid="myTrack"] {
            font-size: 18px;
        }

    
        .github-link {
            text-align: center;
            margin-top: 20px; 
        }
    </style>
</head>
<body>
    <header>
        <h1 data-testid="slackUserName">Ksheff</h1>
    </header>
    <div class="container">
        <img src="images/DPksheff.jpg" alt="Your Slack Username" data-testid="slackDisplayImage">
        <p data-testid="currentDayOfTheWeek">Friday</p>
        <p data-testid="currentUTCTime">UTC Time</p>
        <p data-testid="myTrack">Frontend</p>
    </div>

    <script>
    
        const currentUTCTimeElement = document.querySelector('[data-testid="currentUTCTime"]');
        function updateCurrentUTCTime() {
            const currentUTCTime = Date.now();
            currentUTCTimeElement.textContent = currentUTCTime.toString();
        }

        updateCurrentUTCTime();

        setInterval(updateCurrentUTCTime, 5000);

    </script>
    <div class="github-link">
        <a href="https://github.com/Kshefff/FRONTEND-TRACK/blob/main/README.md?plain=1" target="_blank">Click to Visit GITHUB</a>
    </div>

</body>
</html>
