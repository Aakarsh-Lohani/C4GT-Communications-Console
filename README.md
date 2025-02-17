## C4GT Communications Console (Contributions-to-Karmayogi-Bharat)

API Usage and Showcase : https://youtu.be/fxzCveuP0gM

# Smart Email Notifier

## Overview

The Smart Email Notifier App is designed to streamline the process of sending notifications and managing email templates within an application. It provides a flexible interface for creating, configuring, and sending emails, as well as viewing user data and email history.

## APIs

| Request      | Middleware                               | API                              |
|-------------|----------------------------------------|---------------------------------|
| GET         | anonymous, anonymous                  | `/api/email`                   |
| POST        | anonymous, multerMiddleware, anonymous | `/api/email/send-email`        |
| POST, GET   | anonymous, anonymous                  | `/api/email/templates`         |
| GET, PUT    | anonymous, anonymous                  | `/api/email/templates/:id`     |
| POST, GET   | anonymous, anonymous                  | `/api/email/users`             |
| POST        | anonymous, multerMiddleware, uploadUserData | `/api/email/upload-user-data` |
| GET         | anonymous, router                     | `/api/email/history`           |


![Docs](https://github.com/user-attachments/assets/59602f97-1b5f-4420-adae-f901f16abd8f)
## Tech Stack

This project uses the **MEAN** stack:

- MongoDB
- Express.js
- Angular
- Node.js

## Provider

The service provider for sending emails in this project is **Nodemailer**.

## Why We Are Using These Technologies

**MEAN Stack:** We are using the MEAN stack because it allows for a full-stack JavaScript solution, meaning both the client-side and server-side use the same language. This simplifies development and maintenance.

**Nodemailer:** We are using Nodemailer because it provides a simple and flexible way to send emails from our Node.js application. It supports various transport methods and allows for customization of email content.

## How We Are Using These Technologies

### MEAN Stack

- **MongoDB** is used as the database to store application data.
- **Express.js** is used as the web application framework to build the server-side logic.
- **Angular** is used to build the client-side application and manage the user interface.
- **Node.js** is used as the runtime environment to execute server-side code.

### Nodemailer

- We set up Nodemailer with a transporter configuration to connect to an email service provider (e.g., Gmail).
- We define email options such as sender, recipient, subject, and body content.
- We use the `sendMail` method to send emails from our Node.js application.

## Components

### Main Content Area

The main content area dynamically displays content based on the selected menu option. It supports the following functionalities:

- **Create Template**: Interface for creating new email templates.
- **Configure Template**: Allows users to configure existing email templates.
- **View User Data**: Displays user data relevant to the email service and allows selecting users to send emails.
- **Upload User Data**: Provides an option to upload user data for email targeting.
- **Send Email**: Interface for sending emails using configured templates.
- **History**: Shows the history of sent emails for tracking and auditing purposes.
- **Docs**: (default) Displays the documentation to understand the platform interface and learn about the project.

## Usage

### Navigation

Users can navigate through the service using a menu that changes the `selectedMenu` variable. This variable controls which component is displayed in the main content area.

### 1. Creating a Template
![Create](https://github.com/user-attachments/assets/a0d9e76d-162a-4475-b7cc-3e39a4a16711)
1. Select "Create Template" from the menu.
2. Fill in the template details in the provided form.
3. Submit the form to save the template.

### 2. Configuring a Template
![configure 1](https://github.com/user-attachments/assets/e5953910-d7f9-4e2a-84ab-f891301808cb)
![Edit template configure 1](https://github.com/user-attachments/assets/299c4adb-0cd9-44ea-af9e-7312ba0d291f)
![Configure Template Save](https://github.com/user-attachments/assets/20776af0-d580-407d-9c80-6a55222444c6)
1. Select "Configure Template" from the menu.
2. Choose a template from the list of existing templates.
3. Make the necessary changes in the configuration interface.
4. Save the changes to update the template.

### 3. Viewing User Data
![User Data](https://github.com/user-attachments/assets/6520e27f-bd41-425a-ba26-21699a25393f)
Select "View User Data" from the menu to display a list of user data, filter and select users to send email.

### 4. Uploading User Data

1. Select "Upload User Data" from the menu.
2. Use the interface to upload user data files.
3. Confirm the upload to make the data available for email targeting.

### 5. Sending an Email
![Send Email 1](https://github.com/user-attachments/assets/ae74cb29-7e00-4ba2-8183-84d8ac8d5ff6)
![Send](https://github.com/user-attachments/assets/a742a593-3e40-4f26-bfca-945792ef6f6b)
![Email Sent](https://github.com/user-attachments/assets/c80a994f-11ff-4c48-8dd8-b0761d5dd673)
![Received Email](https://github.com/user-attachments/assets/2407b4a3-8a6f-4f62-a434-7bcfdb095a0b)

1. Select "Send Email" from the menu.
2. Choose a template and configure the necessary details.
3. Preview the email before sending.
4. Upload an attachment (optional).
5. Submit the form to send the email to the selected recipients.

### 6. Viewing History
![History](https://github.com/user-attachments/assets/2fdf65c4-6389-414f-9ff0-6a399128914b)
Select "History" from the menu to view a log of sent emails, including timestamps and recipient details.

### 7. DATA BASE (MONGODB)
![DB Templates](https://github.com/user-attachments/assets/b788e4fb-9fa6-4378-b8ac-adb2b7a628b6)
![DB History](https://github.com/user-attachments/assets/5651cc85-d695-466b-b150-e4454c6a7e11)


## Conclusion

The Smart Email Notifier provides a comprehensive suite of tools for managing email notifications within an application. By leveraging its components, users can efficiently create, send, and track emails, ensuring effective communication with their audience.
