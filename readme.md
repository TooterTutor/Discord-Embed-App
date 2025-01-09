# Message Embedder
This is a Discord App that allows the user to send customized messages using Embeds written in JSON. Embeds are a way to add rich content to messages, such as information, images, and more.

## Embeds support the following features:
- **Title**: A title for the embed, which can be up to 256 characters long.
- **Description**: A description for the embed, which can be up to 2048 characters long.
- **Fields**: A list of fields, which can be up to 25 fields long. Each field can have a name, value, and inline flag.
- **Thumbnail**: An image to be displayed as a thumbnail.
- **Image**: An image to be displayed as the main image.
- **Footer**: A footer for the embed, which can be up to 2048 characters long.
- **Timestamp**: A timestamp for the embed, which can be up to 20 characters long.
- **Color**: A color for the embed in hexidecimal format, which can be up to 6 characters long.

## Usage
To send an embed, simply type `/embed send` followed by the JSON data for the embed. <br>
To edit an existing embed sent by the app, type `/embed edit` followed by the messageId of the embed. <br>
To preview an embed before you send it, type `/embed preview` followed by the JSON data for the embed. <br>
To create, update, or load an embed template, type `/embed template` followed by the template name and the JSON data for the embed, or the template name and the messageId of the embed. <br>
To delete an existing embed sent by the app, type `/embed delete` followed by the messageId of the embed. <br>

To view various help commands, type `/embed help` followed by the topic you want to view help for. Topics include `send`, `edit`, `preview`, `template`, and `delete`. <br>

## JSON Examples
Here are some examples of JSON data for embeds: <br>

Example with Fields:
```json
{
    "title": "Hello, World!",
    "description": "This is a test embed.",
    "fields": [
        {
            "name": "Field 1",
            "value": "This is the value of field 1.",
            "inline": true
        },
        {
            "name": "Field 2",
            "value": "This is the value of field 2.",
            "inline": true
        }
    ]
}
```

Example with Author, Footer, and Image:
```json
{
    "title": "Hello, World!",
    "description": "This is a test embed.",
    "author": {
        "name": "TooterTutor",
        "url": "https://github.com/TooterTutor/Discord-Embed-App/",
        "icon_url": "https://github.com/TooterTutor.png"
    },
    "footer": {
        "text": "TooterTutor's Discord Embed App",
        "icon_url": "https://github.com/TooterTutor.png"
    }
}
```