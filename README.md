# GDAPI

GDAPI is a API wrapper for the game called "Geometry Dash".

## Requirements
 - Python 2.25.1

## Installing
`pip install gdapi`

## Examples

### User info
```python
import gdapi
print(gdapi.user("RobTop"))

>>> {'username': 'RobTop', 'playerID': '16', 'accountID': '71', 'rank': 249576, 'stars': 1927, 'diamonds': 1399, 'coins': 3, 'userCoins': 113, 'demons': 5, 'cp': 0, 'friendRequests': False, 'messages': 'off', 'commentHistory': 'all', 'moderator': 2, 'youtube': 'UCz_yk8mDSAnxJq0ar66L4sw', 'twitter': 'RobTopGames', 'twitch': 'robtopgames', 'icon': 255, 'ship': 158, 'ball': 106, 'ufo': 118, 'wave': 92, 'robot': 65, 'spider': 67, 'col1': 6, 'col2': 3, 'deathEffect': 1, 'glow': True}

print(gdapi.user("RobTop")["playerID"])

>>> 16
```

### Level info

```python
import gdapi
print(gdapi.level(128))

>>> {'name': '1st level', 'id': '128', 'description': '(No description provided)', 'author': 'real storm', 'playerID': '30144023', 'accountID': '6338004', 'difficulty': 'Hard'...

print(gdapi.level(128)["name"])

>>> "1st level"
```
### Leaderboard

```python
import gdapi
print(gdapi.leaderboard(type="stars"))

>>> [{'rank': 1, 'username': 'Smiffy777', 'playerID': '7708568', 'accountID': '1413859', 'stars': 181060, 'demons': 4212, 'cp': 0, 'coins': 149, 'usercoins': 37044, 'diamonds': 123499, 'icon': {'form': 'icon'...

print(gdapi.leaderboard(type="cps")

>>> [{'rank': 1, 'username': 'ViPriN', 'playerID': '1078150', 'accountID': '2795', 'stars': 23817, 'demons': 697, 'cp': 278, 'coins': 149, 'usercoins': 3008, 'diamonds': 25515, 'icon': {'form': 'icon', 'icon': 133, 'col1': 11...
```

### Song verification

```python
import gdapi
print(gdapi.songV(1))

>>> True

print(gdapi.songV(0))

>>> False
```
## More
GDAPI: https://gdbrowser.com/api
License: GNU General Public License V3
I'll add more features later ;)
