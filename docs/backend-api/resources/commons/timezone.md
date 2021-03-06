---
title: /timezone
description: /timezone
---

## list()
Information about all supported timezones for the specified locale. Does not require user authorization.

#### return:
```javascript
{
    "success": true,
    "list": [
        {
            "zone_id": <string>,     // timezone ID, which is used throughout the API, e.g. "Africa/Dar_es_Salaam"
            "description": <string>, // Localized description of the timezone, e.g. "Ekaterinburg"
            "base_offset": <double>,    // base timezone offset in hours, e.g. 4 for Moscow. May be negative or fractional!
            "dst_offset": <int>,     // DST offset in hours (0 if no DST rules for this timezone).
            "country_code": <string>, // ISO country code for timezone, e.g. "RU",
            "alt_ids": [<string>, <string>] //list of strings, optional, alternative timezone IDs
        },
        ...
    ]
}
```

#### errors:
*   only standard errors
