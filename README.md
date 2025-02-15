# Customize Oh My Posh

### Review
![img](review-theme.png)

### [Scheme](quangthaictc.omp.json)
```json
{
    "palette": {
      "white": "#f7f7f7",
      "black": "#111111"
    },
    "blocks": [
      {
        "type": "prompt",
        "alignment": "left",
        "newline": true,
        "segments": [
          {
            "background": "transparent",
            "foreground": "#54C392",
            "style": "plain",
            "template": "\u250c",
            "type": "text"
          },
          {
            "background": "#464646",
            "foreground": "p:white",
            "properties": {
              "windows": "\ueb53",
              "linux": "\uf17c",
              "ubuntu": "\uf31b",
              "macos": "\uf179"
            },
            "style": "plain",
            "template": " {{.Icon}} \u2800",
            "type": "os"
          },
          {
            "background": "p:white",
            "foreground": "p:black",
            "style": "diamond",
            "template": " \uf489 {{ .Name }}\u2800",
            "trailing_diamond": "\ue0b0",
            "type": "shell"
          },
          {
            "background": "transparent",
            "foreground": "transparent",
            "style": "diamond",
            "template": " \uf489 \u2800",
            "trailing_diamond": "\ue0b0",
            "type": "text"
          },
          {
            "background": "#73EC8B",
            "foreground": "p:black",
            "style": "diamond",
            "template": " \uf2c0 {{.UserName}}  ",
            "trailing_diamond": "\ue0b0",
            "type": "session"
          },
          {
            "background": "transparent",
            "foreground": "transparent",
            "style": "diamond",
            "template": " \uf489 \u2800",
            "trailing_diamond": "\ue0b0",
            "type": "text"
          },
          {
            "background": "#54C392",
            "foreground": "p:black",
            "properties": {
              "branch_icon": " \ue0a0 "
            },
            "style": "diamond",
            "template": "\u2800{{.HEAD}} ",
            "trailing_diamond": "\ue0b0",
            "type": "git"
          },
          {
            "background": "transparent",
            "foreground": "transparent",
            "style": "diamond",
            "template": " \uf489 \u2800",
            "trailing_diamond": "\ue0b0",
            "type": "text"
          },
          {
            "background": "#15B392",
            "foreground": "p:white",
            "properties": {
              "windows": "\ue62a",
              "linux": "\uf17c",
              "ubuntu": "\uf31b",
              "macos": "\uf179"
            },
            "style": "diamond",
            "template": " {{.Icon}}{{if .WSL}} (WSL){{end}} ",
            "trailing_diamond": "\ue0b0",
            "type": "os"
          }
        ]
      },
      {
        "type": "prompt",
        "alignment": "left",
        "newline": true,
        "segments": [
          {
            "background": "transparent",
            "foreground": "p:white",
            "properties": {
              "folder_icon": "\uf07b",
              "folder_separator_template": "<#54C392> \u00bb </>",
              "home_icon": "\ueb06",
              "style": "agnoster"
            },
            "style": "plain",
            "template": "<#54C392>\u2514</><#54C392>[</> {{.Path}} <#54C392>] \uf101</>",
            "type": "path"
          }
        ]
      },
      {
        "type": "prompt",
        "alignment": "left",
        "newline": true,
        "segments": [
          {
            "background": "transparent",
            "foreground": "#15B392",
            "foreground_templates": [
              "{{if gt .Code 0}}#15B392{{end}}"
            ],
            "properties": {
              "always_enabled": true
            },
            "style": "plain",
            "template": "\u276f\u276f",
            "type": "status"
          }
        ]
      }
    ],
    "console_title_template": "{{if .Root}}[root] {{end}}{{.Shell}} in [{{.Folder}}]",
    "final_space": true,
    "version": 3
  }
```
