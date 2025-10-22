<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CNC Conference Room - Book a Slot</title>
  <link rel="icon" href="favicon.ico" type="image/x-icon">
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Roboto', sans-serif;
      background-color: #f0f2f5;
      color: #333;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      text-align: center;
    }
    .container {
      background: #fff;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 8px 25px rgba(0,0,0,0.1);
      max-width: 500px;
      width: 90%;
    }
    h1 {
      color: #2c3e50;
      font-size: 2.2em;
      margin-bottom: 15px;
      font-weight: 700;
    }
    p { color: #555; }
    .intro-paragraph { color: #666; margin-bottom: 30px; }
    .button-group { display: flex; flex-direction: column; gap: 15px; }
    .gc-scheduling-button {
      font-size: 1.2em !important;
      padding: 15px 30px !important;
      border-radius: 8px !important;
      transition: transform 0.2s, box-shadow 0.2s;
      width: 100%;
    }
    .gc-scheduling-button:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 15px rgba(0,0,0,0.25);
    }
    @media (max-width: 480px) {
      .container { padding: 25px; }
      h1 { font-size: 1.8em; }
      .gc-scheduling-button { font-size: 1em !important; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Welcome CNC Members!</h1>
    <p class="intro-paragraph">
      Quickly book the right type of meeting for your team-whether it’s a small huddle or a large discussion.
    </p>
    <div class="button-group">
      <div id="conf-btn"></div>
      <div id="smallroom-btn"></div>
      <div id="zoom-btn"></div>
    </div>
    <p style="margin-top:30px; font-size:0.9em; color:#777;">Hope you have a great meeting experience!</p>
  </div>

  <!-- Google Calendar script -->
  <script src="https://calendar.google.com/calendar/scheduling-button-script.js" defer></script>

  <script>
    window.addEventListener('load', function() {
      // Book Conference Room (6+ Attendees)
      calendar.schedulingButton.load({
        url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ1JCwJNC4c8tLtVT68LxD5BhvuKwTMHkZkgOoHC8Fw4funbfoii6MNLre8V-KEAKHp9s9zZQAgh?gv=true',
        color: '#039BE5',
        label: 'Book Conference Room (6+ Attendees)',
        target: document.getElementById('conf-btn'),
      });

      // Book Meeting Room (Fewer Attendees)
      calendar.schedulingButton.load({
        url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2meAb8q3yZwCVgedCVWfH8_IreX8mhqpmunWNUW4r6kIio-PPkssqv1ZR5cO8nuLJea3_fa9-o?gv=true',
        color: '#34A853',
        label: 'Book Meeting Room (Fewer Attendees)',
        target: document.getElementById('smallroom-btn'),
      });

      // Book a Zoom Meeting
      calendar.schedulingButton.load({
        url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ32KEM4_0v-kbkSR1hj93VqH18-gPpaTkzqOR_Jgo-YVYHVrN4c8Z5uVAc3cqxvMpRl5YLs2_X_?gv=true',
        color: '#F4B400',
        label: 'Book a Zoom Meeting',
        target: document.getElementById('zoom-btn'),
      });
    });
  </script>
</body>
</html>
