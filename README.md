## Cowsay @coachdefracassos

```
 ________________________
< lute como nunca perca como sempre >
 ------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||--WWW |
                ||     ||

```
Comece o dia com frases "motivadoras" no seu terminal.

## Requisitos

* Jq
```
sudo apt install jq 
```

* Curl
```
sudo apt install curl
```

* Cowsay
```
sudo apt install cowsay
```

## Install



Se você utiliza o **bash**, cole o script abaixo no arquivo **.bashrc**. Ou se você utiliza o **zsh**, cole no arquivo **.zshrc**
 
```
curl -s  https://raw.githubusercontent.com/julianosirtori/Cowsay-coachdefracassos/master/frases.json | jq -r '.[] | .frase ' | sort -R | head -n 1 | cowsay -f www
```