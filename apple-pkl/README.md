### Send file path on Windows

#### Convert Windows path to POSIX:

- Windows Path: `C:\tmp\teste.pkl`
- POSIX Path: `/C:/tmp/teste.pkl`

#### Example:
`pkl eval /C:/tmp/teste.pkl`
```
name = "Pkl: Configure your Systems in New Ways"
attendants = 100
isInteractive = true
amountLearned = 13.37
```
---
`pkl eval -f json /C:/tmp/teste.pkl`
```json
{
  "name": "Pkl: Configure your Systems in New Ways",
  "attendants": 100,
  "isInteractive": true,
  "amountLearned": 13.37
}
```
