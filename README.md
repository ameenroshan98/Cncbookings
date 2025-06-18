<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNC Bookings - Schedule Your Appointment</title>
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
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Make body take full viewport height */
            text-align: center;
            line-height: 1.6;
        }

        /* Main Container for Content */
        .container {
            background-color: #ffffff;
            padding: 40px;
            border-radius: 12px; /* Rounded corners */
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1); /* Soft shadow */
            max-width: 500px; /* Limit width for better readability */
            width: 90%; /* Responsive width */
            box-sizing: border-box; /* Include padding in element's total width and height */
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

        /* Styling specific to the Google Calendar button (to ensure it looks good) */
        /* You might need to inspect the Google button's generated classes for more specific overrides */
        .gc-scheduling-button {
             /* Example: if you want to override default Google styles */
            font-size: 1.2em !important;
            padding: 15px 30px !important;
            border-radius: 8px !important;
            /* background-color: #039BE5 !important; /* This should be handled by the script color */
            /* color: white !important; */
            /* box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2); */
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }

        .gc-scheduling-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.25);
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome to CNC Bookings!</h1>
        <p>We're excited to help you schedule your next CNC appointment. Click the button below to view our availability and book a slot that works for you.</p>

        <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
        <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
        <script>
        (function() {
          var target = document.currentScript; // This targets the current script tag itself
          window.addEventListener('load', function() {
            calendar.schedulingButton.load({
              url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2ua06LyvKlQzoG2ELGuqVraDJc36NWPhHOfZzM-VtXvJFBTAciXQhEaqUz_LBFowX2X4Bcrj6d?gv=true',
              color: '#039BE5', // Google's default blue
              label: 'Book Your CNC Slot', // Changed button text for better context
              target,
            });
          });
        })();
        </script>
        <p style="margin-top: 30px; font-size: 0.9em; color: #777;">
            We look forward to seeing you!
        </p>
    </div>

</body>
</html>

