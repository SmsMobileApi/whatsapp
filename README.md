# whatsapp
Easily connect WhatsApp to SMSMobileAPI to send messages via API requests using your own number. Enjoy full control, seamless integration, and real-time message visibility in your WhatsApp app. Perfect for businesses seeking efficient communication!

# WhatsApp Messaging with SMSMobileAPI

Easily send WhatsApp messages via the SMSMobileAPI using simple API requests. With this integration, messages are sent directly from your WhatsApp-linked phone number, ensuring full transparency and seamless communication.

---

## API Endpoint for Sending WhatsApp Messages

### Endpoint
https://api.smsmobileapi.com/sendsms


---

## Parameters

| Parameter   | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `apikey`    | Your unique API key (generated when you create an account on SMSMobileAPI). |
| `recipients`| The recipient's phone number (must be available on WhatsApp).               |
| `message`   | The message to send (supports multi-line messages).                         |
| `waonly`    | Must be set to `yes` to specify that only a WhatsApp message is sent.       |

---

## Example Request

### GET Request
GET https://api.smsmobileapi.com/sendsms?apikey=YOUR_API_KEY&waonly=yes&recipients=+1234567890&message=Hello%20World


### Decoded Example
```plaintext
https://api.smsmobileapi.com/sendsms?apikey=YOUR_API_KEY&waonly=yes&recipients=+1234567890&message=Hello World


Step-by-Step Guide

1. Create an Account
   - Sign up or log in to SMSMobileAPI to generate your unique API key.
   - Manage your account here: [Create or Manage Your Account](https://smsmobileapi.com/fr/connect/).

2. Prepare Your Request
   - Replace `YOUR_API_KEY` with your actual API key.
   - Replace `+1234567890` with the recipient's WhatsApp-enabled phone number.
   - Replace `Hello%20World` with your desired message.

3. Send the Request
   - Use a tool like Postman, cURL, or your server's HTTP client to send the GET request.

4. Receive the Response
   - Upon success, the API will return a response confirming the message was sent.
