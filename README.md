## Setup
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