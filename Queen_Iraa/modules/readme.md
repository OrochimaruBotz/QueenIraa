# Queen_Iraa Robot Example plugin format

## Advanced: Pyrogram
```python3
from pyrogram import filters
from Queen_Iraa import pgram

@pgram.on_message(filters.command("hi"))
async def hmm(_, message):
    await message.reply_text(
        "Namaste"
    )
    
__mod_name__ = "Hi"
__help__ = """
*Hi*
- /hi: Namaste
"""
```

## Advanced: Telethon
```python3
from Queen_Iraa import telethn
from Queen_Iraa.events import register

@register(pattern="^/hi$")
async def _(event):
    j = "Namaste"
    await event.reply(j)
    
__mod_name__ = "Hi"
__help__ = """
*Hi*
- /hi: Namaste
"""
```

## Advanced: PTB
```
PTB 13.7 Comming Soon
```
