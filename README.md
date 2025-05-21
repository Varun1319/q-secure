# q-Secure
This was made for my college Mini Project for the 5th Semester.
Modern Chat Applications use End-to-End Encrytption, which typically uses algorithms like RSA, which can be broken with enough quantum computing power. <br> 

So I decided to build a chat client that can completely resist such attacks.

## Focus
My focus was to build a chat client that could theoretically resist quantum attacks breaking end to end encryption algorithms in the long run, and while I could not achieve that to the full extent, I did make a decent enough version for academic purposes.

## How to Run
You would require an App Password from google for the mailing features for the `Forgot Password` Section to work. <br>
<a href="https://support.google.com/accounts/answer/185833?hl=en">Refer this Google article to get your own App Password.</a>

1. Clone the repo

2. Navigate to the project folder and create a `.env` file with the following fields: <br><br>
   a. `MONGO_URI` <br>
   b. `SECRET_KEY` <br>
   c. `MAIL_USERNAME` <br>
   d. `MAIL_PASSWORD` <br>

3. Install the necessary packages to run the application by running `pip install -r requirents.txt`.
4. Run the app by running the command `python app.py`
5. Open your browser and navigate to `https://localhost:8000`


## Limitations 
1. This is a symmetric encryption algorithm
2. The quantum safe algorithm implemented is a One Time Padding (OTP) XOR encryption. In theory that would be quantum safe, but my implementation is very low level.
3. The key size is fixed.

## Contributing

Contributions are welcome! If you have suggestions for improvements or find any issues, please create an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new pull request.
