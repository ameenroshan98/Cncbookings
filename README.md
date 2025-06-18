<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNC Conference Room - Book a Slot</title>
    <!-- Optional: Add your own favicon file if you have one.
         Replace 'favicon.ico' with the actual path to your icon file. -->
    <link rel="icon" href="favicon.ico" type="image/x-icon">

    <!-- Google Fonts import for a modern and clean typeface (Roboto) -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <style>
        /* Basic CSS Reset and Body Styling */
        body {
            margin: 0; /* Remove default body margin */
            padding: 0; /* Remove default body padding */
            font-family: 'Roboto', sans-serif; /* Apply Roboto font */
            background-color: #f0f2f5; /* Light grey background for the page */
            color: #333; /* Default text color */
            display: flex; /* Use flexbox for centering content */
            justify-content: center; /* Center content horizontally */
            align-items: center; /* Center content vertically */
            min-height: 100vh; /* Ensure body takes at least full viewport height */
            text-align: center; /* Center text within the body */
            line-height: 1.6; /* Improve readability with line spacing */
            box-sizing: border-box; /* Include padding and border in element's total width and height */
        }

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
        }

        /* Styling for Paragraphs */
        p {
            font-size: 1.1em; /* Slightly larger font size for body text */
            color: #555; /* Medium grey for paragraph text */
            margin-bottom: 30px; /* Space below paragraphs */
        }

        /* Specific Styling for the Google Calendar button (to ensure consistent look) */
        /* !important is used here to potentially override Google's inline styles if necessary,
           though Google's script largely controls the button's appearance. */
        .gc-scheduling-button {
            font-size: 1.2em !important; /* Larger font size for the button text */
            padding: 15px 30px !important; /* More padding for a larger click area */
            border-radius: 8px !important; /* Rounded corners for the button */
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out; /* Smooth hover effects */
        }

        /* Hover effect for the Google Calendar button */
        .gc-scheduling-button:hover {
            transform: translateY(-2px); /* Lifts the button slightly on hover */
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.25); /* Adds a more pronounced shadow on hover */
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome!</h1>
        <p>Use this tool to efficiently book CNC Conference Room slots. Click the button below to see availability and secure your preferred time.</p>

        <!-- Google Calendar Appointment Scheduling button begins here -->
        <!-- These two lines load the necessary external CSS and JavaScript files provided by Google for the button.
             'async' ensures the script loads without blocking the rest of the page. -->
        <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
        <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>

        <!-- This inline JavaScript block initializes the Google Calendar scheduling button. -->
        <script>
        (function() {
          // document.currentScript refers to the <script> tag this code is running from.
          // This allows Google's script to inject the button exactly where this script tag is located.
          var target = document.currentScript;

          // Ensures the scheduling button loads after the entire page (including its own scripts) is ready.
          window.addEventListener('load', function() {
            // Calls the Google Calendar API to load the scheduling button.
            calendar.schedulingButton.load({
              // The unique URL for your specific Google Calendar appointment schedule.
              // REPLACE THIS WITH YOUR ACTUAL GOOGLE CALENDAR SCHEDULE LINK if it changes!
              url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2ua06LyvKlQzoG2ELGuqVraDJc36NWPhHOfZzM-VtXvJFBTAciXQhEaqUz_LBFowX2X4Bcrj6d?gv=true',
              // The color of the button (Google's default blue).
              color: '#039BE5',
              // The text label displayed on the button.
              label: 'Book Your Conference Room',
              // The target element where the button will be rendered.
              target,
            });
          });
        })();
        </script>
        <!-- End Google Calendar Appointment Scheduling button -->

        <p style="margin-top: 30px; font-size: 0.9em; color: #777;">
            We look forward to a productive session!
        </p>
    </div>

</body>
</html>
