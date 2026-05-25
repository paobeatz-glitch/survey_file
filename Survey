<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Invitation ☕</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #fdfbf7 0%, #f5ece1 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
            color: #4a3b32;
        }

        .container {
            background: #ffffff;
            max-width: 500px;
            width: 100%;
            border-radius: 24px;
            box-shadow: 0 15px 35px rgba(139, 115, 85, 0.15);
            padding: 35px;
            text-align: center;
            border: 1px solid rgba(230, 215, 200, 0.6);
            transition: all 0.4s ease;
        }

        .icon {
            font-size: 48px;
            margin-bottom: 15px;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        h1 {
            font-size: 26px;
            color: #61483b;
            margin-bottom: 15px;
            font-weight: 700;
        }

        p {
            font-size: 16px;
            line-height: 1.6;
            color: #6e5d53;
            margin-bottom: 25px;
        }

        .highlight-box {
            background-color: #faf5f0;
            border-left: 4px solid #b19482;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 30px;
            font-style: italic;
            text-align: left;
            font-size: 14.5px;
        }

        .options-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            text-align: left;
        }

        .option-card {
            border: 2px solid #ebdcd0;
            border-radius: 12px;
            padding: 15px;
            cursor: pointer;
            transition: all 0.2s ease;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .option-card:hover {
            border-color: #b19482;
            background-color: #faf6f2;
        }

        .option-card input[type="radio"] {
            accent-color: #8c6d58;
            width: 18px;
            height: 18px;
            cursor: pointer;
        }

        .option-label {
            font-size: 16px;
            font-weight: 600;
            color: #524136;
            cursor: pointer;
            width: 100%;
        }

        .custom-date-container {
            margin-top: 12px;
            padding-left: 30px;
            display: none;
            width: 100%;
        }

        .inputs-wrapper {
            display: flex;
            flex-direction: column;
            gap: 10px;
            width: 100%;
        }

        .custom-date-input {
            width: 100%;
            padding: 10px 15px;
            border: 1px solid #d1bfb3;
            border-radius: 8px;
            font-size: 14px;
            color: #4a3b32;
            background-color: #fff;
            outline: none;
            transition: border-color 0.2s;
        }

        .custom-date-input:focus {
            border-color: #8c6d58;
            box-shadow: 0 0 0 3px rgba(140, 109, 88, 0.15);
        }

        input[type="date"] {
            font-family: inherit;
            cursor: pointer;
        }

        .submit-btn {
            margin-top: 25px;
            background-color: #8c6d58;
            color: #ffffff;
            border: none;
            padding: 14px 28px;
            font-size: 16px;
            font-weight: 600;
            border-radius: 12px;
            cursor: pointer;
            width: 100%;
            transition: background-color 0.2s, transform 0.1s;
            box-shadow: 0 4px 10px rgba(140, 109, 88, 0.2);
        }

        .submit-btn:hover {
            background-color: #735947;
        }

        .submit-btn:active {
            transform: scale(0.98);
        }

        /* Thank You Screen Styles */
        .result-screen {
            display: none;
            text-align: center;
            animation: fadeIn 0.5s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .success-badge {
            background-color: #e6f4ea;
            color: #137333;
            padding: 6px 16px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            display: inline-block;
            margin-bottom: 20px;
        }

        .receipt-card {
            background: #fafafa;
            border: 2px dashed #d1bfb3;
            border-radius: 16px;
            padding: 25px;
            margin: 25px 0;
            text-align: left;
        }

        .receipt-row {
            margin-bottom: 12px;
            font-size: 15px;
        }

        .receipt-row:last-child {
            margin-bottom: 0;
        }

        .receipt-label {
            color: #8c7669;
            font-weight: 500;
        }

        .receipt-value {
            color: #33251d;
            font-weight: 700;
            margin-top: 4px;
            font-size: 17px;
        }

        .screenshot-instruction {
            font-size: 13px;
            color: #8c7669;
            background-color: #f0ebe6;
            padding: 10px;
            border-radius: 8px;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            justify-content: center;
            width: 100%;
            font-weight: 500;
        }
    </style>
</head>
<body>

    <div class="container" id="invitationCard">
        <div id="formView">
            <div class="icon">☕</div>
            <h1>Coffee Date?</h1>
            <p>I would absolutely love to grab a coffee with you anytime or any day this week! I'm genuinely thrilled to get to know you better and share some good conversation.</p>
            
            <div class="highlight-box">
                <strong>Gentle reminder:</strong> You just need to prepare and show up! Absolutely no actions or planning are needed on your end. I'll take care of everything. ✨
            </div>

            <form class="options-form" id="dateForm">
                <label class="option-card" for="optYes">
                    <input type="radio" id="optYes" name="dateOption" value="Yes! Let's do it." required onclick="toggleCustomDate(false)">
                    <span class="option-label">Yes! Let's do it.</span>
                </label>

                <label class="option-card" for="optAbsolutely">
                    <input type="radio" id="optAbsolutely" name="dateOption" value="Absolutely! Count me in." onclick="toggleCustomDate(false)">
                    <span class="option-label">Absolutely! Count me in.</span>
                </label>

                <label class="option-card" for="optCustom" style="flex-wrap: wrap;">
                    <input type="radio" id="optCustom" name="dateOption" value="Custom Date" onclick="toggleCustomDate(true)">
                    <span class="option-label">I'd love to! Here is a day/time that works for me...</span>
                    
                    <div class="custom-date-container" id="customDateContainer">
                        <div class="inputs-wrapper">
                            <input type="date" id="customDatePicker" class="custom-date-input">
                            <input type="text" id="customTimeInput" class="custom-date-input" placeholder="Preferred time (e.g., After 5 PM, or lunch time)">
                        </div>
                    </div>
                </label>

                <button type="submit" class="submit-btn">Confirm My Choice ✨</button>
            </form>
        </div>

        <div id="resultView" class="result-screen">
            <div class="success-badge">✓ It's an official date!</div>
            <h1>Thank You & See You Soon! ☕</h1>
            <p>I cannot wait! Everything is set on your end. Here is a summary of your response:</p>

            <div class="receipt-card">
                <div class="receipt-row">
                    <div class="receipt-label">Your Response:</div>
                    <div class="receipt-value" id="finalResponse">--</div>
                </div>
                <div style="height: 1px; background-color: #ebdcd0; margin: 15px 0;"></div>
                <div class="receipt-row">
                    <div class="receipt-label">Your Only Task:</div>
                    <div class="receipt-value" style="color: #8c6d58;">Just dress up, show up, and relax!</div>
                </div>
            </div>

            <div class="screenshot-instruction">
                📸 Take a screenshot of this page & send it back to me!
            </div>
        </div>
    </div>

    <script>
        function toggleCustomDate(show) {
            const container = document.getElementById('customDateContainer');
            const datePicker = document.getElementById('customDatePicker');
            
            if (show) {
                container.style.display = 'block';
                datePicker.required = true;
                datePicker.focus();
            } else {
                container.style.display = 'none';
                datePicker.required = false;
            }
        }

        // Set minimum pickable date to today's date dynamically
        const today = new Date().toISOString().split('T')[0];
        document.getElementById('customDatePicker').setAttribute('min', today);

        // Submission handler to map values cleanly to the final confirmation card
        document.getElementById('dateForm').addEventListener('submit', function(event) {
            event.preventDefault(); 
            
            const selectedOption = document.querySelector('input[name="dateOption"]:checked');
            let finalChoiceText = "";

            if (selectedOption.value === "Custom Date") {
                const chosenDate = document.getElementById('customDatePicker').value;
                const chosenTime = document.getElementById('customTimeInput').value.trim();
                
                // Format the chosen calendar date nicely (YYYY-MM-DD to a readable string)
                let dateObject = new Date(chosenDate + "T00:00:00");
                let formattedDate = dateObject.toLocaleDateString('en-US', { 
                    weekday: 'long', 
                    month: 'short', 
                    day: 'numeric' 
                });

                // Combine chosen calendar date with the time details if they entered any
                if (chosenTime) {
                    finalChoiceText = `Free on ${formattedDate} (${chosenTime})`;
                } else {
                    finalChoiceText = `Free on ${formattedDate}`;
                }
            } else {
                finalChoiceText = selectedOption.value;
            }

            // Insert response text into summary block
            document.getElementById('finalResponse').innerText = finalChoiceText;

            // Transition screens smoothly
            document.getElementById('formView').style.display = 'none';
            document.getElementById('resultView').style.display = 'block';
            
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });
    </script>
</body>
</html>
