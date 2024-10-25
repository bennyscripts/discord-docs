# Introduction

Thank you for considering contributing to this project! Any contribution is immensely valuable, and helps out the community in general.

## General Contribution Guidelines

1. **Structure**: Every new guide or documentation should follow this structure:
   - **Introduction**: Provide a summary of what the guide will cover.
   - **Instructions**: Each step must have code examples if needed.
   - **Code Blocks**: Use fenced code blocks with language specifiers for any code snippets. For example:
     \```python
     print("Hello World")
     \```
   - **Sections**: Split the document into clearly defined sections with headings.
   - **Sources**: Refer to related sources and/or additional resources.

2. **Language**: Use clear and concise language. Avoid unnecessary jargon. Make sure the instructions are accessible to both beginners and experienced developers.

3. **Consistency**: Follow the patterns of existing files such as:
   - `FIRST_BOT.md` for guides.
   - `CLASSIFY.md` for more technical, detailed content.

## Adding New Endpoints

When adding new endpoints to the `endpoints/` directory, ensure you follow those steps:
1. **Structure**:
   - Include the request method (`GET`, `POST`, etc.), endpoint URL, and an example of the request.
   - Include the response from the HTTP request, if any.

   Example:
   ```http
   GET https://discord.com/api/v10/users/@me
   Authorization: TOKEN
   ```
   Response:
    ```json
    {
        "id": "1234",
        "username": "harmlessaccount",
        "avatar": null,
        "discriminator": "0",
        "public_flags": 0,
        "flags": 0,
        "banner": null,
        "accent_color": null,
        "global_name": "Harmless",
        "avatar_decoration_data": null,
        "banner_color": null,
        "clan": null,
        "mfa_enabled": false,
        "locale": "en-US",
        "premium_type": 0,
        "email": "harm@less.net",
        "verified": true,
        "phone": null,
        "nsfw_allowed": true,
        "linked_users": [],
        "bio": "",
        "authenticator_types": []
    }
    ```
    
    Make sure that you include placeholder information instead of exposing your own.

Additionally, you may use my project: https://github.com/harmlessaccount/discord-url to test URLs, which provides a way to test URLs on a CLI, with TLS capabilities and a way to anonymize outputs automatically. After adding an URL to the `endpoints/` directory, please make sure to add it to the `discord-url` project.
