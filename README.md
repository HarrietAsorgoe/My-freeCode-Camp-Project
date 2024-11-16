# My-freeCode-Camp-Project
To fulfill the user stories and pass all the tests for your survey form project, here is the updated HTML structure with the required elements. This should help you complete the project and pass the tests.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Survey Form</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="form-container">
        <!-- Title of the form -->
        <h1 id="title">Survey Form</h1>
        
        <!-- Short description of the form -->
        <p id="description">We would love to get your feedback. Please fill out this short survey.</p>
        
        <!-- Survey Form -->
        <form id="survey-form">
            <!-- Name input field -->
            <label id="name-label" for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your name" required>

            <!-- Email input field -->
            <label id="email-label" for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required>

            <!-- Number input field -->
            <label id="number-label" for="number">Age:</label>
            <input type="number" id="number" name="age" min="1" max="120" placeholder="Enter your age" required>

            <!-- Dropdown selection -->
            <label for="dropdown">How did you hear about us?</label>
            <select id="dropdown" name="source">
                <option value="friends">Friends</option>
                <option value="social-media">Social Media</option>
                <option value="advertisement">Advertisement</option>
            </select>

            <!-- Radio button group -->
            <p>How satisfied are you with our service?</p>
            <label>
                <input type="radio" name="satisfaction" value="very-satisfied"> Very Satisfied
            </label>
            <label>
                <input type="radio" name="satisfaction" value="satisfied"> Satisfied
            </label>
            <label>
                <input type="radio" name="satisfaction" value="neutral"> Neutral
            </label>

            <!-- Checkbox group -->
            <p>What services did you use? (Select all that apply)</p>
            <label>
                <input type="checkbox" name="services" value="service1"> Service 1
            </label>
            <label>
                <input type="checkbox" name="services" value="service2"> Service 2
            </label>
            <label>
                <input type="checkbox" name="services" value="service3"> Service 3
            </label>

            <!-- Textarea for additional comments -->
            <label for="comments">Additional Comments:</label>
            <textarea id="comments" name="comments" rows="4" placeholder="Share your thoughts here"></textarea>

            <!-- Submit button -->
            <button type="submit" id="submit">Submit</button>
        </form>
        
        <div id="response-message"></div>
    </div>

    <script src="script.js"></script>
</body>
</html>

