# Yelm.Chat
 Chat SDK 

Start Chat.Core - register with platform from Yelm.Server wiki and put user_id 

```swift
    YelmChat.start(platform: platform, user: user) {
      (load) in
      if (load) {
        YelmChat.core.register {
          (done) in
          if (done) {
            YelmChat.core.server(host: "https://chat.yelm.io/")
          }
        }
      }
    }
```
