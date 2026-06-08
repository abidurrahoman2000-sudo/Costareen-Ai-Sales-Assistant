# Costareen AI Sales Assistant

## Project Overview

Costareen AI Sales Assistant is an n8n-based AI chatbot workflow designed for a business that sells 3D printers, filaments, and accessories. The assistant works like a human sales representative and helps customers by answering product questions, checking stock availability, and giving quick buying guidance.

The workflow uses Google Gemini as the AI model and connects with Google Sheets to read product stock and sales-related data.

## Problem It Solves

Many small businesses receive repeated customer messages about product availability, prices, recommendations, and basic sales information. Replying manually to every message takes time and can delay customer decisions.

This project solves that problem by creating an automated AI sales assistant that can:

- Respond to customer questions instantly
- Check product availability from a Google Sheet
- Give helpful product suggestions
- Communicate naturally in English, Bangla, and Banglish
- Reduce manual workload for sales staff
- Improve customer response time
- Help close sales faster

For a 3D printing business like Costareen, customers often ask about filaments, printers, colors, stock, and accessories. This assistant can answer those questions quickly without needing a human staff member every time.

## Solution

The solution is an AI-powered sales assistant built with n8n. When a customer sends a chat message, the workflow sends that message to an AI Agent. The AI Agent uses Google Gemini to understand the message and respond naturally.

The assistant can also use Google Sheets as a tool to check product stock and sales data. This allows the chatbot to answer customer questions using real business information instead of only giving general replies.

## How The Workflow Works

1. A customer sends a chat message.
2. The n8n Chat Trigger receives the message.
3. The message is passed to the AI Agent.
4. The AI Agent uses Google Gemini to generate a response.
5. The AI Agent checks Google Sheets when stock or sales information is needed.
6. The assistant replies to the customer in a short, polite, and natural style.

## Main Features

- AI-powered sales conversation
- Supports English, Bangla, and Banglish
- Replies in the same language used by the customer
- Checks product stock from Google Sheets
- Gives 3D printer, filament, and accessory advice
- Keeps short conversation memory
- Protects exact stock numbers by only saying available or out of stock
- Designed for real customer-facing sales support

## Tools And Technologies Used

- n8n
- Google Gemini AI
- Google Sheets
- LangChain AI Agent node
- Simple Memory node
- Chat Trigger node

## Workflow Structure

The workflow contains these main nodes:

- When chat message received
- AI Agent
- Google Gemini Chat Model
- Simple Memory
- Google Sheets stock lookup tool
- Google Sheets sales entry lookup tool

## Business Use Case

This project is useful for a business that sells 3D printers, filaments, and accessories. Instead of manually answering every customer message, the AI assistant can handle common sales questions and guide customers toward the right product.

Example customer questions:

- White filament available?
- Which 3D printer is good for beginners?
- Do you have PLA filament?
- Price koto?
- Accessories available ase?

The assistant can answer in a friendly and local style, making the customer experience feel more natural.

## Setup Instructions

To use this workflow:

1. Download or clone this GitHub repository.
2. Open n8n.
3. Import the workflow JSON file.
4. Connect your own Google Gemini API credential.
5. Connect your own Google Sheets credential.
6. Select your own Google Sheet for stock and sales data.
7. Test the workflow using the chat trigger.
8. Activate the workflow when everything is working correctly.

## Important Note About Credentials

This project does not include private API keys, passwords, or login credentials. Anyone importing this workflow into n8n must connect their own:

- Google Gemini API credential
- Google Sheets credential
- Google Sheet data source

Do not upload API keys, passwords, tokens, `.env` files, or private customer data to GitHub.

## Files Included

- `Costareen_AI_sales_Assistant.json` - exported n8n workflow
- `Costareen_AI_sales_Assistant_photo.png` - screenshot of the workflow
- `README.md` - project explanation and documentation

## Future Improvements

In the future, this project can be improved by adding:

- WhatsApp or Messenger integration
- Automatic sales entry creation
- Order confirmation system
- Customer lead collection
- Product recommendation based on budget
- Admin notification when a customer is ready to buy
- Better analytics for customer questions

## Conclusion

Costareen AI Sales Assistant shows how AI automation can support small businesses by reducing repetitive manual work and improving customer response time. By combining n8n, Google Gemini, and Google Sheets, the workflow creates a practical sales assistant that can answer customer questions and support faster sales communication.
