# Information
### DISCLAIMER: Everything shown here is intended for educational purposes. Please do not use any of this with ill intent
This respository was made to inform people on OSiNT (Open-source intelligence). For this we will be using [Google Cloud Console](https://console.cloud.google.com/) which is a completly free cloud profile platform.

## [PhoneInfoga](https://github.com/sundowndev/phoneinfoga):
```bash
docker pull sundowndev/phoneinfoga:latest
docker run -it -p 8080:8080 sundowndev/phoneinfoga serve -p 8080
```

## [Sherlock](https://github.com/sherlock-project/sherlock):
```bash
git clone https://github.com/sherlock-project/sherlock.git
cd sherlock
python3 -m pip install -r requirements.txt

python3 sherlock --timeout 2 [INSERT USERNAME HERE]
```

## [Twint](https://github.com/twintproject/twint):
```bash
git clone --depth=1 https://github.com/twintproject/twint.git
cd twint 
pip3 install . -r requirements.txt

twint -u [TWITTER USERNAME] --limit [NUMBER OF TWEETS]
```

However, you can also search for certain keywords using the following
```bash
twint -u [TWITTER USERNAME] -s "KEYWORD HERE" --limit [NUMBER OF TWEETS]
```

You can also add `-o data.json --json` to output it into a .json file called data.json

Some of the other things you can add are as followed:
`--min-likes [NUMBER]` to search tweets with a minimum amount of likes

`--since [YYYY/MM/DD]` search since a date.

`--year [YEAR]` specify a year

`--images` Only tweets with images

`--near [PLACE]`

`-g="[LONGITUDE], [LATITUDE], [RADIUS]"` Find tweets from certain coordiantes

## [Osintgram](https://github.com/Datalux/Osintgram)
```bash
git clone https://github.com/Datalux/Osintgram.git
cd Osintgram
pip install -r requirements.txt
mkdir config
cd config

echo "[YOUR INSTAGRAM USERNAME] > username.conf"
echo "[YOUR INSTAGRAM PASSWORD]" > pw.conf
echo "{}" > settings.json

cd ..
python3 main.py [USERNAME TO PERFORM OSINT ON] 
list

exit // Used to get out
cd output
ls
```

## [OSiNT Industrys](https://osint.industries/)
OSiNT Industrys is a website I highly reccomend. Just by using someones phone or email address you can gather a json file of data connected to that information. Click [here](https://osint.industries/) to use it!
