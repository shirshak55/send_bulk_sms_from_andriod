# Sending Bulk SMS from airdriod


## Intro

This project was initially intended to be used by marketers who wants to send sms to their customer from phone directly. Using dedicated api for sending sms using third party may be handy but it may not be useful to many small companies.

## Technology Used
Programming Lang: Rust

## Idea
Install airdriod app and send bulk sms using their unofficial api.

What I have done so far?
- They used des algorithm so I wrote a way to decrypt their payloads.


## How to use?
Create an excel file called data.xlsx (name can be changed from config.toml) with following headers
sms_content
send_sms 
phone_number

sms_content is the text you want to send to phone_number. Send sms is boolean where u set TRUE to 
corresponding rows you want to send.

Start the Airdriod app in andriod. Run it in web mode where u can use ip eg. 192.168.1.23:8888.
And run the following command in cmd or terminal

```
./airdriod_rs.exe
```


## Future?
- Rewrite gui in wpf (currenly I do have gui in druid but not exposed)
- Improve coding standard. To get work done I have used a lot of .clone and .to_string.
- Handle andriod sms rate api limit
- More api like exporting sms to excel etc.
