# Employee Activity Tracker

## Project Description

The **Employee Activity Tracker** is a Python-based desktop agent application designed to monitor and track employee activity. It captures relevant data, such as screenshots, and uploads it to a cloud storage service like Amazon S3. This application aims to provide comprehensive tracking features while ensuring compliance with best software development practices.

## Features

- **Activity Monitoring:** Tracks genuine user activity to ensure accurate data collection.
- **Screenshot Capture:** Periodically takes screenshots after every 60 seconds to record user activity.
- **Cloud Storage Integration:** Uploads captured data to Amazon S3 or a similar cloud storage service.
- **Configuration Management:** Handles configuration changes dynamically to adapt to different environments.
- **Robust Design:** Adheres to best practices in software development, including error handling and logging.

## Installation

1. **Create a Virtual Environment:**

    ```bash
    python -m venv C:\V_E\venv
    ```

2. **Activate the Virtual Environment:**

    - On Windows:

        ```bash
        venv\Scripts\activate\Activate.ps1
        ```

    - On macOS/Linux:

        ```bash
        source venv/bin/activate.ps1
        ```

3. **Install Required Dependencies:**

    ```bash
    pip install boto3
    pip install pynput
    pip install win32gui
    pip install pillow
    ```

4. **Configure the Application:**

    Create a configuration file named `config.json` in the root directory with the necessary settings for cloud storage and other configurations.

5. **Run the Application:**

    ```bash
    python user_activity_monitor.py
    ```

## Configuration

The application configuration is managed through a `config.json` file. Below is a sample configuration file:


# Several steps to S3 configuration roles:-
-> Created a IAM role in AWS and attached the policy(S3 full access) to create a custom password.
-> Attached json file in bucket policy.
-> After configuring and completing the above steps ,the screenshots are now stored in the S3 bucket. 


cloud_storage: Configuration details for the cloud storage service.
screenshot: Settings related to screenshot capture intervals.

Acknowledgments
Amazon S3 for cloud storage services.
Python for the programming language.
GitHub for hosting the repository.



# Conclusion:-
we can add more additional features to this application like Authentication , Dashboards for the admins .

![screenshot_20240831_165037](https://github.com/user-attachments/assets/ab73924d-4bf5-44b5-a476-22428a73dd8e)


![screenshot_20240831_165102](https://github.com/user-attachments/assets/846c44a5-7b71-4111-b40b-1f035e972c26)


![Screenshot 2024-08-31 180554](https://github.com/user-attachments/assets/89b2e9cc-ebe2-42de-bc72-886c7169ea6a)

