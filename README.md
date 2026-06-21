# QBX AI Ticket Bot

QBox FiveM серверийн Discord дээрх AI дэмжлэгийн ticket систем.

## Юу хийдэг вэ
- Тоглогч "Ticket нээх" товч дарж хувийн нууц суваг үүсгэнэ
- Сувгийг зөвхөн ticket нээгч, админ, bot гурав л харна
- AI туслах (Gemini) эхний хариуг өгнө, шаардлагатай бол админ нэгдэнэ
- "Ticket хаах" → баталгаажуулах → transcript архивлаад суваг устана

## Railway-д тохируулах хувьсагчид (Variables)

| Хувьсагч | Тайлбар |
|----------|---------|
| `DISCORD_TOKEN` | Bot-ийн token (Developer Portal) |
| `GEMINI_API_KEY` | Gemini API key (aistudio.google.com/apikey) |
| `GUILD_ID` | Discord серверийн ID |
| `PANEL_CHANNEL_ID` | "Ticket нээх" товч харагдах суваг |
| `TICKET_CATEGORY_ID` | Ticket сувгууд үүсэх category (заавал биш) |
| `ADMIN_ROLE_ID` | Ticket хардаг админ рол |
| `TRANSCRIPT_CHANNEL_ID` | Transcript архивлах суваг |

## Bot-д хэрэгтэй эрхүүд
`Manage Channels`, `Manage Roles`, `Send Messages`,
`Read Message History`, `View Channels`, `Attach Files`

## Анхаар
- Bot-ийн рол админ ролоос ДЭЭГҮҮР байх ёстой
- Developer Portal дээр **Message Content Intent**-ийг асаах
- ID авах: Discord Settings → Advanced → Developer Mode → баруун товч → Copy ID

## Асаах (локалд турших бол)
```
npm install
npm start
```
