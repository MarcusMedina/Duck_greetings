# 🦆 Duck Events - The Geeky Terminal Greeter

Welcome to **Duck Events**, a quirky, fun, and surprisingly informative Bash script that supercharges your terminal's welcome message. This script was born from a collaboration between **Marcus** and **Gemini** and **ChatGPT** with the goal of making every new shell session a delightful experience.

Instead of a blank prompt, you'll be greeted by our friendly ASCII duck and a curated list of events for the day, including everything from geeky movie premieres to ancient pagan holidays.

## ✨ Features

  * **Friendly ASCII Duck:** Every session starts with a charming ASCII art duck from https://kaomojis.wiki/duck-ascii-art
  * **The Canon Nerd Chart:** A huge, curated list of important dates, including:
      * **Sci-Fi Premieres:** The complete timelines for every *Star Trek* series and key dates from the *Star Wars*, *Alien*, and *Doctor Who* universes.
      * **Gaming Legends:** Anniversaries for iconic games like *DOOM*, *Zelda*, *Minecraft*, and *Half-Life*.
      * **Tech History:** Key moments like the release of C\# 1.0 and the first GSM call in Stockholm.
  * **Astro & Seasonal Vibes:** Know the current Zodiac sign and get nuanced seasonal greetings based on astronomical events and ancient holidays (Sabbats).
  * **Time-Sensitive Greetings:** Get special messages for "Leet O'Clock" (13:37) if you log in at that exact time, Blue Monday, and different advice for weekdays vs. weekends.
  * **Optimized & Clean:** The script is refactored to be efficient, calling `date` only once per run.
  * **Easy to Personalize:** A clearly marked section at the top makes it simple to add your own birthdays, anniversaries, and reminders.

## Sample Output

Here's a taste of what you might see when you open your terminal:

```
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣤⡶⠿⠿⠷⣶⣄⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣰⡿⠁⠀⠀⢀⣀⡀⠙⣷ ⠀⠀⠀
⠀⠀⠀⡀⠀⠀⠀⠀⠀⢠⣿⠁⠀⠀⠀⠘⠿⠃⠀⢸⣿⣿⣿⣿
# ... and so on ...

The duck welcomes you marcus 2025-09-21 at 14:09:00...

Today's Zodiac sign is ♍ Virgo.
🕊️ International Day of Peace.
🎬 Andor premiered (2022).
🍂 Autumn Equinox (Mabon). A time of balance.
✨ Have a quack day, and don't quack it up!
```

## 🏁 Installation

Getting the duck into your terminal is easy.

**Step 1: Get the Script**

Clone this repository to your home directory:

```
git clone https://github.com/MarcusMedina/Duck_events.git ~/duck-events
```

Alternatively, you can just download the `duck_events.sh` file and save it in your home directory (`~/`).

**Step 2: Make it Executable**

Navigate to the directory and make the script runnable:

```
cd ~/duck-events
chmod +x duck_events.sh
```

**Step 3: Add it to Your Shell Configuration**

The final step is to tell your shell to run the script every time it starts. Open your shell's configuration file (`.bashrc` for Bash, `.zshrc` for Zsh, etc.) with a text editor:

```
nano ~/.bashrc   # Or nano ~/.zshrc for Zsh
```

Add the following line to the very end of the file:

```
# Run the Duck Events greeter
if [ -f ~/duck-events/duck_events.sh ]; then
    ~/duck-events/duck_events.sh
fi
```

Save the file, close it, and open a new terminal. Your duck should now be there to greet you\!

## 🔧 Customization

This script is meant to be yours\! Open the `duck_events.sh` file and find the section at the top labeled `STEP 1: Personal Dates & Reminders`. You can easily add, edit, or remove any dates to make it perfectly tailored to you.

## Collaboration

If you are missing any geeky dates, send a pull request.

## 📄 License

This project is licensed under the GNU3 License. See the `LICENSE` file for details.
