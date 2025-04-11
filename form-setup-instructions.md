# Contact Form Setup Instructions

The website is using [Formspree](https://formspree.io/) to handle the contact form submissions without requiring any backend development. Follow these steps to set it up:

## Setting Up Formspree

1. **Create a Formspree Account**
   - Go to [Formspree.io](https://formspree.io/) and sign up for an account
   - The free tier allows up to 50 submissions per month

2. **Create a New Form**
   - In your Formspree dashboard, click "New Form"
   - Give your form a name (e.g., "Shalom Therapy Contact")
   - Choose the email where you want to receive the form submissions (e.g., info@shalomtherapy.in)

3. **Get Your Form Endpoint**
   - After creating the form, Formspree will provide you with a unique form endpoint URL 
   - It will look something like: `https://formspree.io/f/xrgdopwz`

4. **Update Your Website Code**
   - Open the `index.html` file
   - Find the form action attribute: `<form action="https://formspree.io/f/yourformspree" method="POST">`
   - Replace `yourformspree` with your actual form ID from step 3

5. **Test the Form**
   - Visit your website and fill out the contact form
   - Submit a test message
   - Check your email to confirm you received the submission
   - Also check your Formspree dashboard to see the submission there

## Form Features

- **Form Validation**: Required fields must be filled out before submission
- **Success Feedback**: Users will see a confirmation message when their message is sent
- **Error Handling**: If there's a problem, users will see an error message
- **Spam Protection**: Formspree includes built-in spam protection

## Customizing Email Notifications

In your Formspree dashboard, you can:
- Customize the email subject line
- Add multiple recipients
- Set up auto-responses
- Integrate with other services (premium feature)

## Troubleshooting

- If form submissions aren't coming through, check your spam folder
- Verify that the form endpoint URL is correctly entered in the HTML
- Ensure your website is properly deployed and accessible

For additional help, refer to the [Formspree documentation](https://help.formspree.io/) 