# Zoom Meeting Link Generation

This Python script utilizes the Zoom API to create a Zoom meeting. It retrieves an access token using OAuth, then sends a request to the Zoom API to create a meeting with specified details such as the topic, duration, start date, and start time.

## Prerequisites

Before using this script, make sure you have:

- Zoom Developer Account
- Client ID, Account ID, and Client Secret from your Zoom App
- Python installed on your system
- Required Python packages installed (`requests`)

# Zoom App Configuration

## 1. App Creation

- Accessed the Zoom App Marketplace and initiated the app creation process.
- Clicked on the "Develop" dropdown and selected "Build Server-to-Server App."
- Named the app "[App Name]" for clarity.
- Securely recorded the app credentials (Account ID, Client ID, Client Secret).

## 2. Information and Features

- Provided a brief description of the app's purpose.
- Included developer contact information for activation and communication.

## 3. Scope Selection

### Get a meeting's encoded SIP URI:

- Enables integration with SIP-based conferencing systems.
- Allows retrieval of encoded SIP URIs for scheduled Zoom meetings.

### View and manage all user meetings:

- Grants comprehensive access to view, create, modify, and delete meetings for all users.
- Essential for planned functionalities.

## 4. Activation

- Thoroughly reviewed all configurations and activated the app.

## Setup

1. **Replace the placeholder values in the script:**
    - `client_id`: Replace with your Zoom App's Client ID.
    - `account_id`: Replace with your Zoom account ID.
    - `client_secret`: Replace with your Zoom App's Client Secret.


## Usage

Modify the `create_meeting` function parameters to customize the Zoom meeting details:

```python
create_meeting(
    "Test Zoom Meeting",
    "60",
    "2024-01-12",
    "20:29",
)

## Output

Upon successful execution, the script will print the generated Zoom meeting link. 

Feel free to enhance and adapt this script according to your specific requirements. If you encounter any issues, refer to the [Zoom API documentation](https://marketplace.zoom.us/docs/api-reference/introduction) for further assistance.
