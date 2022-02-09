# Repro

```
sfdx force:org:create --setdefaultusername -f config/project-scratch-def.json
sfdx force:source:beta:push
sfdx force:source:beta:push
```

Expected:
The second push should detect no changes

Actual: ERROR running force:source:beta:push:  We couldn't complete the push operation due to conflicts. Verify that you want to keep the local versions, then run "sfdx force:source:push -f" with the --forceoverwrite (-f) option.

