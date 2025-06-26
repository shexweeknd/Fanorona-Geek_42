# Hackaton 24-06-2024

This project is part of the intra-university `hackathon` of `Ecole 42 Antananarivo`.

The theme for this hackathon is 🎆`Independence Day`🎆.

The event started on `2024-06-24 at 8 A.M`. and ended on `2024-06-25 at 12 P.M`.

## Team

The team is composed of `four strong members`. We are students at `42 Antananarivo` following the `Common Core Cursus`. Here are our **logins** in the **42 Global Network**:

@**anjrakot** [github profile](https://github.com/Fafafa12)

@**hramaros** [github profile](https://github.com/shexweeknd)

@**nrabarij** [github profile](https://github.com/nrabarij)

@**nrabehar** [github profile](https://github.com/nrabehar)

![profiles](https://github.com/w3bu1/blob/blob/main/hackaton_24_06_2024/profiles.png?raw=true)

## Technologies

This program is basically written in `C` and uses the `MinilibX` library as a graphical API. It also utilizes a `Node.js` script for network communication.

## Project Overview

Because the theme of the hackathon was `Independence day`, all the projects requested had to be related to `Malagasy traditions and customs`.

For our part, we decided to code our popular Malagasy game called `Fanorona`.

The game consists of ***two players***, opposing each other. 🤼‍♂️

#### Strategy

The game is played on a board of `3x3`, `5x5` or `9x5`. Represented as `[column]x[lines]`.

It has two sides, composed of stones (or any items which can represent the pawns). The `white` and `black` pawns take `alternate turns`, starting with white in order to capture the opposing pieces.

![fanorona](https://github.com/w3bu1/blob/blob/main/hackaton_24_06_2024/fanorona.png?raw=true)

There are two kinds of moves:

- A **non-capturing move**, which is called a `paika`.
- And a **capturing move**.

#### End conditions

If one player captures all opponent's stones, the game `ends` and the player `wins`.

Or, if neither player can achieve this, the game ends with a `Draw`. 🤝🏽

#### Challenges

We faced the challenge of creating a simple game, yet enjoyable. 💁🏽

The real deal is to be able to play the game from `two different computers`, by transmitting player's data through a `server` which will display the board on each client's side. 🤔

## Usage

Currently we are working on public deployment in order to make the game enjoyable online. 🔗

If you want to test `fanorona` locally, here are the steps:

- Prerequisites:

1. **Linux OS (preferred Stable Version)**
2. **Build-Essentials**
3. **NodeJs**

- Clone the project:

```bash
git clone https://github.com/w3bu1/hackaton_24_06_2024.git
```

- Go to the root directory and compile the game:

```bash
cd hackathon_24_06_2024/ &&\

make &&\

cd ../
```

At the root directory (`hackathon_24_06_2024`), open `three terminals`:

1. The `first one` should launch the `local server`.
2. The `second one` will launch the `first player` program.
3. The `third one` will lauch the `second player` program.

- Launch the local server on the first Terminal:

```bash
cd server/ &&\

node index.js
```

>Note: You will see the broadcast messages from the server, don't touch anything in this terminal, if you still want to test the game, otherwise you are gonna need to relaunch the server with `nodejs`. 😁

- Launch the first player in the second Terminal:

```bash
cd client/ &&\

./fanorona 127.0.0.1
```

>Note: The provided command will display the first player interface. You still can not play the game until another player joins the room. 🫠

- Finally launch the second player in the third Terminal:

```bash
cd client/ &&\

./fanorona 127.0.0.1
```

Enjoy the game 😎

- Stopping the game:

If you want to `close efficiently everything` like a pro just close the windows of the players, go to the `first Terminal` (the one that displays broadcast messages) and type `Ctrl + C`. 😎

## Acknowledgements

- **Ntaolo Malagasy**
- **All Teammates**
- **Axian Group**
- **42 Antananarivo**
- **YAS Madagascar**
- **NextA**
- **MinilibX contributors**
