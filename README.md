<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNC Conference Room - Book a Slot</title>
    <!-- Optional: Add your own favicon file if you have one.
         Replace 'favicon.ico' with the actual path to your icon file. -->
    <link rel="icon" href="favicon.ico" type="image/x-icon">

    <!-- Google Fonts import for Roboto -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <style>
        /* Basic CSS Reset and Body Styling */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Roboto', sans-serif; /* Default body font */
            background-color: #f0f2f5;
            color: #333;
            display: flex;
            flex-direction: column; /* Arrange items vertically */
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
            line-height: 1.6;
            box-sizing: border-box;
        }

        /* Main Container Styling for the content box */
        .container {
            background-color: #ffffff;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
            max-width: 500px;
            width: 90%;
            box-sizing: border-box;
        }

        /* Styling for Headings */
        h1 {
            color: #2c3e50;
            font-size: 2.2em;
            margin-bottom: 15px;
            font-weight: 700;
            font-family: 'Roboto', sans-serif; /* Keep body font or choose another for headings */
        }

        /* Styling for Paragraphs */
        p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 30px;
            font-family: 'Roboto', sans-serif; /* Keep body font */
        }

        /* Specific styling for the new introductory paragraph */
        .intro-paragraph {
            margin-top: 10px;
            margin-bottom: 30px;
            font-size: 1.0em;
            color: #666;
        }

        /* Container for multiple buttons */
        .button-group {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-bottom: 30px;
        }

        /* Specific Styling for the Google Calendar button (to ensure consistent look) */
        .gc-scheduling-button {
            font-size: 1.2em !important;
            padding: 15px 30px !important;
            border-radius: 8px !important;
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
            width: 100%;
            box-sizing: border-box;
        }

        /* Hover effect for the Google Calendar button */
        .gc-scheduling-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.25);
        }

    </style>
</head>
<body>
    <!-- The "Cncbookings" text previously appeared implicitly as plain text,
         not as a styled <div> with a specific font. -->

    <div class="container">
        <h1>Welcome CNC Members!</h1>
        <p class="intro-paragraph">
            This platform is designed to help you quickly and efficiently book meeting rooms that suit your session size and purpose. Whether it’s for a small team huddle or a large group discussion.
        </p>
        <p>Please choose the type of meeting room you would like to book, based on your meeting needs:</p>

        <div class="button-group">
            <!-- Google Calendar Appointment Scheduling button for Conference Room (Minimum 6 attendees) -->
            <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
            <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
            <script>
            (function() {
              var target = document.currentScript;
              window.addEventListener('load', function() {
                calendar.schedulingButton.load({
                  url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ1JCwJNC4c8tLtVT68LxD5BhvuKwTMHkZkgOoHC8Fw4funbfoii6MNLre8V-KEAKHp9s9zZQAgh?gv=true',
                  color: '#039BE5', /* Google Blue */
                  label: 'Book Conference Room (6+ Attendees)',
                  target,
                });
              });
            })();
            </script>

            <!-- Google Calendar Appointment Scheduling button for Zoom Meeting -->
            <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
            <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
            <script>
            (function() {
              var target = document.currentScript;
              window.addEventListener('load', function() {
                calendar.schedulingButton.load({
                  url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ32KEM4_0v-kbkSR1hj93VqH18-gPpaTkzqOR_Jgo-YVYHVrN4c8Z5uVAc3cqxvMpRl5YLs2_X_?gv=true',
                  color: '#F4B400', /* Google Yellow for contrast */
                  label: 'Book a Zoom Meeting',
                  target,
                });
              });
            })();
            </script>

            <!-- Google Calendar Appointment Scheduling button for Boardroom (Ideal for lesser attendees) -->
            <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
            <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
            <script>
            (function() {
              var target = document.currentScript;
              window.addEventListener('load', function() {
                calendar.schedulingButton.load({
                  url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2meAb8q3yZwCVgedCVWfH8_IreX8mhqpmunWNUW4r6kIio-PPkssqv1ZR5cO8nuLJea3_fa9-o?gv=true',
                  color: '#34A853', /* Google Green for contrast */
                  label: 'Book Boardroom(Fewer Attendees)',
                  target,
                });
              });
            })();
            </script>
        </div>

        <p style="margin-top: 30px; font-size: 0.9em; color: #777;">
            Hope you have a great meeting experience!
        </p>
    </div>

</body>
</html>
