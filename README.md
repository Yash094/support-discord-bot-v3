# thirdweb Support Bot

A dedicated forum-based support Discord bot for the thirdweb community. This bot is created specifically for the community setup of thirdweb community. If you want to use the bot would recommend to use the [public version](https://github.com/warengonzaga/forum-based-support-discord-bot) of it.

## 🤔 How to Use

This bot has only one command to use, for auto closing the posts from forum channels.

- Make sure the forum post has tags that is required before posting.
- Add proper permission to the bot to avoid unexpected issues.

### Commands

To close thread using prefix command.

```bash
!close
```

To close the thread and resolved by the username mentioned

```bash
!close @username
```

## 🎛️ Configurations

### Config File

```json
{
    "resolution_tag_name": "Solved",
    "command_prefix": "!",
    "utc_offset": -8,
    "datasheet_init": "init",
    "datasheet_response": "response",
    "datasheet_resolve": "resolve",
    "mention_message": "Hello there! If you need help, please read the information in <#1074862134284005396> and post your questions or issues in the <#1029543258822553680> channel. Our team and community members are always ready to help you out. Thank you for building with us!"
}
```

| Config Name | Description |
| --- | --- |
| `resolution_tag_name` | The name of the tag to mark the post resolved. |
| `command_prefix` | A prefix you want to use with `close` command to be recognized by the bot. |
| `utc_offset` | Time and date UTC offset for recording the data. |
| `datasheet_init` | Refers to the sheet name in your google spreadsheet. This should be the first sheet in the order. |
| `datasheet_response` | Refers to the sheet name in your google spreadsheet. This should be the second sheet in the order. |
| `datasheet_resolve` | Refers to the sheet name in your google spreadsheet. This should be the third sheet in the order. |
| `mention_message` | The message bot will send if the bot mentioned by the user, you can use use the channel ids to mention it within the bot message. |

## 👁️ Environment Variables

```env
DISCORD_BOT_TOKEN=<discord_bot_token>
DISCORD_SUPPORT_ROLE_ID=<role_id>,<role_id>
GOOGLE_PRIVATE_KEY=<private_key>
GOOGLE_SERVICE_ACCOUNT_EMAIL=<service_email_account>
GOOGLE_SPREADSHEET_ID=<google_spreadsheet_id>
```

## 💻 Development

### Install the packages

```bash
yarn install
```

### Run the bot

```bash
yarn dev
```

## 📃 License

The Forum-based Support Bot (thirdweb support) is licensed under [GNU General Public License v3](https://opensource.org/licenses/GPL-3.0).

## 📝 Author

The Forum-based Support Bot (thirdweb support) is developed and maintained by **[Waren Gonzaga](https://github.com/warengonzaga)**, with the help of awesome [contributors](https://github.com/warengonzaga/thirdweb-support-discord-bot/graphs/contributors) for the [thirdweb community](https://discord.gg/thirdweb).

[![contributors](https://contrib.rocks/image?repo=warengonzaga/thirdweb-support-discord-bot)](https://github.com/warengonzaga/thirdweb-support-discord-bot/graphs/contributors)

---

💻💖☕ by [Waren Gonzaga](https://warengonzaga.com) | [He is Awesome](https://www.youtube.com/watch?v=HHrxS4diLew&t=44s) 🙏
