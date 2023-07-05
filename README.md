# trailsfc_jpsetup
## This repository provides the setup for studying Japanese of the PC Version of The Legend of Heroes: Trails in the Sky (FC)
- Contains compilation of sources found online to add voice lines to the game (Japanese) and change in-game text to Japanese
- Includes Extraction of Dialogue Text in the game for vocabulary/grammar study
- **Does not include combat voices (I am not sure have not tested it in combat yet, I will update once I tried it out)**
## 1. **Install the game**

## 2. **Download the Voice Pack:**
- https://drive.google.com/file/d/11b_3SgO90fdwHzhzH5p27E7LGawVl2Do/view

- Extract the voice pack to the Game Directory with the .exe file
- (Sample Directory: C:\Program Files (x86)\Steam\steamapps\common\Trails in the Sky FC)
- Full video tutorial provided by: https://www.youtube.com/watch?v=upaUO2aw-LA&ab_channel=choops
- To test try to launch the game and play a New Game, at this point there should be voice lines but the text will still be in English.

### ***If it's not working please check that you deployed the files in the correct directory***

## 3. **Change Dialogue Text to Japanese:**
- Download the scena folder which contains the Japanese voice:
- https://drive.google.com/file/d/1RNRVHCB-c-XRNWli_agXNdinVTy24JBW/view

- Extract to the /voice/scena directory.
- (Sample Directory: C:\Program Files (x86)\Steam\steamapps\common\Trails in the Sky FC\voice\scena)
- Overwrite everything (this will change the Dialogue Text from English to Japanese)
- Launch the game again and play a New game, the dialogue should be in Japanese with Japanese voice.
- ***Discussion (link provided by raeldor70): https://www.reddit.com/r/Falcom/comments/wc5pjp/are_there_any_text_hookers_for_trails_in_the_sky/***

### ***If it's not working please check the previous steps if they are working correctly***

## 4. **Download the latest release of Textractor**
- https://github.com/Artikash/Textractor/releases
- After installing Textractor, launch Textractor (x86)
- Launch the game in DX8 (This one worked for me reliably compared to the other options)
- Click "Attach to game" button found on Textractor, find the corresponding process (.exe) of the game
- After attaching the game, press "Add hook" button and input the following code: ***HS932#-18@51CDD0***
- If the text is incorrect try out ***HS932#-18@4E9130*** instead
- Once successful, the dialogue text should be captured by Textractor should appear (as shown below):
![Once successful the following should show up on Textractor1:](https://github.com/kurichon/trailsfc_jpsetup/blob/main/sample_textractor2.png)
![Once successful the following should show up on Textractor2:](https://github.com/kurichon/trailsfc_jpsetup/blob/main/sample_textractor3.png) 
![Once successful the following should show up on Textractor3:](https://github.com/kurichon/trailsfc_jpsetup/blob/main/sample_textractor.png)

For any issues regarding Textractor please visit (https://github.com/Artikash/Textractor/releases)

## 5. **(Optional) Change UI to Japanese**
- Go to the /dll folder (Sample Directory: C:\Program Files (x86)\Steam\steamapps\common\Trails in the Sky FC\dll)
- Create an empty file lang_jpn.dll
- ***Discussion: https://www.reddit.com/r/Falcom/comments/8uqs8q/instructions_on_how_to_apply_japanese_script_in/***
## 6. **(Optional) Change Dialogue to Japanese (without voice)**
- Follow the steps below:
- ***Discussion: https://www.reddit.com/r/Falcom/comments/8uqs8q/instructions_on_how_to_apply_japanese_script_in/***
## 7. **(Optional) Adjust the volume of the voice acting**
- Go to the /voice folder (Sample Directory: C:\Program Files (x86)\Steam\steamapps\common\Trails in the Sky FC\voice)
- Open "ed_voice.ini" file (This file is only generated once you launch the game once with Step 2 finished)
- Change it to desired volume

# Post-Setup
- Launch Textractor, followed by the game (Textractor will automatically use the hook you've set-up previously and automatically attached to the game when you launch it)
- The game should run with both Japanese Text and Voice, and all dialogue should be shown on Textractor
# Troubleshooting
- If nothing works, uninstall the game and clear up the remaining files in the installation directory
- (Sample Directory: C:\Program Files (x86)\Steam\steamapps\common\Trails in the Sky FC)
- Reinstall the game and try again from Step 2

# Additional Credits:
- Changing Dialogue Text to Japanese: http://modding.tistory.com/28
- Source Repository for the Voice Addon: https://github.com/ZhenjianYang/SoraVoice
- Wiki Page: https://www.pcgamingwiki.com/wiki/The_Legend_of_Heroes:_Trails_in_the_Sky
- Credits goes to all people who contributed to making this possible
