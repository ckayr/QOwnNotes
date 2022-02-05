# Installeer op Raspberry Pi OS

## Raspberry Pi OS 11

Voer de volgende shell-opdrachten uit om de repository te vertrouwen.

```bash
wget http://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_11/Release.key -O - | sudo apt-key add -
```

Voer de volgende shell-opdrachten uit om de repository toe te voegen en vanaf daar QOwnNotes te installeren.

```bash
sudo bash -c "echo 'deb http://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_11/ /' >> /etc/apt/sources.list.d/qownnotes.list"
sudo apt-get update
sudo apt-get install qownnotes
```

[Directe download](https://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_11)

## Raspberry Pi OS 10

Voer de volgende shell-opdrachten uit om de repository te vertrouwen.

```bash
wget http://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_10/Release.key -O - | sudo apt-key add -
```

Voer de volgende shell-opdrachten uit om de repository toe te voegen en vanaf daar QOwnNotes te installeren.

```bash
sudo bash -c "echo 'deb http://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_10/ /' >> /etc/apt/sources.list.d/qownnotes.list"
sudo apt-get update
sudo apt-get install qownnotes
```

[Directe download](https://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_10)

## Raspbian 9.0

Voer de volgende shell-opdrachten uit om de repository te vertrouwen.

```bash
wget http://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_9.0/Release.key
-O - | sudo apt-key add -
```

Voer de volgende shell-opdrachten uit om de repository toe te voegen en vanaf daar QOwnNotes te installeren.

```bash
sudo bash -c "echo 'deb http://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_9.0/ /' >> /etc/apt/sources.list.d/qownnotes.list"
sudo apt-get update
sudo apt-get install qownnotes
```

[Directe download](https://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/Raspbian_9.0)
