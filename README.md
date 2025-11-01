# secmail_io
temp email web api 1secmail.io nim-lang
# Example
```nim
import asyncdispatch, secmail_io, json
waitFor init_cookie()
let data = waitFor get_messages()
echo data["mailbox"].getStr
let messages = waitFor get_messages()
echo messages["messages"]
```
# Launch (your script)
```
nim c -d:ssl -r  your_app.nim
```
