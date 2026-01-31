# Pushkar
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Happy Birthday Pushkar</title>
    <style>
        /* Force the page to fill the mobile screen perfectly */
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            background-color: #000;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
        }

        /* This creates ONE border around the whole screen, no lines in the middle */
        .screen-frame {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            pointer-events: none;
            z-index: 100;
            border: 20px solid transparent;
            border-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Ctext y='50' font-size='40'%3E🌸%3C/text%3E%3Ctext x='50' y='90' font-size='40'%3E🌺%3C/text%3E%3C/svg%3E") 30 round;
        }

        .content {
            text-align: center;
            z-index: 10;
        }

        /* Modern Appear Animation */
        .animate {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 1s ease-out forwards;
        }

        .text-top {
            color: #ffffff;
            font-size: 1.5rem;
            font-weight: 300;
            margin-bottom: 0.5rem;
        }

        .name-big {
            color: #ff4081;
            font-size: 4rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 2px;
            animation-delay: 0.5s; /* Appears after 'Happiest Birthday' */
            text-shadow: 0 0 20px rgba(255, 64, 129, 0.4);
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>

    <div class="screen-frame"></div>

    <div class="content">
        <div class="animate text-top">Happiest Birthday</div>
        <div class="animate name-big">Pushkar</div>
    </div>

</body>
</html>
