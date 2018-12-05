# VSS_ShadowCopyStats_AWSSNSnotifications
Get VSS shadow copy stats for all drives on a file server via email using powershell and AWS SNS

The script sends an email via AWS SNS in json with the following example output:

    [
        {
            "SystemName":  "ABCFS01",
            "DriveLetter":  "C:",
            "CapacityGB":  69.66,
            "FreeSpaceGB":  32.7,
            "ShareCount":  3,
            "Shares":  "ADM$, C$, printerdata$",
            "ShadowAllocatedSpaceGB":  6.96,
            "ShadowUsedSpaceGB":  6.7,
            "ShadowMaxSpaceGB":  6.96,
            "DiffVolumeDriveLetter":  "C:",
            "DiffVolumeCapacityGB":  69.66,
            "DiffVolumeFreeSpaceGB":  32.7,
            "ShadowCopyCount":  21,
            "OldestShadowCopy":  "Tuesday, 27 November 2018 12:00:00 PM",
            "LatestShadowCopy":  "Wednesday, 5 December 2018 12:00:00 PM",
            "ShadowAverageSizeGB":  0.32,
            "ShadowAverageSizeMB":  326.7
        },
        {
            "SystemName":  "ABCFS01",
            "DriveLetter":  "D:",
            "CapacityGB":  5999.87,
            "FreeSpaceGB":  680.38,
            "ShareCount":  2,
            "Shares":  "D$, CorpData$",
            "ShadowAllocatedSpaceGB":  119.36,
            "ShadowUsedSpaceGB":  116.92,
            "ShadowMaxSpaceGB":  599.99,
            "DiffVolumeDriveLetter":  "D:",
            "DiffVolumeCapacityGB":  5999.87,
            "DiffVolumeFreeSpaceGB":  680.38,
            "ShadowCopyCount":  64,
            "OldestShadowCopy":  "Friday, 9 November 2018 7:01:02 AM",
            "LatestShadowCopy":  "Wednesday, 5 December 2018 12:01:04 PM",
            "ShadowAverageSizeGB":  1.83,
            "ShadowAverageSizeMB":  1870.72
        },
        {
            "SystemName":  "ABCFS01",
            "DriveLetter":  "E:",
            "CapacityGB":  3021.87,
            "FreeSpaceGB":  826.76,
            "ShareCount":  2,
            "Shares":  "E$, AppData$",
            "ShadowAllocatedSpaceGB":  11.87,
            "ShadowUsedSpaceGB":  11.21,
            "ShadowMaxSpaceGB":  19.53,
            "DiffVolumeDriveLetter":  "S:",
            "DiffVolumeCapacityGB":  59.87,
            "DiffVolumeFreeSpaceGB":  44.69,
            "ShadowCopyCount":  43,
            "OldestShadowCopy":  "Wednesday, 21 November 2018 11:00:03 AM",
            "LatestShadowCopy":  "Wednesday, 5 December 2018 11:00:03 AM",
            "ShadowAverageSizeGB":  0.26,
            "ShadowAverageSizeMB":  266.95
        }
    ]

