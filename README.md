# FRC-Tools
A Firebase web app that allows. 

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development, testing, and use.

### Prerequisites
This requires the [Firebase CLI](https://github.com/firebase/firebase-tools). To install just run:
```
$ npm install -g firebase-tools
```

You also need to create a Firebase Project on the Firebase Console.

In addition, you need to authenticate the Firebase CLI with your Google account by running:
```
$ firebase login
```

### Installation/Usage
Follow this guide to install FRC-Tools locally.

First clone this repository:
```
$ git clone https://github.com/SumiGovindaraju/FRC-Tools.git
```

Install prerequisites (see [Prerequisites](#prerequisites)).

To configure the Firebase project locally, run this and follow all instructions:
```
$ firebase init
```

Be careful not to overwrite `database.rules.json` or `public/index.html` and to select the multiple page web app setting.

To host this on a website, run:
```
$ firebase deploy
```

## Project Plan
A common practice that many FRC teams, including our own (Team 254: The Cheesy Poofs), do at competitions is lend tools and parts to other teams. However, we haven't found an elegant solution to keep track of all of the tools we've lent out. FRC-Tools fixes that.

FRC-Tools uses Firebase for realtime database storage and web hosting, and can keep track of who has borrowed tools, which team they are from, and what tools they have borrowed. When a tool is returned, that session is deleted from the database, keeping storage space to a minimum.

FRC-Tools was made to be portable. Using Firebase allows us to perform all the server-side functions without a server. Therefore, FRC-Tools can be added to any existing Pit Display or vice versa. Also, since this can be hosted on Firebase, FRC-Tools can be accessed by any device with an internet connection, making this project ideal for any FRC team.

## Built With
* [Firebase](https://firebase.google.com/) - Service/Library used for hosting and database
* [Bootstrap](https://getbootstrap.com/) - Library used for styling
* [jQuery](https://jquery.com/) - Bootstrap dependency 

## Authors
* Sumi Govindaraju

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details