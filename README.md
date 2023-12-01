
# EchoVRCE
- EchoVRCE (pronounced "echo-verse") is short for **Echo VR Community Edition**
- This is what you are playing when you connect to community server for Echo VR
---
## FAQ

### If it is "EchoVRCE", why does everyone call it "Echo Relay"?
They don't. When someone says "Echo Relay" they are referring to the software running on the community servers.
If you want to get involved with that project, see [EchoRelay](https://github.com/EchoTools/EchoRelay)

### Didn't they shut down all the servers for Echo VR?
Yes, [ReadyAtDawn](https://www.readyatdawn.com/) did that on August 1st, 2023. Community servers went up on October 31, 2023 thanks to the work of [Xenomega](https://github.com/Xenomega) releasing the [EchoRelay](https://github.com/Xenomega/EchoRelay) project, and the [Echo Combat Lounge](https://discord.gg/echo-combat-lounge-779349159852769310) Discord community running it on their personal servers.

### How do I play?
There are about a hundred youtube videos, but the current recommendation is to use the [config.json](https://raw.githubusercontent.com/EchoVRCE/echovrce/main/src/config.json) in this repo. Replace the "USERNAME" and "PASSWORD" with the username you want and a completely random password. The password is not encrypted, so it should not be something you use anywhere else. Fortunately, you do not need to remember it, it just has to be unique. Then follow any instructions to get the config into your copy of the game. If you run into difficulty ask questions in the Echo Combat Lounge [help-channel](https://discord.com/channels/779349159852769310/1170584218649231390)

### Can I play Echo Arena on the Echo Combat Lounge servers?
Yes, Echo VR itself is unmodified. The only change during installation is to point to community servers. "Echo Combat Lounge" is the name largest group, and there are usually enough players online at any given time to play a round of Arena.

### Do I need a computer, or can I play on Quest?
Currently you need a computer to modify the configuration file to connect to a community server. However, after that initial setup, you do not need a computer. You can play Echo VR just like you did when the original servers were up.

### Does everything work?
There are a few quirks:
- The party system is not reliable, but [spark](https://ignitevr.gg/spark/) links work.
- Matchmaking does not take skill into account, so you may be playing against VRML players your first match.
- Emotes are not differentiated by left/right. Whatever you chose last will apply to both sides.
- In-game tints are ignored, but social tints work fine.
These quirks are due to the server side (Echo Relay) being built from the ground up without any knowledge of the original server code. They may be fixed as the EchoTools developers learn more about how Echo VR communicates with game servers.
