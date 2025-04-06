# my-karabiner-elements-settings

## Change control+; to delete (original)

```json
{
  "description": "Change control+; to delete (original)",
  "manipulators": [
    {
      "from": {
        "key_code": "semicolon",
        "modifiers": {
          "mandatory": ["control"],
          "optional": ["any"]
        }
      },
      "to": [{ "key_code": "delete_or_backspace" }],
      "type": "basic"
    }
  ]
}
```

## Change control to left_option (original)

```json
{
  "description": "Change control to left_option (original)",
  "manipulators": [
    {
      "from": {
        "key_code": "left_control",
        "modifiers": { "optional": ["any"] }
      },
      "to": [{ "key_code": "left_option" }],
      "type": "basic"
    }
  ]
}
```

## Change caps_lock to left_control (original)

```json
{
  "description": "Change caps_lock to left_control (original)",
  "manipulators": [
    {
      "from": {
        "key_code": "caps_lock",
        "modifiers": { "optional": ["any"] }
      },
      "to": [{ "key_code": "left_control" }],
      "type": "basic"
    }
  ]
}
```

## Map ctrl + / to ctrl + k

```json
{
  "description": "Map ctrl + / to ctrl + k",
  "manipulators": [
    {
      "from": {
        "key_code": "slash",
        "modifiers": {
          "mandatory": ["control"],
          "optional": ["any"]
        }
      },
      "to": [
        {
          "key_code": "k",
          "modifiers": ["control"]
        }
      ],
      "type": "basic"
    }
  ]
}
```

## Left ctrl + hjkl to arrow keys Vim

```json
{
  "description": "Left ctrl + hjkl to arrow keys Vim",
  "manipulators": [
    {
      "from": {
        "key_code": "h",
        "modifiers": {
          "mandatory": ["left_control"],
          "optional": ["any"]
        }
      },
      "to": [{ "key_code": "left_arrow" }],
      "type": "basic"
    },
    {
      "from": {
        "key_code": "j",
        "modifiers": {
          "mandatory": ["left_control"],
          "optional": ["any"]
        }
      },
      "to": [{ "key_code": "down_arrow" }],
      "type": "basic"
    },
    {
      "from": {
        "key_code": "k",
        "modifiers": {
          "mandatory": ["left_control"],
          "optional": ["any"]
        }
      },
      "to": [{ "key_code": "up_arrow" }],
      "type": "basic"
    },
    {
      "from": {
        "key_code": "l",
        "modifiers": {
          "mandatory": ["left_control"],
          "optional": ["any"]
        }
      },
      "to": [{ "key_code": "right_arrow" }],
      "type": "basic"
    }
  ]
}
```

## Ctrl+N for English input, Ctrl+M for Japanese Kana input

```json
{
  "description": "Ctrl+N for English input, Ctrl+M for Japanese Kana input",
  "manipulators": [
    {
      "from": {
        "key_code": "n",
        "modifiers": {
          "mandatory": ["control"],
          "optional": ["any"]
        }
      },
      "to": [{ "select_input_source": { "language": "en" } }],
      "type": "basic"
    },
    {
      "from": {
        "key_code": "m",
        "modifiers": {
          "mandatory": ["control"],
          "optional": ["any"]
        }
      },
      "to": [
        {
          "select_input_source": {
            "input_source_id": "com.apple.inputmethod.Kotoeri.RomajiTyping.Japanese",
            "language": "ja"
          }
        }
      ],
      "type": "basic"
    }
  ]
}
```

## Left Command + Control for English input, Right Command + Control for Japanese input

```json
{
  "description": "Left Command + Control for English input, Right Command + Control for Japanese input",
  "manipulators": [
    {
      "from": {
        "key_code": "left_command",
        "modifiers": {
          "mandatory": ["control"],
          "optional": ["any"]
        }
      },
      "to": [{ "select_input_source": { "language": "en" } }],
      "type": "basic"
    },
    {
      "from": {
        "key_code": "right_command",
        "modifiers": {
          "mandatory": ["control"],
          "optional": ["any"]
        }
      },
      "to": [
        {
          "select_input_source": {
            "input_source_id": "com.apple.inputmethod.Kotoeri.RomajiTyping.Japanese",
            "language": "ja"
          }
        }
      ],
      "type": "basic"
    }
  ]
}
```
