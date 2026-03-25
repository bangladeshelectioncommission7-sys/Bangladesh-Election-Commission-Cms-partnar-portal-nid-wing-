# EC OTP Vercel Project

## Files
- index.html
- api/send-otp.js
- vercel.json
- .env.example
- package.json

## Environment Variables
Set these in Vercel Project Settings -> Environment Variables

- SMS_API_URL
- SMS_API_KEY
- SMS_FROM
- SMS_UNICODE
- SMS_ACTION
- OTP_MESSAGE_TEMPLATE

## Example
SMS_API_URL=https://sms.one9.one/sms/api
SMS_API_KEY=YOUR_API_KEY
SMS_FROM=sms
SMS_UNICODE=1
SMS_ACTION=send-sms
OTP_MESSAGE_TEMPLATE=বাংলাদেশ নির্বাচন কমিশন (NID সেবা): আপনার OTP কোড {{OTP}}। এটি ৫ মিনিটের জন্য প্রযোজ্য। কারো সাথে শেয়ার করবেন না।

## Health Check
Open:
https://your-domain.vercel.app/api/send-otp

If working, it returns:
OTP API is running
