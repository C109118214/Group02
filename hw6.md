![ERD](png.png)

// Entity: Chatbot

class Chatbot {
  constructor(ID, name, avatar, userID, guildID) {
    this.ID = ID;
    this.name = name;
    this.avatar = avatar;
    this.userID = userID;
    this.guildID = guildID;
  }
}

// Entity: User

class User {
  constructor(ID, name, avatar, discordID) {
    this.ID = ID;
    this.name = name;
    this.avatar = avatar;
    this.discordID = discordID;
  }
}

// Entity: Guild

class Guild {
  constructor(ID, name, discordID) {
    this.ID = ID;
    this.name = name;
    this.discordID = discordID;
  }
}

// Relationship: Chatbot is associated with a User

class ChatbotUser {
  constructor(chatbotID, userID) {
    this.chatbotID = chatbotID;
    this.userID = userID;
  }
}

// Relationship: Chatbot is associated with a Guild

class ChatbotGuild {
  constructor(chatbotID, guildID) {
    this.chatbotID = chatbotID;
    this.guildID = guildID;
  }
}
