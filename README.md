# ekg-interpretation
Project for Human Computer Interaction class where myself and Nick Landers design a web app that takes CSV data that represent an EKG reading and returns a statistical analysis of the results to the nurse.

Tech stack:

    Frontend:
        Tailwind CSS
            https://tailwindcss.com/docs/installation
            https://tailwindcss.com/docs/configuration
    Backend:
        Python with Flask
            https://flask.palletsprojects.com/en/3.0.x/installation/
            https://flask.palletsprojects.com/en/3.0.x/quickstart/

To run the web app:
First execute '. .venv/bin/activate'
Next, run 'flask --app app run'

Each row in the patient csv files corresponds to an EKG reading. The first row is the
most recent reading and the third row represents that patient's previous reading.

TODO:
    - Handle edge case in which patient is visiting for the first time, and display
    "Patient's first EKG reading on record" in the "stability change" section.