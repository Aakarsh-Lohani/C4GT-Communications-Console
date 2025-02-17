# Contributions-to-Karmayogi-Bharat
## C4GT Communications Console

API Usage and Showcase : https://youtu.be/fxzCveuP0gM


Project Showcase: https://youtu.be/m1WGsx6s0j4


# Smart Email Notifier Documentation

## Overview

The Email Notifier Service is designed to streamline the process of sending notifications and managing email templates within an application. It provides a flexible interface for creating, configuring, and sending emails, as well as viewing user data and email history.

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

### Creating a Template

1. Select "Create Template" from the menu.
2. Fill in the template details in the provided form.
3. Submit the form to save the template.

### Configuring a Template

1. Select "Configure Template" from the menu.
2. Choose a template from the list of existing templates.
3. Make the necessary changes in the configuration interface.
4. Save the changes to update the template.

### Viewing User Data

Select "View User Data" from the menu to display a list of user data, filter and select users to send email.

### Uploading User Data

1. Select "Upload User Data" from the menu.
2. Use the interface to upload user data files.
3. Confirm the upload to make the data available for email targeting.

### Sending an Email

1. Select "Send Email" from the menu.
2. Choose a template and configure the necessary details.
3. Preview the email before sending.
4. Upload an attachment (optional).
5. Submit the form to send the email to the selected recipients.

### Viewing History

Select "History" from the menu to view a log of sent emails, including timestamps and recipient details.

## Conclusion

The Smart Email Notifier provides a comprehensive suite of tools for managing email notifications within an application. By leveraging its components, users can efficiently create, send, and track emails, ensuring effective communication with their audience.
