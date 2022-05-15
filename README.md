# About
This is a demo to use GPT-3 to summarize a YouTube video based on the captions.

# Examples
⚠️ __Disclaimer__ ⚠️ Examples below are selected from instances where GPT-3 was fairly accurate. There has been cases where the summary failed to capture the main topic of the video. 


[![Thumbnail](https://img.youtube.com/vi/cB4Dzc-qUzk/0.jpg)](https://www.youtube.com/watch?v=cB4Dzc-qUzk)
- Title: __Top 10 Happy Meal Toy Fails__ 
- CLI: `python main.py --video_id cB4Dzc-qUzk --title_type top10`
- Summary:
```
Top 10 Happy Meal Toy Fails
1. American Idol MP3 Player: A thin plastic MP3 player that played the American Idol theme song on repeat.
2. Zizzle Izzes: Creepy plastic figurines that did not take off with children.
3. Toothbrush and Toothpaste: A toothbrush and toothpaste offered in place of a toy in 1983.
4. Pop Boys: A bunch of meaningless pieces of plastic that children could connect to create nothing.
5. McDonald's Character Sunglasses: Plastic sunglasses that were unattractive and had inappropriate undertones.
6. Mighty Ducks Pucks: Hockey pucks that were advertised as functional but shattered easily.
7. Tickle Feather Sponge: A long yellow foam cutout that was intended for use in tickling.
8. Spider-Man 2 Girl Toys: Toys for girls that were just Spider-Man stuff colored pink and purple.
9. Cursing Minions: Talking minion figurines that said expletives when their words were translated.
```
---

[![Thumbnail](https://img.youtube.com/vi/kqnvrjgyEMc/0.jpg)](https://www.youtube.com/watch?v=kqnvrjgyEMc)
- Title: __Faster Internet for FREE in 30 seconds - No... Seriously__
- CLI: `python main.py --video_id kqnvrjgyEMc --title_type general`
- Summary: The article discusses how Cloudflare's new DNS service, 1.1.1.1, is faster and more private than other DNS providers. The article explains how DNS works and how Cloudflare's new service is faster and more private than other DNS providers. The article also explains how to configure your devices to use 1.1.1.1 and how to use it to improve your internet speed.

---

[![Thumbnail](https://img.youtube.com/vi/1N12nBGlxc0/0.jpg)](https://www.youtube.com/watch?v=1N12nBGlxc0)
- Title: __Can You WATERPROOF Your Entire Body?__
- CLI: `python main.py --video_id 1N12nBGlxc0 --title_type question`
- Summary: No, you cannot waterproof your entire body.

# Setup
Install dependencies.
```bash
pip install -r requirements.txt
```
Create a file called `secret.toml` in the directory. It should look like this:
```toml
openai-key = "<your openai api key>"
```
Run from cli
```bash
 python main.py --video_id <id of video> --title_type top10
```

If the id of the video starts with a `-` character, the CLI may mistake it as a keyword. In such case, prepend the id with an `@`. For example:
```bash
 python main.py --video_id <id of video> --title_type top10
```


