# AI Media Generation Automation

An automated media generation workflow built with n8n that combines AI content processing, image generation, video generation, job monitoring, and Telegram delivery in a single pipeline.

The workflow is designed to handle the full generation cycle automatically, from preparing the input content to delivering the final generated media.

## Features

- Scheduled workflow execution
- Content retrieval and preprocessing
- AI-assisted content generation using Google Gemini
- Structured JSON output parsing
- Rule-based routing between image and video generation flows
- Image generation using Google Imagen
- Video generation using Google Veo
- Video generation using HeyGen
- Asynchronous job status polling
- Automatic retrieval of generated media
- Telegram delivery
- Execution status tracking and logging

## Technologies

- n8n
- Google Gemini
- Google Imagen
- Google Veo
- HeyGen
- Telegram Bot API
- REST APIs
- JSON

## Workflow

The workflow follows this process:

1. The workflow is triggered on a defined schedule.
2. Input data is retrieved from the configured data source.
3. Gemini processes the input and generates structured content.
4. The output is parsed into JSON.
5. The workflow selects the appropriate generation path based on the requested media type.
6. Images are generated through Imagen, while videos are generated through Veo or HeyGen.
7. Long-running generation jobs are monitored until completion.
8. The generated media is retrieved automatically.
9. The final result is sent through Telegram.
10. The execution result is recorded for tracking and monitoring.

## Workflow Architecture

<img width="1862" height="914" alt="image" src="https://github.com/user-attachments/assets/c36c5a23-6f3a-4f74-9354-59b4f38378a6" />

## Setup

1. Import the workflow JSON file into n8n.
2. Configure the required credentials.
3. Update the API endpoints and data sources where needed.
4. Configure the Telegram destination.
5. Test the workflow nodes individually.
6. Activate the workflow.

## Security

Credentials, API keys, tokens, and other sensitive values are not included in this repository.

The workflow requires users to configure their own credentials before execution.

## Author

Ahmad Butmah
