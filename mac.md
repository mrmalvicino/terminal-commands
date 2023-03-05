# MacBook terminal

## Comandos generales

- Consultar la aceleración del mouse (-1 sin aceleración, 3 aceleración máxima):

```
defaults read -g com.apple.mouse.scaling
```

- Cambiar la aceleración del mouse (a -1):

```
defaults write -g com.apple.mouse.scaling -integer -1
```