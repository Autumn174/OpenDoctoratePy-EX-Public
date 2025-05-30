# DoctoratePy-EX-Public

[中文](https://github.com/jiellll1219/OpenDoctoratePy-EX-Public/tree/main/README.md) | [EN](https://github.com/jiellll1219/OpenDoctoratePy-EX-Public/tree/main/docs/README_EN.md) |

[Update Log (CN Only)](https://github.com/jiellll1219/OpenDoctoratePy-EX-Public/tree/main/docs/updata_log.md)

⚠Machine translation warning: This README is supported by machine translation⚠

This project serves as a branch of OpenDoctoratePy, aiming to expand and improve its functionality. The short-term goal is to prevent being kicked back to the login interface due to 404 or unknown errors as much as possible, while the long-term goal is to achieve a single-player local service similar to the SPT-AKI project.

The code and data structure for some features of this repository are based on [LocalArknight](https://github.com/jiellll1219/LocalArknight).

Development is purely driven by personal interest, and updates are made sporadically due to limited skills. If you encounter issues, please raise an issue, but I cannot guarantee prompt bug fixes (as a student, I only have free time during vacations or after school to write code).

This repository welcomes developers to propose pull requests. Collaborating on DoctoratePy is the original intention behind creating this repository.

If you need to contact me, please raise an issue or send an email to jiege0019@gmail.com.

This project has no community groups and prohibits any profit-driven redistribution or secondary development.

If you want to contribute code but lack data, you can at [Here](https://tptpmmpc.ap-southeast-1.clawcloudrun.com/) to get the il2cpp file, I will upload the il2cpp files for each version irregularly.

## Expansion Progress

| Target Feature | Progress | Completion Status | Remarks |
|:---:|:---:|:---:|:---:|
| Public Recruitment | Paused | Phantom bug |  |
| Targeted Search | Completed | Done | Tested |
| Building | Needs Improvement | Needs Improvement |  |
| Shop | Completed | Mostly Done | Can't Buy Anything |
| Recharge | Completed | Done |  |
| Interface Design | Completed | Done | Tested |
| CheckIn | Completed | Done | Tested |
| Activity CheckIn | Continuous updates | Mostly Done |  |
| Limited-time event | Continuous updates |  |  |
| SandBox | Paused |  |  |
| Friends | Paused |  |  |

## Declaration for Top-up System Code

# **The top-up system in this repository is completely unusable in a real payment environment. Please do not attempt to port this part of the code to your private repository. I will not upload the implementation code for this part to the public repository, as I do not want this repository to be subject to a DMCA Takedown.**

## Usage Guide Example

Please make sure that you are using a version of Python 3.11.0 or later, and that the datetime module of Python may be missing if it is lower than 3.11.0  
1. Search for GameData or dump game resources on your own to obtain the 'Excel' folder and its  contents, and place the 'Excel' folder in the 'data' directory  
2. Use the pip command to install the required modules ` pip install -r requirements.txt`  
3. Start the server by running 'start_dacal_Server. abt'  
4. Find a way to route the game to the server on your own, this repository does not provide a solution

If you think this is troublesome, you can also connect to my public server to experience it. The server address is `http://8.138.148.178:8443/`. My function development progress will also be synchronized to this server in ~~real time~~ sometime. Note! The version of this server is still a single-player version and does not support multi-user play. This server is located in China. The code structure used by the server is not completely consistent with the code of this warehouse, but the functions are basically the same

## Data Structure Explanation

The storage structure for some data in this project is based on [LocalArknight](https://github.com/jiellll1219/LocalArknight).

For detailed file structures and related files, please refer to this repository: [LocalArknight-res](https://github.com/jiellll1219/LocalArknight-res).

The game version of user.json provided by this repository is CN 2.4.41

## EX_Config Parameter Explanation

### virtualtime

Used for enabling old gacha pools. When the value is less than 0, real-time is returned.

It may cause issues with infrastructure. Avoid reducing the value unnecessarily once set.

Compatible with more time formats. You can directly input timestamps or formats like `"2024/02/02 12:12:12"` or `"2024-02-02 12:12:12"`. Ensure to use English double quotes `""`, include a space between date and time, and ensure the entered time is complete and reasonable.

### useMemoryCache

Control whether to use memory caching function, default to false (set to off). When enabled (set to true), this function will occupy at least 0.4GB of memory after starting the server, and will slightly reduce CPU usage, syncdata function time, and other functions that read table files. When this feature is not enabled, the memory usage after startup is around 80MB, and the maximum memory consumption is around 0.2GB. Please enable it as appropriate.

### useExistingCharData

When synchronizing data (SyncData), the default setting is false (set to off). Whether to use role data saved in user.exe for personalized role settings. When enabled (set to true) with role data, this feature can speed up function execution

## Keys in user.json

In the user dictionary of this file, the following items exist:

```json
"dungeon": {},
"activity": {},
"status": {},
"troop": {},
"npcAudio": {},
"pushFlags": {},
"equipment": {},
"skin": {},
"shop": {},
"mission": {},
"social": {},
"building": {},
"dexNav": {},
"crisis": {},
"crisisV2": {},
"nameCardStyle": {},
"tshop": {},
"gacha": {},
"backflow": {},
"mainline": {},
"avatar": {},
"background": {},
"homeTheme": {},
"rlv2": {},
"deepSea": {},
"tower": {},
"siracusaMap": {},
"sandboxPerm": {},
"openServer": {},
"trainingGround": {},
"storyreview": {},
"medal": {},
"inventory": {},
"limitedBuff": {},
"carousel": {},
"car": {},
"collectionReward": {},
"consumable": {},
"ticket": {},
"aprilFool": {},
"retro": {},
"campaignsV2": {},
"recruit": {},
"checkIn": {},
"share": {},
"charRotation": {},
"charm": {},
"firework": {},
"event": {}
