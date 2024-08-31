# Employee Activity Tracker

## Project Description

The **Employee Activity Tracker** is a Python-based desktop agent application designed to monitor and track employee activity. It captures relevant data, such as screenshots, and uploads it to a cloud storage service like Amazon S3. This application aims to provide comprehensive tracking features while ensuring compliance with best software development practices.

## Features

- **Activity Monitoring:** Tracks genuine user activity to ensure accurate data collection.
- **Screenshot Capture:** Periodically takes screenshots to record user activity.
- **Cloud Storage Integration:** Uploads captured data to Amazon S3 or a similar cloud storage service.
- **Configuration Management:** Handles configuration changes dynamically to adapt to different environments.
- **Robust Design:** Adheres to best practices in software development, including error handling and logging.

## Installation

1. **Create a Virtual Environment:**

    ```bash
    python -m venv venv
    ```

2. **Activate the Virtual Environment:**

    - On Windows:

        ```bash
        venv\Scripts\activate\Activate.ps1
        ```

    - On macOS/Linux:

        ```bash
        source venv/bin/activate
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

```json
{
  "cloud_storage": {
    "service": "amazon_s3",
    "bucket_name": "your-bucket-name",
    "access_key": "your-access-key",
    "secret_key": "your-secret-key"
  },
  "screenshot": {
    "interval": 300
  }
}



cloud_storage: Configuration details for the cloud storage service.
screenshot: Settings related to screenshot capture intervals.

Acknowledgments
Amazon S3 for cloud storage services.
Python for the programming language.
GitHub for hosting the repository.


**Previews:**
