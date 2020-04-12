# Emote Plugin for Oxide

Quite simple to use, basically just "`/me slaps himself silly`" to emote in the chat.

## Permissions

* `emote.use` - Allows player or group to use emotes

## Configuration

```json
{
  "Config":{
    "EnableEmotes":"false",
    "Text":"[#f0f0f0][i][b]{Player}[/b] {Message}[/i][/#]"
  },
  "Emotes":{
    ":$":"blushes",
    ":-$":"blushes",
    ":(":"sulks",
    ":-(":"sulks",
    ":)":"smiles",
    ":-)":"smiles",
    ":*":"blows a kiss",
    ":-*":"blows a kiss",
    ":@":"looks angry",
    ":-@":"looks angry",
    ":|":"is speechless",
    ":-|":"is speechless",
    ":=$":"blushes",
    ":=(":"sulks",
    ":=)":"smiles",
    ":=*":"blows a kiss",
    ":=@":"looks angry",
    ":=|":"is speechless",
    ":=d":"grins",
    ":=D":"grins",
    ":=p":"sticks out a tongue",
    ":=P":"sticks out a tongue",
    ":d":"grins",
    ":-d":"grins",
    ":D":"grins",
    ":-D":"grins",
    ":p":"sticks out a tongue",
    ":-p":"sticks out a tongue",
    ":P":"sticks out a tongue",
    ":-P":"sticks out a tongue",
    "\\o":"waves back",
    "]:)":"gives an evil grin",
    ">:)":"gives an evil grin",
    "o/":"waves",
    "x(":"looks angry",
    "x-(":"looks angry",
    "X(":"looks angry",
    "X-(":"looks angry",
    "x=(":"looks angry",
    "X=(":"looks angry"
  },
  "Plugin":{
    "Version":"1.0.1"
  }
}
```

## For Developers

```csharp
CheckForEmotes(IPlayer player, string message)
```

If an emote rule is matched this will return the string it would otherwise send to the chat. Otherwise, it will return your original message.