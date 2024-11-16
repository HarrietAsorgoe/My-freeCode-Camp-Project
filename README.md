# My-freeCode-Camp-Project

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

/* General body styling */
body {
    font-family: Arial, sans-serif;
    background-color: #f7f7f7;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

/* Form container */
.form-container {
    background: #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    padding: 20px 30px;
    width: 100%;
    max-width: 400px;
    text-align: center;
}

/* Title and description */
#title {
    color: #333333;
    margin-bottom: 10px;
}

#description {
    color: #666666;
    font-size: 0.9rem;
    margin-bottom: 20px;
}

/* Form styling */
form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

/* Labels */
label {
    text-align: left;
    color: #333333;
    font-size: 0.9rem;
    font-weight: bold;
}

/* Inputs, select, textarea */
input, select, textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #cccccc;
    border-radius: 5px;
    font-size: 0.9rem;
    color: #333333;
    outline: none;
}

input:focus, select:focus, textarea:focus {
    border-color: #4CAF50;
    box-shadow: 0 0 5px rgba(76, 175, 80, 0.5);
}

/* Placeholder color */
input::placeholder, textarea::placeholder {
    color: #aaaaaa;
}

/* Radio and checkbox alignment */
input[type="radio"], input[type="checkbox"] {
    margin-right: 8px;
}

/* Submit button */
#submit {
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    padding: 10px;
    font-size: 1rem;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

#submit:hover {
    background-color: #45a049;
}

/* Responsive design */
@media (max-width: 480px) {
    .form-container {
        padding: 15px 20px;
    }

    form {
        gap: 10px;
    }
}
