# WhatsApp Tag Contact List from Image Prompt

**Task:**  
Extract all phone numbers from the attached contact list image and output a single-line WhatsApp tagging string, formatted for tagging each number directly.

**Instructions:**  
- Read every phone number from the image (ignore names, just focus on the numbers).
- Use these formatting rules:  
  - For USA numbers: format as `@+1 (xxx) xxx-xxxx`
  - For Indian numbers: use `@+91 xxxxx xxxxx` **or** `@+91 xxxx xxx xxx` (pick the one seen in the image, or mention both if unsure)
  - For other countries: use `@+[country code] [full number, spaced as per the image]`
- Output all tags in one single line, separated by spaces, and ensure no numbers are missed.
- If unsure of Indian number grouping, provide both possible formats.

**Example output:**  
@+91 12345 67890 @+91 1234 567 890 @+1 (123) 456-7890 @+49 176 12345678


**Purpose:**  
This string will be used in WhatsApp group messaging to tag contacts by their phone numbers and ensure everyone receives the notification.
