---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const regionalAndLanguageSettings = {
    defaultDisplayLanguage: {
        locale: 'en-US'
    },
    authoringLanguages: [
        {
            locale: 'fr-FR'
        },
        {
            locale: 'de-DE'
        }
    ],
    defaultTranslationLanguage: {
        locale: 'en-US'
    },
    defaultSpeechInputLanguage: {
        locale: 'en-US'
    },
    defaultRegionalFormat: {
        locale: 'en-GB'
    },
    regionalFormatOverrides: {
        calendar: 'Gregorian Calendar',
        firstDayOfWeek: 'Sunday',
        shortDateFormat: 'yyyy-MM-dd',
        longDateFormat: 'dddd, MMMM d, yyyy',
        shortTimeFormat: 'HH:mm',
        longTimeFormat: 'h:mm:ss tt',
        timeZone: 'Pacific Standard Time'
    },
    translationPreferences: {
        translationBehavior: 'Yes',
        languageOverrides: [
            {
                languageTag: 'fr',
                translationBehavior: 'Yes' 
            }
        ]
     }
};

await client.api('/me/settings/regionalAndLanguageSettings')
	.version('beta')
	.put(regionalAndLanguageSettings);

```