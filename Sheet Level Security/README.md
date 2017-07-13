# Sheet Level Security

## Description
This rule package will use a custom property to mark which apps sheet level security
is applied to. If sheet level security is on only users in the group added to the
description of the sheet will get see the sheet in the app.

## Rules
| Rule     | Description |
|----------|-------------|
|Stream|If sheet level security is on for this app this rule should not apply|
|SheetLevelSecurity|if sheet level security is on for the app show only sheet where the current users is member of the group in the description of the sheet|

## Custom Properties
|Custom Property|Description|
|---------------|-----------|
|@SheetLevelSecurity|If set to Yes the app will apply sheet level security|
