# Instant-Multi-Language-Translation-Bot-
An instant multi-language translation bot that accepts text input in any language, detects the source language using AI, and replies with English translation. Built with n8n workflow automation.


# Multi-Language Translation Bot

A WhatsApp bot that accepts text in any language and replies with English translation using AI.

## Features

- Accepts text input in any language (Urdu, Spanish, French, Arabic, Turkish, German, and more)
- Automatically detects the source language
- Translates the message to English
- Replies instantly to the user on WhatsApp

## How It Works

User sends WhatsApp message in any language -> Bot receives message -> AI detects language -> AI translates to English -> Bot sends translated text back to user on WhatsApp

## Tech Stack

- n8n for workflow automation
- AI Translation API for language detection and translation
- WhatsApp API for messaging

## Prerequisites

- n8n installed (self-hosted or cloud version)
- WhatsApp account
- AI Translation API key (OpenAI, Google Translate, or FluentC)

## Setup Instructions

1. Connect WhatsApp to n8n
   - Install WhatsApp community node in n8n (WhatsApp Trigger)
   - Scan QR code from n8n using your WhatsApp mobile app
   - Your WhatsApp number will be connected

2. Import Workflow to n8n
   - Download the workflow.json file from this repository
   - Open n8n and go to Workflows
   - Click Import from File and select the downloaded JSON file

3. Configure Credentials
   - For WhatsApp Trigger: Ensure your WhatsApp session is connected
   - For AI Translation Node: Add your API key

4. Activate the Workflow
   - Turn on the workflow
   - Send a message to your WhatsApp number from any other number
   - You will receive the English translation as a reply

## Testing Results

Tested languages and their translations:

Spanish: Hola, como estas? -> Hello, how are you?

French: Bonjour! J'espere que vous passez une excellente journee -> Hello! I hope you're having a great day

Urdu: Aaj ka din bohat khoobsurat hai -> Today is a very beautiful day

Arabic: Marhaba! Atamanna an yakoma yawmuka jameelan -> Hello! I hope your day is beautiful

German: Hallo! Ich hoffe du hast einen produktiven Tag -> Hello! I hope you have a productive day

Turkish: Merhaba! Bugun yeni seyler ogrenmek icin harika bir gun -> Hello! Today is a great day to learn new things

## Project Files

- workflow.json - The n8n workflow export
- README.md - Project documentation

