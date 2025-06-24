<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Company Competition Leaderboard</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom font for a clean look */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8; /* Light background */
        }
        /* Specific styling for the news and events sections to ensure proper spacing and appearance */
        .news-item:not(:last-child),
        .event-item:not(:last-child) {
            margin-bottom: 0.5rem; /* Add some space between items */
        }
    </style>
</head>
<body class="p-4 sm:p-8 flex items-center justify-center min-h-screen">
    <div class="w-full max-w-4xl bg-white rounded-xl shadow-xl overflow-hidden">
        <!-- Leaderboard Header -->
        <div class="bg-gradient-to-r from-purple-600 to-indigo-700 p-6 sm:p-8 text-white text-center rounded-t-xl">
            <h1 class="text-3xl sm:text-4xl font-bold mb-2">IGNITE'25</h1>
            <p class="text-lg opacity-90">Current Standings - Simple Points Accumulation</p>
        </div>

        <!-- Leaderboard Table Container -->
        <div class="p-4 sm:p-6 overflow-x-auto">
            <table class="min-w-full divide-y divide-gray-200">
                <thead class="bg-gray-50">
                    <tr>
                        <th scope="col" class="px-3 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider rounded-tl-lg">
                            Rank
                        </th>
                        <th scope="col" class="px-3 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">
                            Team/Individual Name
                        </th>
                        <th scope="col" class="px-3 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">
                            Total Points
                        </th>
                        <th scope="col" class="px-3 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider rounded-tr-lg">
                            Last Updated
                        </th>
                    </tr>
                </thead>
                <tbody class="bg-white divide-y divide-gray-200">
                    <!-- Sample Data Rows with updated team names -->
                    <tr class="hover:bg-purple-50 transition duration-200 ease-in-out">
                        <td class="px-3 py-4 whitespace-nowrap text-sm font-medium text-gray-900 rounded-bl-lg">
                            1
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            Golden Titans
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            1500
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-500 rounded-br-lg">
                            2025-06-24 10:30 AM
                        </td>
                    </tr>
                    <tr class="bg-purple-50 hover:bg-purple-100 transition duration-200 ease-in-out">
                        <td class="px-3 py-4 whitespace-nowrap text-sm font-medium text-gray-900">
                            2
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            Vortex Squad
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            1250
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-500">
                            2025-06-24 10:28 AM
                        </td>
                    </tr>
                    <tr class="hover:bg-purple-50 transition duration-200 ease-in-out">
                        <td class="px-3 py-4 whitespace-nowrap text-sm font-medium text-gray-900">
                            3
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            Flame Warriors
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            1100
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-500">
                            2025-06-24 10:25 AM
                        </td>
                    </tr>
                    <tr class="bg-purple-50 hover:bg-purple-100 transition duration-200 ease-in-out">
                        <td class="px-3 py-4 whitespace-nowrap text-sm font-medium text-gray-900">
                            4
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            Penta Force'25
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-700">
                            980
                        </td>
                        <td class="px-3 py-4 whitespace-nowrap text-sm text-gray-500">
                            2025-06-24 10:20 AM
                        </td>
                    </tr>
                    <!-- Removed "Future Thinkers" -->
                </tbody>
            </table>
        </div>

        <!-- Running News Section -->
        <div class="bg-blue-50 border-t border-blue-200 p-4 sm:p-6">
            <h3 class="text-xl font-semibold text-blue-800 mb-4 flex items-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M19 20H5a2 2 0 01-2-2V6a2 2 0 012-2h10a2 2 0 012 2v10m-3 4H7a2 2 0 01-2-2V6a2 2 0 012-2h10a2 2 0 012 2v10a2 2 0 01-2 2zM9 9h6m-6 4h6m-6 4h6" />
                </svg>
                Competition News & Updates
            </h3>
            <ul class="text-gray-700 text-sm sm:text-base">
                <li class="news-item border-b border-blue-100 pb-2 mb-2">
                    <span class="font-semibold text-blue-700">[2025-06-24]</span> **Milestone Alert!** "Golden Titans" just crossed the 1500 point mark! Fantastic work!
                </li>
                <li class="news-item border-b border-blue-100 pb-2 mb-2">
                    <span class="font-semibold text-blue-700">[2025-06-24]</span> **Sports Challenge Update:** The "Fitness Fanatics" are leading the step count challenge this week! Keep moving!
                </li>
                <li class="news-item border-b border-blue-100 pb-2 mb-2">
                    <span class="font-semibold text-blue-700">[2025-06-24]</span> **Arts & Creativity Spotlight:** Check out the amazing digital art submissions in the #IGNITE_Art channel! Voting starts soon.
                </li>
                <li class="news-item border-b border-blue-100 pb-2 mb-2">
                    <span class="font-semibold text-blue-700">[2025-06-23]</span> New bonus points opportunity announced for **"Collaboration Initiatives"** - Check your email for details!
                </li>
                <li class="news-item border-b border-blue-100 pb-2 mb-2">
                    <span class="font-semibold text-blue-700">[2025-06-22]</span> Last call for Q3 Innovation ideas! Submissions close end of day 2025-06-25.
                </li>
                <li class="news-item">
                    <span class="font-semibold text-blue-700">[2025-06-21]</span> Don't forget to log all your training completions. Points are updated every night!
                </li>
            </ul>
        </div>

        <!-- Upcoming Event Section -->
        <div class="bg-green-50 border-t border-green-200 p-4 sm:p-6 mt-4">
            <h3 class="text-xl font-semibold text-green-800 mb-4 flex items-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2 text-green-600" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                </svg>
                Upcoming Events
            </h3>
            <ul class="text-gray-700 text-sm sm:text-base">
                <li class="event-item border-b border-green-100 pb-2 mb-2">
                    <span class="font-semibold text-green-700">2025-07-01:</span> **Mid-Competition Check-in & Workshop** - Virtual session on "Boosting Your Innovation Score."
                </li>
                <li class="event-item border-b border-green-100 pb-2 mb-2">
                    <span class="font-semibold text-green-700">2025-07-08:</span> **Carroms Tournament** - Sign-ups are open now! Details on the #sports channel.
                </li>
                <li class="event-item border-b border-green-100 pb-2 mb-2">
                    <span class="font-semibold text-green-700">2025-07-15:</span> **"Idea Pitch-Off" Round 1** - Present your best ideas to a panel for bonus points! (Sign-ups open 2025-07-05)
                </li>
                <li class="event-item border-b border-green-100 pb-2 mb-2">
                    <span class="font-semibold text-green-700">2025-07-22:</span> **Chess Challenge** - Strategic minds unite! Register for a chance to be the IGNITE'25 Chess Master.
                </li>
                <li class="event-item border-b border-green-100 pb-2 mb-2">
                    <span class="font-semibold text-green-700">2025-08-05:</span> **Calligraphy Workshop** - Unleash your artistic side with our guided session. Limited spots!
                </li>
                <li class="event-item">
                    <span class="font-semibold text-green-700">2025-08-30:</span> **Competition Grand Finale & Awards Ceremony** - Save the date for the big reveal!
                </li>
            </ul>
        </div>

        <!-- Leaderboard Footer / Update Info -->
        <div class="bg-gray-100 p-4 sm:p-6 text-center text-sm text-gray-600 rounded-b-xl">
            <p>Leaderboard updated daily. Keep earning points!</p>
            <p class="mt-1">Next update: 2025-06-25 09:00 AM</p>
            <!-- Link to Google Sheet -->
            <p class="mt-2 text-blue-600 hover:text-blue-800 transition duration-200 ease-in-out">
                <a href="[https://docs.google.com/spreadsheets/d/YOUR_GOOGLE_SHEET_ID_HERE/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1IIH_ARCpfkEyr3Ztlk-CYK3gZQiPVf32HK3m3fCuzcM/edit?usp=sharing)" target="_blank" rel="noopener noreferrer" class="underline">
                    View/Edit Raw Data in Google Sheet
                </a>
            </p>
        </div>
    </div>
</body>
</html>
