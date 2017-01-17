## hourCycle option on Intl.DateTimeFormat API Specification [draft]

### Status

Current Stage:

 * 🚀 __Stage 0__

Spec Text:

 * https://rawgit.com/zbraniecki/proposal-ecma402-hourcycle/master/out/

### Authors

 * Zibi Braniecki  (@zbraniecki)

### Reviewers

 * ?

### Informative

This proposal is based on the LDML spec, Part 1, 3.6.1 Unicode BCP 47 U Extension:

 * http://unicode.org/reports/tr35/#UnicodeHourCycleIdentifier

### Usage

```javascript
let o = new Intl.DateTimeFormat("en" , {
  hour: "numeric",
  minute: "numeric",
  hourCycle: "h24"
});
console.log(o.format(Date.now())); // "13:31"
```


### Render Spec

```bash
npm install
npm run build
open index.html
```

### Backpointers

 * https://github.com/tc39/ecma402/issues/105
