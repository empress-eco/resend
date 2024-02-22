<div align="center">
![Empress Resend Integration Logo](https://grow.empress.eco/uploads/default/original/2X/1/1f1e1044d3864269d2a613577edb9763890422ab.png
<p align="center">
Unleash the power of automated email marketing with Empress Resend Integration.
<br />
<a href="https://grow.empress.eco/">Explore the Docs</a>
·
<a href="https://github.com/empress-eco/resend/issues">Report Bug</a>
·
<a href="https://github.com/empress-eco/resend/issues">Request Feature</a>
</p>
</div>

## About The Project

### 📖 Overview
Empress Resend Integration is a robust tool designed to connect your Empress instance with the [Resend](https://resend.com) platform, transforming your email marketing efforts. It's an ideal solution for businesses aiming to automate their email workflows, reach larger audiences, and enhance their impact.

### ✨ Key Features
- Effortlessly send broadcast emails directly from your Empress instance.
- Utilize API to dispatch emails from your custom app or server scripts.
- Webhook setup for smooth and flawless integration.

## Getting Started

### Prerequisites
To get started, ensure you have bench set up. For more detailed information, kindly refer to [this documentation](https://Empressframework.com/docs/v14/user/en/installation).

### Installation
To install the app, simply clone the repository and install it on your site using the following commands:

```sh
git clone https://github.com/empress-eco/resend.git
bench --site <site-name> install-app resend_integration
```

### Setup
Initially, generate an API key from your [Resend](https://resend.com) dashboard and paste it in **Resend Settings** in your Empress instance.

For webhook setup, use this URL:

```
https://<your-site-domain>/api/method/resend_integration.api.handle_resend_webhook
```
Copy the signing secret from your webhook dashboard on Resend and paste it in **Resend Settings** in your Empress instance.

### Usage
Use the **Resend Broadcast Email** DocType to send broadcast emails. You can also send emails from your custom app using a straightforward Python script.

```python
from resend_integration.api import send_resend_emails

send_resend_emails(
 "Get discount!",
 from_email="notifications@buildwithhussain.dev",
 to_emails=["faris@Empress.io"],
 email_html="<h1>Hey!</h1>",
 reply_to="hussain@Empress.io",
)
```
> Note: Ensure your domain is verified before you can use it to send emails.

## Contributing
We warmly welcome all contributions! Here's how you can contribute:

- Fork the Project
- Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
- Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
- Push to the Branch (`git push origin feature/AmazingFeature`)
- Open a Pull Request

## License and Acknowledgements

### License
This project is licensed under the MIT License. Your contributions are equally licensed under the MIT License.

### Acknowledgements
We express our heartfelt gratitude to the Empress Community for their foundational contributions to this project. Their innovative tools and constant support have been instrumental in building the functionalities we rely on. We appreciate their pioneering work and ongoing commitment.