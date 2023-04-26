## Debug Log

```log
DEBUG: migrateAndValidate() (repository=RahulGautamSingh-testing/fix-20539)
DEBUG: migrateConfig() error (repository=RahulGautamSingh-testing/fix-20539)
       "config": {
         "$schema": "https://docs.renovatebot.com/renovate-schema.json",
         "hostRules": [
           {
             "hostType": "nuget",
             "hostName": "nuget.org",
             "matchHost": "nuget.org",
             "username": "root",
             "password": "***********"
           }
         ]
       },
       "err": {
         "validationSource": "config",
         "validationMessage": "hostRules cannot contain more than one host-matching field - use \"matchHost\" only.",
         "validationError": "The renovate configuration file contains some invalid settings",
         "message": "config-validation",
...
DEBUG: findPr(renovate/configure, undefined, closed) (repository=RahulGautamSingh-testing/fix-20539)
DEBUG: ensureIssue(Action Required: Fix Renovate Configuration) (repository=RahulGautamSingh-testing/fix-20539)
 INFO: Issue created (repository=RahulGautamSingh-testing/fix-20539)
 WARN: Config Warning (repository=RahulGautamSingh-testing/fix-20539)
       "configError": {
         "validationSource": "config",
         "validationMessage": "hostRules cannot contain more than one host-matching field - use \"matchHost\" only.",
         "validationError": "The renovate configuration file contains some invalid settings",
         "message": "config-validation",
         "stack": "Error: config-validation\n    at validateHostRule (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\config\\migrations\\custom\\host-rules-migration.js:65:23)\n    at HostRulesMigration.run (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\config\\migrations\\custom\\host-rules-migration.js:14:13)\n    at Function.run (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\config\\migrations\\migrations-service.js:153:27)\n    at Object.migrateConfig (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\config\\migration.js:28:58)\n    at migrateAndValidate (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\config\\migrate-validate.js:13:64)\n    at mergeRenovateConfig (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\workers\\repository\\init\\merge.js:189:76)\n    at async getRepoConfig (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\workers\\repository\\init\\config.js:11:14)\n    at async initRepo (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\workers\\repository\\init\\index.js:34:14)\n    at async Object.renovateRepository (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\workers\\repository\\index.js:46:18)\n    at async attributes.repository (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\workers\\global\\index.js:139:17)\n    at async start (C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\workers\\global\\index.js:128:13)\n    at async C:\\Users\\LENOVO\\Desktop\\Whitesource\\renovate\\dist\\renovate.js:16:24"
       },
       "res": "created"
DEBUG: Repository result: config-validation, status: onboarded, enabled: true, onboarded: true (repository=RahulGautamSingh-testing/fix-20539)
```
