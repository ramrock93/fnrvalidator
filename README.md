fnrvalidator
================

[![CircleCI](https://circleci.com/gh/navikt/fnrvalidator.svg?style=svg)](https://circleci.com/gh/navikt/fnrvalidator)
[![npm version](https://badge.fury.io/js/%40navikt%2Ffnrvalidator.svg)](https://badge.fury.io/js/%40navikt%2Ffnrvalidator)

Validering for fødselsnummer og D-nummer. Alle fødselsnumre som forekommer her er autogenererte.

# Komme i gang

### Installasjon
```
npm install @navikt/fnrvalidator
```

### Bruk
```
const validator = require('@navikt/fnrvalidator')
const fnr = validator.fnr('12345678910')
const dnr = validator.dnr('52345678910')
// eller
const fnr = validator.nr('12345678910')
const dnr = validator.nr('52345678910')
```

### Resultat
```
{
   status: "valid"
   type: "fnr" || "dnr"
}
```

eller

```
{
   status: "invalid",
   reasons: ["some reason", "another reason"]
}
```

---


### Bygg og publisering
```npm run build && npm publish```

# Henvendelser

Spørsmål knyttet til koden eller prosjektet kan stilles som issues her på GitHub.

## For NAV-ansatte

Interne henvendelser kan sendes via Slack i kanalen #område-helse.
