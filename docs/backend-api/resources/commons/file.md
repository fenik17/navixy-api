---
title: /file
description: /file
---

## stats/read

Get user’s files statistic.

#### return:

    {
        "success": true,
        "value": {
            "file_count": 24,       // count of all updloaded files 
            "total_size": 40192953  // total files size in bytes
            "quota": 104857600      // space available to the user in bytes
        }
    }