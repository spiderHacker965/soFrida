# soFrida

With soFrida, you can analyze and detect Cloud API key misconfigurations automatically via dynamic analysis.

This tool willl be released on August (Maybe Defcon 27 Conference)

## How it works?

soFrida find the cloud-misconfiguraion vulnerability with three steps.

Step 1. Check if key-pairs are extraced by launching app

Step 2. Call every possible activities of app while hooking, if no result on Step 1.

Step 3. You can manually set the class name related to cloud authentication and trace all methods.
        
        In this case, you may need to trigger app to cause loading cloud APIs.

## Getting Started

This tool is intended to test APIBleed vulnerability - cloud backend - not for testing general mobile vulnerability.

What you need is as following :

* Android smartphone (Rooted) : newer is better

* Package name : com.test.abc

```
python3 soFrida.py -t "TARGET_APK_Filename"
```

If you want to dwonload app from Google Playstore, use following command

```
python3 pluto.py -e "YOUR_GOOGLE_ID" -p "YOUR_GOOGLE_PASSWORD" -t "TARGET_PKG_NAME"
```

## Dependencies

Install dependent packages with command as following.

```sudo pip install -r requirements.txt```

## Other Useful Codes

You can check How many users downloaded the app with following code.

```python3 get_popularity.py [PKG_LIST_TEXT] ```


## Authors

**Hyunjun Park** - Graduate student of SANE(Security Analysis aNd Evaluation) Lab at Korea Unviersity / Senior Engineer of Samsung SDS

**Soyeon Kim** - Engineer of Samsung SDS

**Yeongjin Jang** - Assistant professor of Computer Science at Oregon State Univeristy

**Seungjoo (Gabriel) Kim** - Professor of Graduate School of Information Security at Korea University /  Head of SANE (Security Analysis aNd Evaluation) Lab.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details