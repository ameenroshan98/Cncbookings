<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNC Conference Room - Book a Slot</title>
    <!-- Optional: Add your own favicon file if you have one.
         Replace 'favicon.ico' with the actual path to your icon file. -->
    <link rel="icon" href="favicon.ico" type="image/x-icon">

    <!-- Google Fonts import for Roboto (for body text) -->
    <!-- Montserrat is no longer needed as the site-title is removed -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <style>
        /* Basic CSS Reset and Body Styling */
        body {
            margin: 0; /* Remove default body margin */
            padding: 0; /* Remove default body padding */
            font-family: 'Roboto', sans-serif; /* Default body font */
            background-color: #f0f2f5; /* Light grey background for the page */
            color: #333; /* Default text color */
            display: flex; /* Use flexbox for centering content */
            flex-direction: column; /* Arrange items vertically */
            justify-content: center; /* Center content horizontally */
            align-items: center; /* Center content vertically */
            min-height: 100vh; /* Ensure body takes at least full viewport height */
            text-align: center; /* Center text within the body */
            line-height: 1.6; /* Improve readability with line spacing */
            box-sizing: border-box; /* Include padding and border in element's total width and height */
        }

        /* The .site-title styling is no longer needed as the element is removed. */

        /* Main Container Styling for the content box */
        .container {
            background-color: #ffffff; /* White background for the content box */
            padding: 40px; /* Internal spacing within the box */
            border-radius: 12px; /* Rounded corners for a softer look */
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1); /* Soft shadow for depth */
            max-width: 500px; /* Maximum width for better readability on large screens */
            width: 90%; /* Responsive width, takes 90% of parent width */
            box-sizing: border-box; /* Ensures padding is included in the 90% width */
        }

        /* Styling for Headings */
        h1 {
            color: #2c3e50; /* Dark blue-grey for prominent headings */
            font-size: 2.2em; /* Larger font size for main heading */
            margin-bottom: 15px; /* Space below the heading */
            font-weight: 700; /* Bold font weight */
            font-family: 'Roboto', sans-serif; /* Headings use Roboto for consistency with body */
        }

        /* Styling for Paragraphs */
        p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 30px;
            font-family: 'Roboto', sans-serif; /* Paragraphs use Roboto */
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
            flex-direction: column; /* Stack buttons vertically */
            gap: 15px; /* Space between buttons */
            margin-bottom: 30px;
        }

        /* Specific Styling for the Google Calendar button (to ensure consistent look) */
        /* !important is used here to potentially override Google's inline styles if necessary,
           though Google's script largely controls the button's appearance. */
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
    <!-- The "Cncbookings" title div has been removed as requested. -->

    <div class="container">
        <h1>Welcome CNC Members!</h1>
        <p class="intro-paragraph">
            This platform is designed to help you quickly and efficiently book meetings that suit your session size and purpose. Whether it’s for a small team huddle or a large group discussion.
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

            <!-- Google Calendar Appointment Scheduling button for Meeting Room (Fewer Attendees) -->
            <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
            <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
            <script>
            (function() {
              var target = document.currentScript;
              window.addEventListener('load', function() {
                calendar.schedulingButton.load({
                  url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2meAb8q3yZwCVgedCVWfH8_IreX8mhqpmunWNUW4r6kIio-PPkssqv1ZR5cO8nuLJea3_fa9-o?gv=true',
                  color: '#34A853', /* Google Green for contrast */
                  label: 'Book Meeting Room (Fewer Attendees)',
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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNC Conference Room - Book a Slot</title>
    <!-- Optional: Add your own favicon file if you have one.
         Replace 'favicon.ico' with the actual path to your icon file. -->
    <link rel="icon" href="favicon.ico" type="image/x-icon">

    <!-- Google Fonts import for Roboto (for body text) -->
    <!-- Montserrat is no longer needed as the site-title is removed -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <style>
        /* Basic CSS Reset and Body Styling */
        body {
            margin: 0; /* Remove default body margin */
            padding: 0; /* Remove default body padding */
            font-family: 'Roboto', sans-serif; /* Default body font */
            background-color: #f0f2f5; /* Light grey background for the page */
            color: #333; /* Default text color */
            display: flex; /* Use flexbox for centering content */
            flex-direction: column; /* Arrange items vertically */
            justify-content: center; /* Center content horizontally */
            align-items: center; /* Center content vertically */
            min-height: 100vh; /* Ensure body takes at least full viewport height */
            text-align: center; /* Center text within the body */
            line-height: 1.6; /* Improve readability with line spacing */
            box-sizing: border-box; /* Include padding and border in element's total width and height */
        }

        /* The .site-title styling is no longer needed as the element is removed. */

        /* Main Container Styling for the content box */
        .container {
            background-color: #ffffff; /* White background for the content box */
            padding: 40px; /* Internal spacing within the box */
            border-radius: 12px; /* Rounded corners for a softer look */
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1); /* Soft shadow for depth */
            max-width: 500px; /* Maximum width for better readability on large screens */
            width: 90%; /* Responsive width, takes 90% of parent width */
            box-sizing: border-box; /* Ensures padding is included in the 90% width */
        }

        /* Styling for Headings */
        h1 {
            color: #2c3e50; /* Dark blue-grey for prominent headings */
            font-size: 2.2em; /* Larger font size for main heading */
            margin-bottom: 15px; /* Space below the heading */
            font-weight: 700; /* Bold font weight */
            font-family: 'Roboto', sans-serif; /* Headings use Roboto for consistency with body */
        }

        /* Styling for Paragraphs */
        p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 30px;
            font-family: 'Roboto', sans-serif; /* Paragraphs use Roboto */
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
            flex-direction: column; /* Stack buttons vertically */
            gap: 15px; /* Space between buttons */
            margin-bottom: 30px;
        }

        /* Specific Styling for the Google Calendar button (to ensure consistent look) */
        /* !important is used here to potentially override Google's inline styles if necessary,
           though Google's script largely controls the button's appearance. */
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
    <!-- The "Cncbookings" title div has been removed as requested. -->

    <div class="container">
        <h1>Welcome CNC Members!</h1>
        <p class="intro-paragraph">
            This platform is designed to help you quickly and efficiently book meetings that suit your session size and purpose. Whether it’s for a small team huddle or a large group discussion.
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

            <!-- Google Calendar Appointment Scheduling button for Meeting Room (Fewer Attendees) -->
            <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
            <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
            <script>
            (function() {
              var target = document.currentScript;
              window.addEventListener('load', function() {
                calendar.schedulingButton.load({
                  url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2meAb8q3yZwCVgedCVWfH8_IreX8mhqpmunWNUW4r6kIio-PPkssqv1ZR5cO8nuLJea3_fa9-o?gv=true',
                  color: '#34A853', /* Google Green for contrast */
                  label: 'Book Meeting Room (Fewer Attendees)',
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
