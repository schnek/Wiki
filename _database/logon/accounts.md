---
title: accounts
type: logondb
category: A
layout: single_markdown
---

# accounts
This table contains the information about the player accounts.

## Structure

Field                                     | Type         | Default             | Comment 
----------------------------------------- | ------------ | ------------------- | --------
[id](#id)                                 | int(10)      |                     | Auto Num
[acc_name](#acc_name)                     | varchar(32)  |                     |         
[encrypted_password](#encrypted_password) | varchar(42)  |                     |         
[banned](#banned)                         | int(10)      |                     |         
[lastlogin](#lastlogin)                   | timestamp    | 0000-00-00 00:00:00 |         
[lastip](#lastip)                         | varchar(16)  |                     |         
[email](#email)                           | varchar(64)  |                     |         
[flags](#flags)                           | tinyint(3)   | 0                   |         
[forceLanguage](#forceLanguage)           | varchar(5)   | enUS                |         
[muted](#muted)                           | int(30)      | 0                   |         
[banreason](#banreason)                   | varchar(255) | NULL                |         
[joindate](#joindate)                     | timestamp    | CURRENT_TIMESTAMP   |         

### id

The unique account id.

### acc_name

The account name

### encrypted_password

If you would switch from cleartext password to encrypted passwords, execute the following sql script:

```sql
UPDATE accounts SET encrypted_password = SHA(CONCAT(UPPER(login),":",UPPER(password)));
```

### banned

    0 = not banned (default)
    if it is not 0 it is unixtime,

### lastlogin

The timestamp the account logged in the last time.

### lastip

The ip address of the last login.

### email

The email address of the account.

### flags

The client flags:

    0 - Classic WoW
    8 - The Burning Crusade
    16 - Wrath of the Lich King
    24 - Wrath of the Lich King & The Burning Crusade
    32 - Cataclysm
    64 -  Mists of Pandaria (untested)
    128 - Warlords of Draenor (untested)
    256 - Legion (untested)

### forceLanguage

The lanuguage code:

Locale   | Name                         |
-------- | ---------------------------- |
koKR     | Korean                       |
frFR     | French                       |
deDE     | German                       |
zhCN     | Chinese                      |
zhTW     | Taiwanese                    |
esES     | Spanish (EU)                 |
esMX     | Spanish (Latin American)     |
ruRU     | Russian                      |

### muted

    0 = not muted (default)
    If it is not 0 it is unixtime.

### banreason

The reason for banning this account.

### joindate

Timestamp on account creation.
