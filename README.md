How It Works:
Password Evaluation (evaluate_password_strength function):

Length: The password must be at least 8 characters long.
Uppercase Letters: At least one uppercase letter is required.
Lowercase Letters: At least one lowercase letter is required.
Digits: The password should contain at least one digit.
Special Characters: The password should include at least one special character (e.g., !, @, #).
Each criterion is checked using regex:

r'[A-Z]': Matches any uppercase letter.
r'[a-z]': Matches any lowercase letter.
r'\d': Matches any digit.
r'[!@#$%^&*(),.?":{}|<>]': Matches any special character.
Password Strength Meter:

The strength score is calculated by how many criteria are met (maximum score of 5).
The st.progress() bar visually represents the strength as a progress bar (multiplying the score by 20).
The strength level is displayed with corresponding labels: "Very Weak," "Weak," "Fair," "Strong," and "Very Strong."
Suggestions:

If the password doesn't meet the required criteria, feedback and suggestions are shown to the user to improve their password.
