<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNC Conference Room - Book a Slot</title>
    <link rel="icon" href="favicon.ico" type="image/x-icon"> <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <style>
        /* Basic Reset & Body Styling */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Roboto', sans-serif; /* Use Roboto from Google Fonts */
            background-color: #f0f2f5; /* Light grey background */
            color: #333;
            display: flex;
            justify-content: center; /* Center horizontally */
            align-items: center; /* Center vertically */
            min-height: 100vh; /* Make body take full viewport height */
            text-align: center;
            line-height: 1.6;
            box-sizing: border-box; /* Include padding/border in element's total width/height */
        }

        /* Main Container for Content */
        .container {
            background-color: #ffffff;
            padding: 40px;
            border-radius: 12px; /* Rounded corners */
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1); /* Soft shadow */
            max-width: 500px; /* Limit width for better readability */
            width: 90%; /* Responsive width */
            box-sizing: border-box;
        }

        /* Headings and Paragraphs */
        h1 {
            color: #2c3e50; /* Darker blue-grey for heading */
            font-size: 2.2em;
            margin-bottom: 15px;
            font-weight: 700;
        }

        p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 30px;
        }

        /* Styling specific to the Google Calendar button */
        .gc-scheduling-button {
            /* You can add more specific overrides here if needed */
            font-size: 1.2em !important;
            padding: 15px 30px !important;
            border-radius: 8px !important;
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
            /* The background-color and text color are set by the Google script's 'color' option */
        }

        .gc-scheduling-button:hover {
            transform: translateY(-2px); /* Slight lift effect on hover */
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.25); /* More prominent shadow on hover */
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome, Employees!</h1>
        <p>Use this tool to efficiently book CNC Conference Room slots. Click the button below to see availability and secure your preferred time.</p>

        <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
        <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
        
        <script>
        (function() {
          var target = document.currentScript; // Targets this specific script tag's location for button placement
          window.addEventListener('load', function() {
            calendar.schedulingButton.load({
              url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2ua06LyvKlQzoG2ELGuqVraDJc36NWPhHOfZzM-VtXvJFBTAciXQhEaqUz_LBFowX2X4Bcrj6d?gv=true',
              color: '#039BE5', // Google's default blue color for the button
              label: 'Book Your Conference Room', // The text displayed on the button
              target, // The element where the button should be injected
            });
          });
        })();
        </script>
        <p style="margin-top: 30px; font-size: 0.9em; color: #777;">
            We look forward to a productive session!
        </p>
    </div>

</body>
</html>
