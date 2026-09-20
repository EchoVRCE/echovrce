# EchoVRCE

**EchoVRCE** (pronounced "echo-verse") is short for **Echo VR Community Edition**:
the community-run service that has kept Echo VR playable since Ready At Dawn shut
the official servers down on August 1, 2023. When you play Echo VR today, this is
what you are connected to.

## Official links

- Website: <https://echovrce.com>
- This GitHub organization: <https://github.com/EchoVRCE> — the project's config and website
- Code (servers, tools, the backend): <https://github.com/EchoTools>
- Echo VR Lounge Discord (the main player community, install help, matchmaking): <https://guilds.echovrce.com/echo-vr-lounge>
- EchoVRCE Discord (operators, hosts, service announcements): <https://guilds.echovrce.com/echovrce>

If a link, download, or Discord server claims to be EchoVRCE and is not reachable from
one of the places above, it is not ours.

## How do I play?

Start at <https://echovrce.com>. It links the two supported installs:

- **PC (PCVR, or a Quest tethered to a PC):** the
  [Echo VR Installer](https://github.com/marshmallow-mia/Echo-VR-Installer/releases).
  It downloads the game, keeps it updated, and applies the community patch if you never
  owned Echo VR on Meta. Its README points at the Lounge channels for PC and Quest setup
  and for help with specific errors.
- **Quest (standalone):** follow the guide at <https://quest.echovr.de/>.

Your in-game identity is your Discord account. Join the Echo VR Lounge before you
install; on first launch the game shows a link code, and you run `/link-headset` with
that code in the Lounge to tie the headset to your Discord account.

## What is `src/config.json`?

The service-endpoint file the community build of Echo VR points at. The installers
handle it for you; it is published here for anyone setting up by hand, and
<https://echovrce.com/config> redirects to the current copy. There is nothing to fill
in: sign-in is through Discord, not a username and password in the file.

## FAQ

### Didn't they shut down all the servers for Echo VR?

Yes. [Ready At Dawn](https://www.readyatdawn.com/) did that on August 1, 2023.
Community servers went up on October 31, 2023, thanks to
[Xenomega](https://github.com/Xenomega) releasing the
[EchoRelay](https://github.com/EchoTools/EchoRelay) project and the community that is
now the Echo VR Lounge running it on their own machines.

### Is this still "Echo Relay"?

Not any more. Echo Relay was the 2023 proof of concept the community launched on. Since
mid-2024 the live service has been a Nakama-based backend built for Echo VR by the
EchoTools developers: [EchoTools/nakama](https://github.com/EchoTools/nakama) (Discord
sign-in, matchmaking, game-server registry) with
[nevr-runtime](https://github.com/EchoTools/nevr-runtime) game servers. The config in
this repo switched to those endpoints on June 29, 2024. People still say "Echo Relay"
out of habit.

### Is Echo VR itself modified?

The game is the same game. The installer points it at the community service and,
for people who never owned it on Meta, applies a licence patch. Everything else is
server-side.

### Do I need a computer, or can I play on Quest?

Both work. PC players install with the Echo VR Installer. Quest players need a computer
once, to sideload the community build; after that the headset plays on its own. The
Quest guide at <https://quest.echovr.de/> walks through it.

### Does everything work?

Mostly, and it keeps improving; the backend and tools are under active development.
Current known issues, release notes, and service status are posted in the EchoVRCE
Discord (`#release-notes`, `#changelog`, `#service-updates`, `#server-status-updates`).
Ask in the Lounge's help channels if something on your end is broken.

### Can I host a game server?

Yes, on Windows or Linux:

- Windows: [EchoVR-Windows-Hosts-Resources](https://github.com/EchoTools/EchoVR-Windows-Hosts-Resources)
- Linux / Docker: [Echo-VR-Server-on-Docker](https://github.com/marshmallow-mia/Echo-VR-Server-on-Docker)

Game servers register with the central service, so hosting needs an operator account.
Ask in the EchoVRCE Discord before you start.

---

Echo VR is © Meta Platforms and Ready At Dawn. EchoVRCE is a fan-run project and is not
affiliated with, endorsed by, or supported by either of them.
